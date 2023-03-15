---
layout: ieeevr-default
title: "Doctoral Consortium"
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
        font-size: 0.9em;
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

<h1>Doctoral Consortium</h1>
<div>
    <!-- <p>
        Coming Soon.
    </p> -->
    <p>
        All times below are Shanghai, China local time (UTC+8).  The event will be held in a hybrid format, with both in-person and online attendees.  All presenters and mentors are encouraged to attend as much of the doctoral consortium as possible.  However, we understand that our different time zones may make attendance difficult at particular times. If a student and/or mentor are not available to meet during the scheduled mentoring sessions, they should set up a time to meet later that is convenient for them both.
        Each presentation will be an 8 minute talk + 4 minutes for questions.
    </p>
</div>


<div>

<div>
    <table class="styled-table" style="font-size: 0.8em; ">
        <tr>
            <th>Schedule</th>
            <th></th>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">08:45 - 09:00 am</span></td>
            <td>
                Welcome
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">09:00 - 10:00 am</span></td>
            <td>
                <strong>Presentations 1 - 5 (8 min talk + 4 min questions)</strong><br/>
                Shane Burrell Jr – Dr. Victoria Interrante<br/>
                Radhika Jain – Dr. Steven Cutchin<br/>
                Damaruka Priya Rajasagi – Dr. Andrea Stevenson Won<br/>
                Xingyao Yu – Dr. Steven Feiner<br/>
                Xiaoyan Zhou – Dr. Doug Bowman
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">10:00 - 10:30 am</span></td>
            <td>
                Breakout with mentors
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">10:30 - 11:00 am</span></td>
            <td>
                Break
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">11:00 - 12:00 am</span></td>
            <td>
                <strong>Presentations 6-10 (8 min talk + 4 min questions)</strong><br/>
                Klara Brandstätter – Dr. Andrew Robb<br/>
                Ziwen Lu – Dr. Stefanie Zollmann<br/>
                Mathieu Lutfallah – Dr. Tabitha Peck<br/>
                Nels Numan – Dr. Rajiv Khadka<br/>
                Antony Prakash – Dr. Joe Gabbard
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">12:00 - 12:30 pm</span></td>
            <td>
                Breakout with mentors
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">12:30 - 14:00 pm</span></td>
            <td>
                Lunch
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">14:00 - 15:00 pm</span></td>
            <td>
                <strong>Presentations 11-15 (8 min talk + 4 min questions)</strong><br/>
                Amira Mahmoud Shaban Ahmed – Dr. Richard Skarbez<br/>
                Adil Khokhar – Dr. Jason Orlosky<br/>
                Dooyoung Kim – Dr. Evan Suma Rosenberg<br/>
                Nadine Wagener – Dr. Nilufar Baghaei<br/>
                Yue Wang – Dr. Lili Wang
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">15:00 - 15:30 pm</span></td>
            <td>
                Breakout with mentors
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">15:30 - 16:00 pm</span></td>
            <td>
                Break
            </td>
        </tr>
        <tr>
            <td><span style="color: #00aeef;">16:00 - 17:00 pm</span></td>
            <td>
                <strong>Presentations 16-19 (8 min talk + 4 min questions)</strong><br/>
                Zhuang Chang – Dr. Anthony Steed<br/>
                Isla Xi Han – Dr. Yiyu Cai<br/>
                Piaopiao Yu – Dr. Lik-Hang Lee<br/>
                Yidan Zhang – Dr. Mark Billinghurst<br/>
            </td>
        </tr>
        <tr>
            <td ><span style="color: #00aeef;">17:00 - 17:30 pm</span></td>
            <td>
                Breakout with mentors
            </td>
        </tr>
    </table>
</div>
    
    
</div>


<h2>Accepted Students</h2>

<div>
    <table class="styled-table" style="font-size: 0.8em; ">
        <tr>
            <th>Student</th>
            <th>Title</th>
            <th>Affiliation</th>
        </tr>
        {% for student in site.data.dc %}
        <tr>
            <td style="font-size: 0.8em;"><span style="color: #00aeef;">{{ student.author }}</span></td>
            <td>{{ student.title }}</td>
            <td>{{ student.affiliation }}</td>
        </tr>
        {% endfor %}
    </table>
</div> 
