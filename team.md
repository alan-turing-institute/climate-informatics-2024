---
layout: page
title: Team
---

Organising contributors to this conference are the members of [Turing Environment and Sustainability Grand Challege](https://www.turing.ac.uk/research/environment-and-sustainability) Operations team, and the [Climate Informatics Community](http://www.climateinformatics.org). 

If you would like to support or engage with the delivery of this meeting, we'd live to hear from you! Please [Contact Us!](../contact)


## MCs and Session Chairs
- [Alden Conner](https://www.turing.ac.uk/people/business-team/alden-conner)
- [Andrew McDonald](https://ampersandmcd.com/)
- [Cassandra Gould van Praag](https://www.turing.ac.uk/people/researchers/cassandra-gould-van-praag)
- [Douglas Rao](https://ncics.org/people/douglas-rao/)
- [Guillaume Couairon](https://gcouairon.github.io)
- [Katy Thompson](https://www.turing.ac.uk/people/business-team/katy-thompson)
- [Kenza Tazi](https://www.bas.ac.uk/profile/kenzi22/)
- [Meghna Asthana](https://www.turing.ac.uk/people/meghna-asthana)
- [Orlando Timmerman](https://biomin.esc.cam.ac.uk/people/2023-Orlando-Timmerman/)
- [Ricardo Barros Lourenço](https://about.me/ricardobarroslourenco) 
- [Scott Hosking](https://www.turing.ac.uk/people/researchers/scott-hosking)
- [Viviana Acquaviva](https://www.drvivianaacquaviva.com)


## Local organising committee
- [Scott Hosking](https://www.turing.ac.uk/people/researchers/scott-hosking) (Chair)
- [Katy Thompson](https://www.turing.ac.uk/people/business-team/katy-thompson) (Treasurer & Events Lead)
- [Léllé Demertzi](https://www.turing.ac.uk/people/business-team/lelle-demertzi) (Secretary)
- [Cassandra Gould van Praag](https://www.turing.ac.uk/people/researchers/cassandra-gould-van-praag) (EDI Champion)
- [Alden Conner](https://www.turing.ac.uk/people/business-team/alden-conner) (Partnerships)

## Online participation
- [Orlando Timmerman](https://biomin.esc.cam.ac.uk/people/2023-Orlando-Timmerman/)
- [Meghna Asthana](https://www.turing.ac.uk/people/meghna-asthana)
- [Katy Thompson](https://www.turing.ac.uk/people/business-team/katy-thompson)
- [Léllé Demertzi](https://www.turing.ac.uk/people/business-team/lelle-demertzi)

## Reproducibility
- [Alejandro Coca Castro](https://www.turing.ac.uk/people/researchers/alejandro-coca-castro)
- [Andrew Hyde](https://www.linkedin.com/in/andrew-hyde-b8913957/?originalSubdomain=uk) (Open Access publishing)
- [Dominic Orchard](https://dorchard.github.io)
- [Marion Weinzierl](https://iccs.cam.ac.uk/about-marion-weinzierl)
- [Roly Perera](https://dynamicaspects.org/research/)

# Programme Committee
- [Alejandro Coca Castro](https://www.turing.ac.uk/people/researchers/alejandro-coca-castro)
- [Guillaume Couairon](https://gcouairon.github.io)
- [Cassandra Gould van Praag](https://www.turing.ac.uk/people/researchers/cassandra-gould-van-praag)
- [Andrew McDonald](https://ampersandmcd.com/)
- [Douglas Rao](https://ncics.org/people/douglas-rao/) (Chair)
- [Orlando Timmerman](https://biomin.esc.cam.ac.uk/people/2023-Orlando-Timmerman/)
- Marla Fuchs
- Christian Fernandez Perotti
- Robert Rouse

## Communications
- [Léllé Demertzi](https://www.turing.ac.uk/people/business-team/lelle-demertzi) (Secretary)
- [Cassandra Gould van Praag](https://www.turing.ac.uk/people/researchers/cassandra-gould-van-praag) (Website)
- [Andrew Hyde](https://www.linkedin.com/in/andrew-hyde-b8913957/?originalSubdomain=uk) (Open Access publishing)
- [Andrew McDonald](https://ampersandmcd.com/) (Social media)
- [Ricardo Barros Lourenço](https://about.me/ricardobarroslourenco) 

## Steering Group
- [Claire Monteleoni](https://www.colorado.edu/faculty/claire-monteleoni/)
- [Jakob Runge](https://www.jakob-runge.com)
- [Eniko Szekely](https://www.datascience.ch/people/eniko-szekely)
- Anastase Alexandre Charantonis


<!-- ## Governance
Governance processes for these committees are detailed here <mark>Coming soon: Governance link</mark> -->

<br>





<!-- ### A special thanks to our volunteers!
<p align="justify">
Our call for volunteers to help build a great Open Science Room was met with enthusiasm! We now have multiple teams up and running and we're very excited about what's next. We are so grateful to be part of such an engaging and helpful community. Thank you all!
</p> -->
<!-- <p align="justify">
Together with the OSR team, the wonderfully talented and hard-working volunteers below made significant contributions to the Open Science Room. We have greatly enjoyed working with them, and proud to have them in our community.
Have a look at their contact links and bios below, and give them a virtual high-five in the OSR!
</p> -->
<br>

<!-- <html>

{% assign volunteers = site.volunteers %}

{% assign n_rows = volunteers.size | divided_by:2 %}
<table class="people">
{% for row in (0..n_rows) %}
    <tr class="people">
    {% for col in (0..1) %}
        <td class="people">

        {% assign idx = row | times:2 | plus:col %}
        {% assign person = volunteers[idx] %}
        {% if person %}

            {% assign img_path = nil %}
            {% assign names = person.Name | downcase | split: " " %}
            {% assign img_path = site.baseurl | append: "/img/person_default.jpg" %}
            {% for file in site.static_files %}                
                {% if file.path contains names.first and file.path contains names[1] %}
                    {% assign img_path = file.path %}
                {% endif %}
            {% endfor %}

            <!--<a style="display:block; color:#05323F" href="{{ site.baseurl }}{{person.url}}">-->
            <a style="display:block; color:#05323F">
            <aside class="speaker-card {% if speaker.column %} {{ speaker.column }}{% endif %}">
            <header>
                <img src="{{ site.baseurl }}{{ img_path }}" style="height:200px; border-radius:50%;">

                <h3>{{ person.Name }}</h3>

                <h6>{{ person.Affiliation }}</h6>

                <h4>
                {% if person.Twitter %} <a target="_blank" href="https://twitter.com/{{ person.Twitter }}"><i class="fa fa-twitter fa-2x" style="position: relative; top: 0px;text-indent:0px;  vertical-align: middle; margin-left:4px; margin-right:4px;"></i></a> {% endif %}
                {% if person.Github %} <a target="_blank" href="https://github.com/{{ person.Github }}"><i class="fa fa-github fa-2x" style="position: relative; top: 0px; text-indent:0px; vertical-align: middle; margin-left:4px; margin-right:4px;"></i></a>{% endif %}
                {% if person.Website %} <a target="_blank" href="{{ person.Website }}"><i class="fa fa-external-link-square fa-2x" style="position: relative; top: 0px;text-indent:0px;  vertical-align: middle; margin-left:4px; margin-right:4px;"></i></a>{% endif %}
                </h4>
                <br>
            </header>
            </aside>
            </a>
        {% endif %}
        </td>
    {% endfor %}
    </tr>
{% endfor %}
</table>

</html> -->
