---
layout: ieeevr-default
title: "Workshop Program"
subtitle: "IEEE VR 2024"
title_separator: "|"
---

<link rel="stylesheet" href="{{ '/assets/css/tableStyles.css' | relative_url }}">

<div>
    <h1 id="call-for-workshop-papers"> Workshops </h1>
    <table class="styled-table">
        <tr>
            <th>Workshops</th>
        </tr>
        {% for workshop in site.data.workshops %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ workshop.id }}">{{ workshop.title }}</a></td>
        </tr>
        {% endfor %}
    </table>

<div>
    {% for workshop in site.data.workshops %}
            <!-- Workshop title matter -->
            <h2 id="{{ workshop.id }}">Workshop: {{ workshop.title }}</h2>
            <!-- <p><strong>{{ workshop.day }}, {{ workshop.starttime }}, {{ workshop.timezone }}</strong></p> -->
            {% if workshop.organiser %}
                <p><small><b style="color: black;">Principal Organiser:</b> {{ workshop.organiser }}</small></p>
            {% endif %}
            {% if workshop.videourl %}
                <div class="video-container">
                    <iframe src="{{workshop.videourl}}" title="YouTube video player" frameborder="0" 
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            {% endif %}
            <p>
            {% if workshop.url %}
                <small><b style="color: black;">Website:</b> <a href="{{ workshop.url }}" target="_blank">{{ workshop.url }}</a></small>
            {% endif %}
            {% if workshop.discordurl %}
                <p><small><b style="color: black;">Discord URL:</b> <a href="{{ workshop.discordurl }}" target="_blank">{{ workshop.discordurl }}</a></small>
            {% endif %}
            {% if workshop.slideurl %}
                <p><small><b style="color: black;">Slides:</b> <a href="{{ workshop.slideurl }}" target="_blank">{{ workshop.slideurl }}</a></small>
            {% endif %}
            </p>
            {% if workshop.abstract %}
                <div id="{{ workshop.id }}" class="wrap-collabsible"> <input id="collapsible{{ workshop.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ workshop.id }}" class="lbl-toggle">Workshop Description</label>
                    <div class="collapsible-content">
                        <div class="content-inner">
                            <p>{{ workshop.abstract }}</p>
                        </div>
                    </div>
                </div>
            {% endif %}
                        
            <!-- Only show the 'workshop papers' toggle if there's actually something to show -->
            {% assign papers_in_session = false %}
            {% for paper in site.data.workshoppapers %}
                {% if workshop.id == paper.workshop %}
                    {% assign papers_in_session = true %}
                {% endif %}
            {% endfor %}
            <!-- Show a hideable list of all papers in this workshop -->
            {% if papers_in_session == true %}
            <div id="{{ workshop.id }}2" class="wrap-collabsible"> <input id="collapsible{{ workshop.id }}2" class="toggle" type="checkbox"> <label for="collapsible{{ workshop.id }}2" class="lbl-toggle">Workshop Papers</label>
                <div class="collapsible-content">
                    <div class="content-inner">
                        {% for paper in site.data.workshoppapers %}
                            {% if workshop.id == paper.workshop %}
                                <h4 id="{{ paper.id }}">{{ paper.title }}</h4>
                                {% if paper.authors %}
                                    <p><i>{{ paper.authors }}</i></p>
                                {% else %}
                                    <p><i>Author information coming soon</i></p>
                                {% endif %}
                                {% if paper.url %}
                                    <p><small>URL: <a href="{{ paper.url }}" target="_blank">{{ paper.url }}</a></small></p>
                                {% endif %}
                                {% if paper.abstract %}
                                    <div id="{{ paper.id }}" class="wrap-collabsible"> <input id="collapsible{{ paper.id }}" class="toggle" type="checkbox"> <label for="collapsible{{ paper.id }}" class="lbl-toggle">Abstract</label>
                                        <div class="collapsible-content">
                                            <div class="content-inner">
                                                <p>{{ paper.abstract }}</p>
                                            </div>
                                        </div>
                                    </div>
                                {% endif %}
                            {% endif %}
                        {% endfor %}
                    </div>
                </div>
            </div>
            {% endif %}
    {% endfor %}
</div>
</div> 
