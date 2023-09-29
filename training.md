---
layout: page
title: Open Science 101
---

<html>

<div>
    <input
        id="search-input"
        type="search"
        class="input-group-text form-control rounded"
        placeholder="Search"
        aria-label="Search"
        aria-describedby="search-addon"
    />
</div>

<!-- This divs are rendered dynamically by the javascript functions below based on the _data/educationals.csv file -->
<div id="tags-contents" class="educational-tags-container"></div>
<div id="educational-contents"></div>



<script>
function getUniqueTags() {
    const educationals = {{ site.data.educational | jsonify }};
    let allTags = [].concat.apply([], educationals.map(educ => educ.Tags.split(',')));
    allTags.push("All");
    const uniqueTags = [...new Set(allTags)];
    uniqueTags.sort();

    return uniqueTags
}

function getTagColorClassName(tag) {
    const availableColors = ["", "pink-tag", "purple-tag"];
    const allTags = getUniqueTags();

    const tagPosition = allTags.indexOf(tag);
    
    return availableColors[tagPosition % availableColors.length];
}

function getFilteredEducationalsByContent(filterValue) {
    const educationals = {{ site.data.educational | jsonify }};
    return educationals.filter(educ => (educ.Name.toLowerCase().includes(filterValue.toLowerCase())));
}
function getFilteredEducationalsByTag(tagValue) {
    const educationals = {{ site.data.educational | jsonify }};
    return educationals.filter(educ => (educ.Tags.toLowerCase().includes(tagValue.toLowerCase())));
}

function buildLinkDiv(educational) {
    let linksDiv = `<div class="educational-links">`;
    if (educational.Link && educational.Link !== "" && educational.Link.includes("youtu")) {
        linksDiv += `<a href=${educational.Link} target="_blank"><img class="educational-link" src="../img/youtube-logo.svg"></a>`;
    }
    if (educational.Douyu && educational.Douyu !== "") {
        linksDiv += `<a href=${educational.Douyu} target="_blank"><img class="educational-link" src="../img/Douyu-logo_geg.svg"></a>`;
    }
    linksDiv += `</div>`;
    return linksDiv;
}

function renderEducationalDiv(educationals) {
    const mainCategories = ["Open Access", "Open Data", "Open Code", "Reproducibility", "Research Integrity", "Research Culture"];
    let educationalHTML = `<div class="educational">`;

    mainCategories.map(category => {
        const relevantEducationalsForCategory = educationals.filter(educational => educational.Tags.includes(category));

        if (relevantEducationalsForCategory.length > 0) {
            educationalHTML += `<div class="row"><h3>${category}</h3></div>`;
            educationalHTML += "<div class='educational-cards'>";
            relevantEducationalsForCategory.map((educational) => {
                const titleDiv = `<div class='educational-card-title'><a href=${educational.Link}>${educational.Name}</a></div>`;
                const descriptionDiv = `<div class='educational-card-description'>${educational.Description}</div>`;
                const linksDiv = buildLinkDiv(educational);
                educationalHTML += `
                    <div class='educational-card'>
                        ${titleDiv}
                        ${descriptionDiv}
                        ${linksDiv}
                    </div>
                `;
            });
            educationalHTML += "</div>";
        }
    });

    educationalHTML += `</div>`;

    // Finally add the cards inside the appropriate div
    document.getElementById("educational-contents").innerHTML = educationalHTML;
}

function renderAllEducationals() {
    renderEducationalDiv({{ site.data.educational || jsonify }});
}

function renderTags() {
    let tags = getUniqueTags();

    // Add additional "All" tag to let user reset the list
    let tagsHTML= ""
    // let tagsHTML = "<a class='btn btn-primary tag-button ${getTagColorClassName('All')}'>All</a>";
    // Add all other tags available in the educationals data file
    tags.map((tag) => {
        const tagColorClassName = getTagColorClassName(tag);
        tagsHTML += `<a class="btn btn-primary tag-button ${tagColorClassName}">${tag}</a>`;
    });

    document.getElementById("tags-contents").innerHTML = tagsHTML;
}

renderTags();
renderAllEducationals();

<!-- Add listeners to handle interactions with the search -->

<!-- This first one is the filtering by clicking on the tag buttons -->
let tagButtons = document.getElementsByClassName("tag-button");
for (let index = 0; index < tagButtons.length; index++) {
    tagButtons[index].addEventListener('click', (event) => {
        <!-- If the value is "All", it means we want to display all the cards -->
        const tagValue = event.target.outerText === "All" ? "" : event.target.outerText;
        const filteredEducationals = getFilteredEducationalsByTag(tagValue);
        renderEducationalDiv(filteredEducationals);
    })
}

<!-- This second one is by leveraging what the users write in the search bar -->
document.getElementById('search-input').addEventListener('keyup', (event) => {
    const inputValue = event.target.value;
    const filteredEducational = getFilteredEducationalsByContent(inputValue);
    renderEducationalDiv(filteredEducational);
});

</script>



</html>
