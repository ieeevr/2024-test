---
layout: ieeevr-default
title: "Tutorials"
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
        background-color: #f3f3f3;
    }

    .styled-table tbody tr:last-of-type {
        border-bottom: 2px solid #00aeef;
    }

    .styled-table tbody tr.active-row {
        font-weight: bold;
        color: #00aeef;
    }

</style>


<div>
    <table class="styled-table">

        <tr>
            <th>Tutorials</th>
        </tr>
        {% for tutorial in site.data.tutorials %}
        <tr>
            <td style="font-size: 0.9em;"><a href="#{{ tutorial.id }}">{{ tutorial.title }}</a></td>
            <td style="font-size: 0.9em;">{{ tutorial.day }}</td>
            <td style="font-size: 0.9em;">{{ tutorial.starttime }}-{{ tutorial.endtime }},{{ tutorial.timezone }} </td>
        </tr>
        {% endfor %}
    </table>
</div>

{% for tutorial in site.data.tutorials %}
{% if tutorial.id == 'T1' %}
<div>
<h2 id="{{ tutorial.id }}">{{ tutorial.name }}: {{ tutorial.title}}</h2>

<!-- TAKE ME TO THE EVENT START
{% for event in site.data.events %}
{% if event.id == 'T5' %}
{% if event.location %}
<div class="notice--info">
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
        {% endif %}
    </p>
</div>
{% endif %}
{% endfor %}
    TAKE ME TO THE EVENT END-->

<p>
    {{ tutorial.day }}, {{ tutorial.starttime }}-{{ tutorial.endtime }}, {{ tutorial.timezone }}, {{ tutorial.room }}
</p>

<p>
    <strong>Organizers</strong>
</p>
<p>
    Jerald Thomas, Virginia Tech<br/> 
    Evan Suma Rosenberg, University of Minnesota<br/> 
    Tabitha Peck, Davidson College<br/>
</p>
<!-- <p>
    <strong style="font-size: 0.8em;color: black"> {{ tutorial.schedule1 }}, {{ tutorial.timezone1 }}</strong>
</p> -->

<h3>About this Tutorial</h3>
<p>
    Several researchers in our field are expressing concern regarding the increased amount of paper reviews they are asked to provide. This is backed up by the <a href="https://clarivate.com/lp/global-state-of-peer-review-report/">2018 Publons Global State of Peer Review (GSPR) report</a>, which shows that the number of requested reviews is outpacing the available reviewers while reviewer fatigue is on the rise. A critical finding was the need for formal training so that newer researchers can enter the peer-reviewer pool earlier and more confidently. This responsibility is often pushed onto students’ advisors, but only 16.1% of the GSRP survey respondents were asked by their supervisor or PI to write a review with them or on their behalf. Furthermore, 39.4% of respondents had never had formal peer-review training. 88% of respondents believe that formal peer-reviewer training is either important or very important for producing high-quality reviews, and 80% respond that formal peer-reviewer training would have either a positive or extremely positive outcome on the peer-review system. It is clear that the research community at large believes that more peer-review training is important, and this tutorial is an attempt to provide it, in part, to this research community.
</p>
<h3>Intended Audience</h3>
<p>
    There will be no technical aspect of the tutorial, so there is no required technical level for participants. The intended audience is persons relatively new to research who will likely find themselves participating in the peer-review process. Specifically, the content will be targeted at junior researchers, including Ph.D. students, but everyone should find something useful in the content.
</p>
<h3>Expected Value for the Audience</h3>
<p>
    The expected value for the audience is twofold. First, participants will have a greater understanding of the peer-review process and how to construct a quality review. With this knowledge, they should be able to enter the peer-reviewer pool earlier than they would otherwise, increasing their visibility to our community. Second, as we increase the size of the peer-reviewer pool, participants will hopefully see a more manageable number of review requests in the future, reducing the chances of reviewer fatigue.
</p>
<h3>Topics Outline</h3>
<p>
The tutorial will be broken into three, one-hour-long sections. First, there will be an introduction and an instructional presentation. The second hour will consist of hands-on and interactive activities aimed at helping participants understand the core components of quality reviews. Finally, we will conclude the tutorial with a panel made up of senior researchers in the field, of whom participants will get the opportunity to ask questions regarding the review process.
</p>
<p>
    Specific topics covered by this tutorial include:
</p>
<ul>
    <li>The purpose of the peer-review process</li>
    <li>The goal of a paper review</li>
    <li>A description of how the peer-review process works in our field, including the more “behind the scenes” aspects</li>
    <li>Components of a good review and signs of a bad review</li>
    <li>Example processes for writing reviews</li>
    <li>Additional tips, tricks, and things to remember</li>
    <li>Discussion and Q&A</li>
</ul>
</div>
{% else %}

<div>
<h2 id="{{ tutorial.id }}">{{ tutorial.name }}: {{ tutorial.title}}</h2>
<p>
    {{ tutorial.day }}, {{ tutorial.starttime }}-{{ tutorial.endtime }}, {{ tutorial.timezone }}, {{ tutorial.room }}
</p>
<p>
    <strong>Organizers</strong>
</p>
<p>
    {% assign authornames = tutorial.authorsfull | split: ";" %}
    {% for name in authornames %}
    {{ name | strip }} <br />
    {% endfor %}
</p>
<h3>Summary</h3>
    {% assign sum = tutorial.summary | split: ";" %}
    {% for para in sum %}
    <p>
    {{ para }} 
    </p>
    {% endfor %}


{% assign techl = tutorial.techlevel | split: ";" %}
{% if tutorial.techlevel %}
<h3>Technical Level</h3>
{% for parat in techl %}
<p>
{{ parat }} 
</p>
{% endfor %}
{% endif %}

{% assign aud= tutorial.audience | split: ";" %}
{% if tutorial.audience %}
<h3>Intended Audience</h3>
{% for paraa in aud %}
<p>
{{ paraa }} 
</p>
{% endfor %}
{% endif %}


{% assign v= tutorial.value | split: ";" %}
{% if tutorial.value %}
<h3>Value</h3>
{% for parav in v %}
<p>
{{ parav }} 
</p>
{% endfor %}
{% endif %}

</div>
{% endif %}
{% endfor %}