---
layout: ieeevr-default
title: "Research Demos"
subtitle: "IEEE VR 2024"
title_separator: "|"
---

<div>
    <table class="styled-table">
        <tr>
            <th>Research Demos</th>
        </tr>
        {% assign i = 0 %}
        {% for demo in site.data.demos %}
            {% assign i = i | plus:1 %}
            <tr>
                <td style="font-size: 0.9em;"><a href="#{{ demo.id }}">{{ demo.title }}</a></td>
            </tr>
        {% endfor %}
    </table>
</div>
<p>
    <table class="program-table">
        <thead>
            <tr>
                <th colspan="4">Research&nbsp;Demos&nbsp;Schedule </th>
            </tr>
        </thead>
        <tbody> 
             <tr>
                <td>Research&nbsp;Demo&nbsp;Booths&nbsp;Open</td>
                <td>Monday,&nbsp;18&nbsp;March</td>                
                <td>9:45&#8209;10:00, 13:00&#8209;13:30, 15:00&#8209;15:30, 17:00&#8209;19:00</td>       
                <td>Sorcerer's&nbsp;Apprentice Ballroom</td>  
            </tr>            
             <tr>
                <td>Research&nbsp;Demo&nbsp;Booths&nbsp;Open</td>
                <td>Tuesday,&nbsp;19&nbsp;March</td>                
                <td>9:45&#8209;10:00, 13:00&#8209;13:30, 15:00&#8209;15:30, 17:00&#8209;17:30</td>       
                <td>Sorcerer's&nbsp;Apprentice Ballroom</td>  
            </tr>
            <tr>
                <td>Research&nbsp;Demo&nbsp;Booths&nbsp;Open</td>
                <td>Wednesday,&nbsp;20&nbsp;March</td>                
                <td>9:45&#8209;10:00, 13:00&#8209;13:30, 15:00&#8209;15:30, 17:00&#8209;17:30</td>       
                <td>Sorcerer's&nbsp;Apprentice Ballroom</td>  
            </tr>
            <tr>
                <td>Awards</td>
                <td>Thursday,&nbsp;21&nbsp;March</td>                
                <td>15:30&#8209;17:00</td>       
                <td>Fantasia Ballroom&nbsp;H</td>  
            </tr>
        </tbody>
    </table>
</p>
<h2>Entries</h2>
<div>
    {% assign j = 0 %}
    {% for demo in site.data.demos %}
        {% assign j = j | plus:1 %}
        <p id="{{ demo.id }}"><strong>{{ demo.title }}</strong><br/></p>
        <div style="margin-left: 35px;">
            <p>
                {% assign authornames = demo.authors | split: ";" %}
                <i>
                    {% for name in authornames %}
                        {% if name == authornames.last %}
                            {{ name | strip }}                             
                        {% else %}
                            {{ name | strip }}, 
                        {% endif %}
                    {% endfor %}
                </i>
            </p>
            <p><strong style="color: black;"> Room: {{ demo.hall }} </strong> <br> </p> 
            {% if demo.abstract %}
                <div id="{{ demo.id }}" class="wrap-collabsible"> <input id="collapsible{{ demo.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ demo.id }}" class="lbl-toggle">Abstract</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ demo.abstract }}</p>
                        </div>
                    </div>
                </div>
            {% endif %}
            {% if demo.url-embed %}
                <div class="video-container">
                    <iframe src="https://www.youtube.com/embed/{{ demo.url-embed }}" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            {% else %}
                {% if demo.url %}
                    <p>Teaser Video: <a href="{{ demo.url }}" target="_blank">Watch Now</a></p>
                {% endif %}
            {% endif %}
        </div>
        {% if j == i %}
        {% else %}
            <hr style="margin: 25px 0 25px 0;">
        {% endif %}
    {% endfor %}
</div>


