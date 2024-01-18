---
layout: page
title: Team
---

The core organising committee are volunteers and previous contributors to the Climate Informatics Community. 

If you would like to support and engage with the delivery of this meeting, we'd live to hear from you! Please [Contact Us!](../contact)

## Local organising committee
- Chair: [Scott Hosking](https://www.turing.ac.uk/people/researchers/scott-hosking)
- [Alden Conner](https://www.turing.ac.uk/people/business-team/alden-conner)
- Secretary: [Léllé Demertzi](https://www.turing.ac.uk/people/business-team/lelle-demertzi)
- Treasurer: [Katy Thompson](https://www.turing.ac.uk/people/business-team/katy-thompson)
- EDI Champion: [Cassandra Gould van Praag](https://www.turing.ac.uk/people/researchers/cassandra-gould-van-praag)
- ECR Champions: <mark>Coming soon: name and profile link</mark> 
- Reproducibility Champion: <mark>Coming soon: name and profile link</mark> 
- Online Participant Champion: <mark>Coming soon: name and profile link</mark> 

## Programme committee
- Chair: [Douglas Rao](https://ncics.org/people/douglas-rao/)
- Cambridge University Press

## Steering Group
- [Claire Monteleoni](https://www.colorado.edu/faculty/claire-monteleoni/)
- [Jakob Runge](https://www.jakob-runge.com)
- [Eniko Szekely](https://www.datascience.ch/people/eniko-szekely)
- Anastase Alexandre Charantonis <mark>Coming soon: profile link</mark>

## Governance
Governance processes for these committees are detailed here <mark>Coming soon: Governance link</mark>

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
