---
layout: ieeevr-default
title: "Workshop Program"
subtitle: "IEEE VR 2023"
title_separator: "|"
---

<style>
    .styled-table {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.8em;
        font-family: sans-serif;
        /*min-width: 400px;*/
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
        display: table;
    }

    .styled-table thead tr {
        background-color: #00aeef;
        color: #ffffff;
        text-align: left;
    }

    .styled-table th,
    .styled-table td {
        padding: 12px 15px;
    }

    .styled-table tbody tr {
        border-bottom: 1px solid #dddddd;
    }

    .styled-table tbody tr:nth-of-type(even) {
        background-color: #fffbed;
    }

    .styled-table tbody tr:last-of-type {
        border-bottom: 2px solid #F5725E;
    }

    .styled-table tbody tr.active-row {
        font-weight: bold;
        color: #F5725E;
    }

    input[type='checkbox'] {
        display: none;
    }

    .wrap-collabsible {
        margin: 1rem 0;
    }

    .lbl-toggle {
        display: block;
        font-weight: bold;
        /* font-family: monospace; */
        font-size: 0.8rem;
        text-align: left;
        padding: 0rem;
        color: #fec10d;
        background: #ffffff;
        cursor: pointer;
        border-radius: 7px;
        transition: all 0.25s ease-out;
    }

    .lbl-toggle:hover {
        /*color: #FFF;*/
    }

    .lbl-toggle::before {
        content: ' ';
        display: inline-block;
        border-top: 5px solid transparent;
        border-bottom: 5px solid transparent;
        border-left: 5px solid currentColor;
        vertical-align: middle;
        margin-right: .7rem;
        transform: translateY(-2px);
        transition: transform .2s ease-out;
    }

    .toggle:checked+.lbl-toggle::before {
        transform: rotate(90deg) translateX(-3px);
    }

    .collapsible-content {
        max-height: 0px;
        overflow: hidden;
        transition: max-height .25s ease-in-out;
    }

    .toggle:checked+.lbl-toggle+.collapsible-content {
        max-height: 1500px;
    }

    .toggle:checked+.lbl-toggle {
        border-bottom-right-radius: 0;
        border-bottom-left-radius: 0;
    }

    .collapsible-content .content-inner {
        background: white;
        /* rgba(0, 105, 255, .2);*/
        border-bottom: 1px solid white;
        border-bottom-left-radius: 7px;
        border-bottom-right-radius: 7px;
        padding: .5rem 1rem;
    }

    .collapsible-content p {
        margin-bottom: 0;
    }

    .video-container {
        overflow: hidden;
        position: relative;
        width: 100%;
    }

    .video-container::after {
        padding-top: 56.25%;
        /* 75% if 4:3*/
        display: block;
        content: '';
    }

    .video-container iframe {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
    }
</style>

<!-- <div>
    <p>
        More information coming soon, please watch this space.
    </p>
</div> -->

<div>
    <h1 id="call-for-workshop-papers"> Workshops </h1>
    <p>
        IEEE VR 2023 seeks high-quality contributions to the following 18 workshops. 
        <!-- These will be held virtually on March 12<sup>th</sup>-13<sup>th</sup>.  -->
        For more details, see each workshop's Call for Papers below.
    </p>
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
                <p><small><b style="color: black;">Slides:</b> <a href="{{ workshop.discordurl }}" target="_blank">{{ workshop.slideurl }}</a></small>
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
            <!-- TAKE ME TO THE EVENT START -->
            <!--{% for event in site.data.events %}
                {% if event.id == workshop.id %}
                    {% if event.location %}
                    <div class="notice--info" style="background-color: $theme-yellow ! important; color: $theme-text ! important;">
                        <strong style="padding-bottom: 5px;">Take me to the event:</strong>
                        <p>
                            <strong style="color: black;">Virbela Location:</strong> {{ event.location }} (<a href="/2021/attend/virbela-instructions/#map">MAP</a>)
                            {% if event.stream-url %}
                                <br />
                                {% if event.aindanaoaconteceu %}
                                    <strong style="color: black;">Watch video stream live:</strong> <a href="{{ event.stream-url }}" target="_blank">HERE</a>
                                {% else %}
                                    <strong style="color: black;">Watch the recorded video stream:</strong> <a href="{{ event.stream-url }}" target="_blank">HERE</a>
                                {% endif %}
                            {% endif %}
                            {% if event.discordurl %}
                                <br />
                                <strong style="color: black;">Discord Channel:</strong> <a href="https://{{ event.discordurl }}" target="_blank">Open in Browser</a>, <a href="discord://{{ event.discordurl }}">Open in App</a> (Participants only)
                            {% endif %}
                        </p>
                    </div>
                    {% endif %}
                {% endif %}
            {% endfor %}-->
            <!-- TAKE ME TO THE EVENT END-->
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