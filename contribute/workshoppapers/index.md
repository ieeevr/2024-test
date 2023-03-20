---
layout: ieeevr-default
title: "Workshop Papers"
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
</div> 
