---
layout: ieeevr-default
title: "Program Overview"
---

<style>
    .styled-table {
        border-collapse: collapse;
        margin: 25px 0;
        font-size: 0.9em;
        font-family: sans-serif;
        /*min-width: 400px;*/
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
        display: table;
    }

    .styled-table thead tr {
        background-color: #F5725E;
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
        border-bottom: 2px solid #F5725E;
    }

    .styled-table tbody tr.active-row {
        font-weight: bold;
        color: #F5725E;
    }


    /*************************
 * GRID SCHEDULE LAYOUT from there: https://css-tricks.com/building-a-conference-schedule-with-css-grid/
 *************************/
    @media screen and (min-width:700px) {
        .schedule {
            display: grid;
            grid-gap: 1em;
            grid-template-rows:
                [tracks] auto [time-0830] 0.5fr [time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr [time-1030] 0.5fr [time-1100] 0.5fr [time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr [time-1730] 0.5fr [time-1800] 0.5fr [time-1830] 0.5fr [time-1900] 0.5fr;
            /* Note 1:
      Use 24hr time for gridline names for simplicity

      Note 2: Use "auto" instead of "0.5fr" for a more compact schedule where height of a slot is not proportional to the session length. Implementing a "compact" shortcode attribute might make sense for this!
      Try 0.5fr for more compact equal rows. I don't quite understand how that works :)
      */

            grid-template-columns:
                [times] 4em [track-1-start] 0.5fr [track-1-end track-2-start] 0.5fr [track-2-end track-3-start] 0.5fr [track-3-end];
        }

        .schedule-sat-25 {
            display: grid;
            grid-gap: 0.3em;
            grid-template-rows:
                [tracks] auto [time-0800] 0.25fr [time-0815] 0.25fr [time-0830] 0.5fr [time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr[time-1030] 0.5fr [time-1100] 0.5fr[time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr [time-1730] 0.5fr [time-1800] 0.5fr [time-1830] 0.5fr;

            grid-template-columns:
                [times] 3em [track-1-start] 0.1fr[track-1-end track-2-start] 0.1fr[track-2-end track-3-start] 0.1fr[track-3-end track-4-start] 0.1fr
                [track-4-end track-5-start] 0.1fr[track-5-end track-6-start] 0.1fr
                [track-6-end track-7-start] 0.1fr[track-7-end track-8-start] 0.1fr
                [track-8-end];
        }

        .schedule-sun-26 {
            display: grid;
            grid-gap: 0.4em;
            grid-template-rows:
                [tracks] auto [time-0800] 0.25fr [time-0815] 0.25fr[time-0830] 0.5fr[time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.5fr [time-1030] 0.5fr [time-1100] 0.5fr [time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.5fr [time-1530] 0.5fr [time-1600] 0.5fr [time-1630] 0.5fr [time-1700] 0.5fr [time-1730] 0.5fr [time-1800] 0.5fr [time-1830] 0.5fr [time-1900] 0.5fr [time-1930] 0.5fr [time-2000] 0.5fr [time-2030] 0.5fr [time-2100] 0.5fr [time-2130] ;

            grid-template-columns:
                [times] 3em [track-1-start] 0.2fr [track-1-end track-2-start] 0.2fr [track-2-end track-3-start] 0.2fr [track-3-end track-4-start] 0.2fr
                [track-4-end track-5-start] 0.2fr [track-5-end track-6-start] 0.2fr 
                [track-6-end track-7-start] 0.2fr [track-7-end];
        }

        .schedule-mon-27 {
            display: grid;
            grid-gap: 0.3em;
            grid-template-rows:
                [tracks] auto [time-0800] auto[time-0830] 0.5fr[time-0900] 0.5fr [time-0930] 0.5fr [time-1000] 0.25fr [time-1015] 0.25fr [time-1030] 0.5fr [time-1100] 0.25fr [time-1115] auto [time-1130] auto [time-1145] 0.25fr [time-1200] 0.5fr [time-1230] 0.5fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.25fr [time-1445] 0.25fr [time-1500] 0.5fr [time-1530] 0.25fr [time-1545] 0.25fr [time-1600] 0.5fr [time-1630] 0.25fr  [time-1645] 0.25fr [time-1700] auto [time-1730] auto [time-1800] 0.5fr [time-1830] 0.25fr[time-1900] 0.25fr [time-1930] 0.25fr [time-2000] 0.25fr [time-2030] 0.25fr [time-2100] 0.25fr  [time-2200] ;

            grid-template-columns:
                [times] 3em [track-1-start]20% [track-1-end track-2-start]20% [track-2-end track-3-start]20% [track-3-end track-4-start]20%
                [track-4-end track-5-start]10%;
                /* 13% [track-5-end track-6-start]13% 
                [track-6-end track-7-start]13% [track-7-end]; */
        }

        .schedule-tue-28 {
            display: grid;
            grid-gap: 0.3em;
            grid-template-rows:
                [tracks] auto [time-0800] auto [time-0815] auto[time-0830] 0.5fr[time-0900] auto [time-0930] 0.5fr [time-1000] auto [time-1015] 0.25fr [time-1030] auto [time-1045] auto [time-1100] 0.25fr [time-1115] 0.25fr [time-1130] auto [time-1145] 0.25fr [time-1200] auto [time-1230] auto 
                [time-1245] 0.25fr [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] auto [time-1430] auto[time-1445] auto [time-1500] 0.25fr [time-1515] 0.25fr [time-1530] 0.25fr[time-1545] auto [time-1600] auto [time-1615] 0.25fr [time-1630] 0.25fr  [time-1645] 0.25fr [time-1700] 0.25fr [time-1730] 0.25fr [time-1800] auto [time-1830] auto [time-1900] auto [time-1930] auto[time-2000] auto [time-2030] auto [time-2100] auto [time-2130] ;

            grid-template-columns:
                [times] 3em [track-1-start]20% [track-1-end track-2-start]20% [track-2-end track-3-start]20% [track-3-end track-4-start]20%
                [track-4-end track-5-start]10%;
                /* 13% [track-5-end track-6-start]13% 
                [track-6-end track-7-start]13% [track-7-end]; */
        }

        .schedule-wed-29 {
            display: grid;
            grid-gap: 0.3em;
            grid-template-rows:
                [tracks] auto [time-0800] 0.25fr [time-0815] 0.25fr [time-0830] 0.5fr [time-0900] 0.5fr [time-0930] 0.25fr [time-0945] 0.25fr [time-1000] 0.5fr[time-1030] 0.25fr [time-1045] 0.25fr [time-1100] 0.5fr[time-1130] 0.5fr [time-1200] 0.5fr [time-1230] 0.25fr 
                [time-1245] 0.25fr
                [time-1300] 0.5fr [time-1330] 0.5fr [time-1400] 0.5fr [time-1430] 0.5fr [time-1500] 0.25fr [time-1515] 0.25fr [time-1530] 0.5fr [time-1600] 0.25fr [time-1615] 0.25fr [time-1630] 0.5fr [time-1700] 0.5fr [time-1730] 0.5fr [time-1800] 0.5fr [time-1830] 0.5fr;

            grid-template-columns:
                [times] 3em [track-1-start] 20% [track-1-end track-2-start]20%[track-2-end track-3-start]20%[track-3-end track-4-start]20%
                [track-4-end track-5-start]10%;
        }
    }

    .time-slot {
        grid-column: times;
        text-decoration: none;

    }

    .track-slot {
        display: none;
        /* hidden on small screens and browsers without grid support */
    }

    @supports(display:grid) {
        @media screen and (min-width:700px) {
            .track-slot {
                display: block;
                padding: 10px 5px 5px;
                position: sticky;
                top: 0;
                z-index: 1000;
                background-color: rgba(255, 255, 255, .9);
            }
        }
    }

    /* Small-screen & fallback styles */
    .session {
        margin-bottom: 1em;
    }

    @supports(display:grid) {
        @media screen and (min-width: 700px) {
            .session {
                margin: 0;
            }
        }
    }

    /*************************
 * VISUAL STYLES
 * Design-y stuff ot particularly important to the demo
 ************************
    body {
        padding: 50px;
        max-width: 1100px;
        margin: 0 auto;
        line-height: 1.5;
    }
    */

    .session {
        padding: .5em;
        border-radius: 5px;
        font-size: 12px;
        box-shadow:
            rgba(255, 255, 255, .6) 1px 1px 0,
            rgba(0, 0, 0, .3) 4px 4px 0;
    }

    .session-title,
    .session-time,
    .session-track,
    .session-presenter {
        display: block;
    }

    .session-title,
    .time-slot {
        margin: 0;
        font-size: 1em;
    }

    .session-title a {
        color: #fff;
        text-decoration-style: dotted;

        &:hover {
            font-style: italic;
        }

        &:focus {
            outline: 2px dotted rgba(255, 255, 255, .8);
        }
    }

    .track-slot,
    .time-slot {
        font-weight: bold;
        font-size: .8em;
    }

    .track-1 {
        background-color: #F5725E;
        color: #fff;
    }

    .track-2 {
        background-color: #009cb4;
        color: #fff;
    }

    .track-3 {
        background-color: rgb(52, 199, 89);
        color: #fff;
    }

    .track-poster {
        background-color: #c65833;
        color: #fff;
    }

    .track-4 {
        background-color: #fec10d;
        color: #fff;
    }
    
    .track-5 {
        background-color: #53c5ca;
        color: #fff;
    }

    .track-all {
        display: flex;
        justify-content: center;
        align-items: center;
        background: #ccc;
        color: #000;
        box-shadow: none;
    }

    .track-teal {
        background-color: #00aeef;
        color: #fff;
    }

    .track-break {
        background-color: #ddf6ff;
        color: #464646;
    }

    .track-green {
        background-color: rgb(52, 199, 89);
        color: #fff;
    }

    .track-orange {
        background-color: rgb(255, 149, 0);
        color: #fff;
    }

    .track-lunch {
        background-color: #ddf6ff;
        color: #464646;
    }
    /* .track-poster {
    background-color: rgb(255, 230, 153);
    color: #fff;
    } */

    .track-purple {
        background-color: rgb(175, 82, 222);
        color: #fff;
    }

    .track-event {
        background-color: rgb(90, 200, 250);
        color: #fff;
    }

    .track-panel {
        background-color: #fec10d;
        color: #fff;
    }

    .track-keynote {
        /* background-color: rgb(196, 136, 195); */
        background-color: rgb(211, 15, 69);
        color: #fff;
    }

    .track-3dui {
        /* background-color: rgb(88, 86, 214); */
        background-color: rgb(196, 136, 195);
        color: #fff;
    }

    .text {
        max-width: 750px;
        font-size: 18px;
        margin: 0 auto 50px;
    }

    .meta {
        color: #555;
        font-style: italic;
    }

    .meta a {
        color: #555;
    }

    hr {
        margin: 40px 0;
    }


    /* Collapsible */
    input[type='checkbox'] {
        display: none;
    }

    .wrap-collabsible {
        margin: 1.2rem 0;
    }

    .lbl-toggle {
        display: block;
        font-weight: bold;
        /* font-family: monospace; */
        font-size: 1rem;
        text-align: left;
        padding: 0.5rem;
        color: #ffffff;
        background: #F5725E;
        cursor: pointer;
        border-radius: 7px;
        transition: all 0.25s ease-out;
    }

    .lbl-toggle:hover {
        color: #FFF;
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
        border-bottom: 1px solid rgba(0, 105, 255, .45);
        border-bottom-left-radius: 7px;
        border-bottom-right-radius: 7px;
        padding: .5rem 1rem;
    }

    .collapsible-content p {
        margin-bottom: 0;
    }

</style>


<h1>Program Overview</h1>

<a href="http://ieeevr.org/2023/assets/attend/Tentative_Program_VR2023.pdf" class="btn btn--info" style="" target="_blank">Tentative Program</a> 



<div style="text-align:center;">
        <small><span style="color:gray;">Conference local time</span></small>
        <iframe src="https://www.zeitverschiebung.net/clock-widget-iframe-v2?language=en&size=small&timezone=Asia%2FShanghai" width="100%" height="140" frameborder="0" seamless></iframe>
        <!-- <iframe src="https://www.zeitverschiebung.net/clock-widget-iframe-v2?language=en&size=small&timezone=Europe%2FLisbon&show=hour_minute" width="100%" height="140" frameborder="0" seamless></iframe> -->
</div>

<!-- <div style="">
    <p style="font-size: 20px;">
        Tentative Program
    </p>
    <img src="../../assets/images/program/Tentative_Program_Page1.png" alt="tentative program page 1" style="width: 90%"/>
    <img src="../../assets/images/program/Tentative_Program_Page2.png" alt="tentative program page 2" style="width: 90%"/>
</div> -->

<div class="notic--warning">
<h3 style="color: rgb(255, 45, 85);">Please note that all times are given in Shanghai, China local time (UTC+8).</h3>
</div>

<!-- <div class="notice--info" style="background-color: $theme-yellow ! important; color: $theme-text ! important;">
    <strong>Locations</strong>
    <p>
        Locations in the program below refer to virtual places in the Virbela platform.
    </p>
    <center>
        <p style="font-size: 20px;">
            <a href="/2021/attend/virbela-instructions/" class="btn btn--primary" style="color: white;">Getting Started with Virbela</a>
        </p>
    </center>
</div> -->
<!--
<div class="notice--warning">
    <strong>Note:</strong>
    <p>
        The indications for locations in this program refer to virtual locations in the Virbela platform. Please find more information about and how to use Virbela <a href="/2021/attend/virbela-instructions/">here</a>.
    </p>
</div>
-->



<div>
    <div class="wrap-collabsible"> <input id="collapsible1" class="toggle" type="checkbox" checked> <label for="collapsible1" class="lbl-toggle">Saturday, March 25</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Shanghai, China, UTC+8</strong></center>
                <div class="schedule-sat-25" aria-labelledby="schedule-heading">
                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-6; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-7; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-8; grid-row: tracks;"></span>
                    <p class="time-slot" style="grid-row: time-0800;">8:00</p>
                    <div class="session session-1 track-teal" style="grid-column: track-7-start / track-7-end; grid-row: time-0800 / time-1130;">
                        <h3 class="session-title"><a href="/2023/program/tutorials/#T5">Tutorial [online]: Demystifying Academic Paper Reviews: How to Construct Quality Reviews for Peer-Reviewed Publications</a></h3>
                        <span class="session-time">8:00 - 11:30</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2023/attend/virbela-instructions/#map">Auditorium A</a></span> -->
                    </div>
                    <p class="time-slot" style="grid-row: time-0815;">08:15</p>
                    <div class="session session-2 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-0815 / time-1330;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#VR4Exergame">Workshop [online]: First Workshop on VR for Exergaming (VR4Exergame)</a></h3>
                        <span class="session-time">8:15 - 13:30</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span> -->
                    </div>
                    <p class="time-slot" style="grid-row: time-0830;">08:30</p>
                    <div class="session session-3 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-1300;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#MASSXR">Workshop [online]: Multi-modal Affective and Social Behavior Analysis and Synthesis in Extended Reality (MASSXR)</a></h3>
                        <span class="session-time">8:30 - 13:10</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span> -->
                    </div>
                    <div class="session session-4 track-green" style="grid-column: track-4-start / track-4-end; grid-row: time-0830 / time-1130;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#TrainingXR">Workshop [online]: 4th Annual Workshop on 3D Content Creation for Simulated Training in eXtended Reality (TrainingXR)</a></h3>
                        <span class="session-time">8:30 - 11:30</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span> -->
                    </div>
                    <div class="session session-5 track-green" style="grid-column: track-6-start / track-6-end; grid-row: time-0830 / time-1830;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#XRIOS">Workshop [online]: 2nd International Workshop on eXtended Reality for Industrial and Occupational Support (XRIOS)</a></h3>
                        <span class="session-time">8:30 - 18:30</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span> -->
                    </div>
                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>
                    <div class="session session-6 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-0830 / time-1130;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#KELVAR">Workshop [online]: KELVAR Workshop: K-12+ Embodied Learning through Virtual and Augmented Reality</a></h3>
                        <span class="session-time">8:30 - 11:30</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span> -->
                    </div>
                    <div class="session session-7 track-green" style="grid-column: track-5-start / track-5-end; grid-row: time-0830 / time-1630;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#ENPT-XR">Workshop [online]: Workshop on Emerging Novel Prototyping Techniques for XR (ENPT XR)</a></h3>
                        <span class="session-time">8:30 - 16:30</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span> -->
                    </div>
                    <div class="session session-8 track-orange" style="grid-column: track-8-start / track-8-end; grid-row: time-0900 / time-1230;">
                        <h3 class="session-title"><a href="/2023/program/doctoral-consortium/">Doctoral Consortium</a></h3>
                        <span class="session-time">9:00 - 12:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>
                    <p class="time-slot" style="grid-row: time-1130;">11:30</p>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>
                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <div class="session session-9 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#XRHealth">Workshop [online]: 2nd XR Health workshop - XR Technologies for Healthcare and Wellbeing (XR Health)</a></h3>
                        <span class="session-time">14:00 - 17:00</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span> -->
                    </div>
                    <div class="session session-10 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#ReDigiTS">Workshop [hybrid]: 3D Reconstruction| Digital Twinning| and Simulation for Virtual Experiences (ReDigiTS)</a></h3>
                        <span class="session-time">14:00 - 17:00</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span> -->
                    </div>
                    <div class="session session-11 track-orange" style="grid-column: track-8-start / track-8-end; grid-row: time-1400 / time-1730;">
                        <h3 class="session-title"><a href="/2023/program/doctoral-consortium/">Doctoral Consortium</a></h3>
                        <span class="session-time">14:00 - 17:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <div class="session session-12 track-teal" style="grid-column: track-7-start / track-7-end; grid-row: time-1700 / time-1830;">
                        <h3 class="session-title">
                            <a href="/2023/program/tutorials/#T2">
                                Tutorial [online]: Introduction to Building Social Virtual Reality with Ubiq
                            </a>
                        </h3>
                        <span class="session-time">17:00 - 18:30</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span> -->
                    </div>
                    <p class="time-slot" style="grid-row: time-1730;">17:30</p>
                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <p class="time-slot" style="grid-row: time-1830;">18:30</p>
                </div>
            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible2" class="toggle" type="checkbox" checked> <label for="collapsible2" class="lbl-toggle">Sunday, March 26</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Shanghai, China, UTC+8</strong></center>
                <div class="schedule-sun-26" aria-labelledby="schedule-heading">
                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-6; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-7; grid-row: tracks;"></span>
                    <p class="time-slot" style="grid-row: time-0800;">8:00</p>
                    <div class="session session-1 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-0800 / time-1330;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#WIVL">Workshop [online]: Workshop on Immersive Visualization Laboratories - Past Present and Future</a></h3>
                        <span class="session-time">8:00 - 13:40</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span> -->
                    </div>
                    <div class="session session-2 track-green" style="grid-column: track-4-start / track-4-end; grid-row: time-0815 / time-1400;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#SecImmeWorld"> Workshop [online]: First Workshop on Security and Privacy for Immersive Virtual Worlds (Secure Immersive Worlds)</a></h3>
                        <span class="session-time">8:15 - 14:00</span>
                        <!-- <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span> -->
                    </div>
                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>
                    <div class="session session-3 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#Data4XR">Workshop [hybrid]: Data4XR: Datasets for Developing Intelligent XR Applications</a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>
                    <div class="session session-4 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#MixReal">Workshop [hybrid]: Mixing Realities: Cross-reality Visualization| Interaction| and Collaboration </a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>
                    <div class="session session-5 track-green" style="grid-column: track-5-start / track-5-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#EUCHS">Workshop [online]: Enhancing User Comfort| Health| and Safety in VR and AR</a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>
                    <div class="session session-6 track-green" style="grid-column: track-6-start / track-6-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#WISP">Workshop [online]: Workshop on Immersive Sickness Prevention (WISP)</a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                    </div>
                    <div class="session session-7 track-teal" style="grid-column: track-7-start / track-7-end; grid-row: time-0900 / time-1030;">
                        <h3 class="session-title"><a href="/2023/program/tutorials/#T4">Tutorial [hybrid]: Introduction to Building Digital human with 3D and 4D Face Capture</a></h3>
                        <span class="session-time">9:00 - 10:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>
                    <div class="session session-8 track-teal" style="grid-column: track-7-start / track-7-end; grid-row: time-1100 / time-1230;">
                        <h3 class="session-title"><a href="/2023/program/tutorials/#T1">Tutorial [hybrid]: Towards Building Automated Non-Rigid Spatially Augmented Reality</a></h3>
                        <span class="session-time">11:00 - 12:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>
                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <div class="session session-9 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1630;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#ANIVAE-2023">Workshop [hybrid]: 6th IEEE VR Internal Workshop on Animation in Virtual and Augmented Environments (ANIVAE-2023)</a></h3>
                        <span class="session-time">14:00 - 16:30</span>
                    </div>
                    <div class="session session-10 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1600;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#I-Meta">Workshop [hybrid]:  Industrial Metaverse (I-Meta) </a></h3>
                        <span class="session-time">14:00 - 16:00</span>
                    </div>
                    <div class="session session-11 track-green" style="grid-column: track-5-start / track-5-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#ARES">Workshop [online]: ARES - Augmented Reality Enabling Superhuman Sports + Serious Games (2nd Annual Workshop)</a></h3>
                        <span class="session-time">14:00 - 17:00</span>
                    </div>
                    <div class="session session-12 track-green" style="grid-column: track-6-start / track-6-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title"><a href="/2023/contribute/workshoppapers/#OAT"> Workshop [online]: Open Access Tools and libraries for virtual reality (OAT)</a></h3>
                        <span class="session-time">14:00 - 17:00</span>
                    </div>
                    <div class="session session-13 track-teal" style="grid-column: track-7-start / track-7-end; grid-row: time-1400 / time-1730;">
                        <h3 class="session-title"><a href="/2023/program/tutorials/#T3"> Tutorial [hybrid]: Introduction of building XR environments using Omniverse</a></h3>
                        <span class="session-time">14:00 - 17:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <p class="time-slot" style="grid-row: time-1900;">19:00</p>
                    <div class="session session-14 track-5" style="grid-column: track-1-start / track-7-end; grid-row: time-1900 / time-2030;">
                        <h3 class="session-title"> Paper fast forward</h3>
                        <span class="session-time">19:00 - 20:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-2000;">20:00</p>
                    <p class="time-slot" style="grid-row: time-2100;">21:00</p>
                </div>
            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible3" class="toggle" type="checkbox" checked> <label for="collapsible3" class="lbl-toggle">Monday, March 27</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Shanghai, China, UTC+8</strong></center>
                <div class="schedule-mon-27" aria-labelledby="schedule-heading">
                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <p class="time-slot" style="grid-row: time-0830;">8:30</p>
                    <div class="session session-1 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0900;">
                        <h3 class="session-title">Opening</h3>
                        <span class="session-time">8:30 - 9:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>
                    <div class="session session-3 track-keynote" style="grid-column: track-1-start / track-1-end; grid-row: time-0900 / time-1000;">
                        <h3 class="session-title"><a href="/2023/program/keynote-speakers/#keynote-guo"> Keynote1</a></h3>
                        <span class="session-time">9:00 - 10:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>
                    <div class="session session-3 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1000 / time-1015;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">10:00 - 10:15</span>
                    </div>
                    <div class="session session-3 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-1015 / time-1115;">
                    <h3 class="session-title"><a href="/2023/program/papers/#5"> Paper Session1 Rendering</a></h3>
                        <span class="session-time">10:15 - 11:15</span>
                    </div>
                    <div class="session session-3 track-3" style="grid-column: track-3-start / track-3-end; grid-row: time-1015 / time-1115;">
                    <h3 class="session-title"><a href="/2023/program/papers/#3">Paper Session3 Locomotion</a></h3>
                        <span class="session-time">10:15 - 11:15</span>
                    </div>
                    <div class="session session-3 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1015 / time-1115;">
                        <h3 class="session-title"><a href="/2023/program/papers/#2">Paper Session2 Collaboration</a></h3>
                        <span class="session-time">10:15 - 11:15</span>
                    </div>
                    <div class="session session-3 track-event" style="grid-column: track-5-start / track-5-end; grid-row: time-1000 / time-1700;">
                        <h3 class="session-title"><a href="/2023/program/social-events/#industry-forum">Industry Forum</a></h3>
                        <span class="session-time">10:00 - 17:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>
                    <div class="session session-3 track-5" style="grid-column: track-1-start / track-3-end; grid-row: time-1115 / time-1200;">
                        <h3 class="session-title"><a>Posters & Demos & 3DUI Contest fast forward: session 1</a></h3>
                        <span class="session-time">11:15 - 12:00</span>
                    </div>
                    <div class="session session-3 track-lunch" style="grid-column: track-1-start / track-3-end; grid-row: time-1200 / time-1330;">
                        <h3 class="session-title">lunch</h3>
                        <span class="session-time">12:00 - 13:30</span>
                    </div>
                    <div class="session session-3 track-3dui" style="grid-column: track-4-start / track-4-end; grid-row: time-1000 / time-1200;">
                        <h3 class="session-title">Exhibition</h3><br>
                        <span class="session-time">10:00 - 12:00</span>
                    </div>
                    <div class="session session-3 track-poster" style="grid-column: track-4-start / track-4-end; grid-row: time-1200 / time-1330;">
                        <h3 class="session-title">Exhibition</h3><br>
                        <h3 class="session-title">Posters: session 1</h3>
                        <br>
                        <h3 class="session-title">Research Demos</h3>
                        <br>
                        <h3 class="session-title">3DUI Contest</h3>
                        <br>
                        <h3 class="session-title">Videos</h3>
                        <span class="session-time">12:00 - 13:30</span>
                    </div>
                    <div class="session session-3 track-3dui" style="grid-column: track-4-start / track-4-end; grid-row: time-1330 / time-1700;">
                        <h3 class="session-title">Exhibition</h3><br>
                        <span class="session-time">13:30 - 17:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>
                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <div class="session session-3 track-panel" style="grid-column: track-1-start / track-1-end; grid-row: time-1330 / time-1430;">
                        <h3 class="session-title"><a href="/2023/program/panels/#P1">Panel 1: Advancing Interactions in XR: Exploring New Input Technologies for the Metaverse</a></h3>
                        <span class="session-time">13:30 - 14:30</span>
                    </div>
                    <div class="session session-3 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1330 / time-1430;">
                        <h3 class="session-title"><a href="/2023/program/papers/#4">Paper Session4 Locomotion</a></h3>
                        <span class="session-time">13:30 - 14:30</span>
                    </div>
                    <div class="session session-3 track-3" style="grid-column: track-3-start / track-3-end; grid-row: time-1330 / time-1430;">
                        <h3 class="session-title"><a href="/2023/program/papers/#1">Paper Session5 Audio</a></h3>
                        <span class="session-time">13:30 - 14:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <div class="session session-3 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1430 / time-1445;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">14:30 - 14:45</span>
                    </div>
                    <div class="session session-3 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-1445 / time-1545;">
                        <h3 class="session-title"><a href="/2023/program/papers/#7">Paper Session6 Tracking</a></h3>
                        <span class="session-time">14:45 - 15:45</span>
                    </div>
                    <div class="session session-3 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1445 / time-1545;">
                        <h3 class="session-title"><a href="/2023/program/papers/#6">Paper Session7 Rendering</a></h3>
                        <span class="session-time">14:45 - 15:45</span>
                    </div>
                    <div class="session session-3 track-3" style="grid-column: track-3-start / track-3-end; grid-row: time-1445 / time-1545;">
                        <h3 class="session-title"><a href="/2023/program/papers/#12">Paper Session8 Cybersickness and SocialEmotional</a></h3>
                        <span class="session-time">14:45 - 15:45</span>
                    </div>
                    <div class="session session-3 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1545 / time-1600;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">15:45 - 16:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <div class="session session-3 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-1600 / time-1700;">
                        <h3 class="session-title"><a href="/2023/program/papers/#8">Paper Session9 360Video and Applications</a></h3>
                        <span class="session-time">16:00 - 17:00</span>
                    </div>
                    <div class="session session-3 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1600 / time-1700;">
                        <h3 class="session-title"><a href="/2023/program/papers/#9">Paper Session10 Agents</a></h3>
                        <span class="session-time">16:00 - 17:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <div class="session session-3 track-event" style="grid-column: track-1-start / track-5-end; grid-row: time-1800 / time-2000;">
                        <h3 class="session-title"><a href="/2023/program/social-events/#reception">Reception</a></h3>
                        <span class="session-time">18:00 - 22:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-2000;">22:00</p>
                </div>
            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible28" class="toggle" type="checkbox" checked> <label for="collapsible28" class="lbl-toggle">Tuesday, March 28</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Shanghai, China, UTC+8</strong></center>
                <div class="schedule-tue-28" aria-labelledby="schedule-heading">
                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <p class="time-slot" style="grid-row: time-0830;">08:30</p>
                    <div class="session session-1 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="/2023/program/papers/#14">Paper Session11 Displays and Haptics</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>
                    <div class="session session-2 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="/2023/program/papers/#11">Paper Session12 Cybersickness</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>
                    <div class="session session-2 track-event" style="grid-column: track-5-start / track-5-end; grid-row: time-0830 / time-1700;">
                        <h3 class="session-title"><a href="/2023/program/social-events/#industry-forum">Industry Forum</a></h3>
                        <span class="session-time">8:30 - 17:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-0900;">09:00</p>
                    <div class="session session-4 track-panel" style="grid-column: track-1-start / track-1-end; grid-row: time-0930 / time-1045;">
                        <h3 class="session-title"><a href="/2023/program/panels/#PP">Plenary Panel: Revisiting what is real about VR</a></h3>
                        <span class="session-time">9:30 - 10:45</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>
                    <div class="session session-4 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1045 / time-1100;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">10:45 - 11:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>
                    <div class="session session-5 track-keynote" style="grid-column: track-1-start / track-1-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title"><a href="/2023/program/keynote-speakers/#keynote-gao">Keynote2</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>
                    <div class="session session-8 track-5" style="grid-column: track-1-start / track-3-end; grid-row: time-1200 / time-1245;">
                        <h3 class="session-title"><a href="/2023/program/keynote-speakers/#keynote-gao">Posters & Demos & 3DUI Contest fast forward: session 2</a></h3>
                        <span class="session-time">12:00 - 12:45</span>
                    </div>
                    <div class="session session-9 track-lunch" style="grid-column: track-1-start / track-3-end; grid-row: time-1245 / time-1400;">
                        <h3 class="session-title">lunch</h3>
                        <span class="session-time">12:45 - 14:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <div class="session session-10 track-3dui" style="grid-column: track-4-start / track-4-end; grid-row: time-0830 / time-1245;">
                        <h3 class="session-title">Exhibition</h3><br>
                        <span class="session-time">08:30 - 12:45</span>
                    </div>
                    <div class="session session-10 track-poster" style="grid-column: track-4-start / track-4-end; grid-row: time-1245 / time-1400;">
                        <h3 class="session-title">Exhibition</h3><br>
                        <h3 class="session-title">Posters: session 2</h3>
                        <br>
                        <h3 class="session-title">Research Demos</h3>
                        <br>
                        <h3 class="session-title">3DUI Contest</h3>
                        <br>
                        <h3 class="session-title">Videos</h3>
                        <span class="session-time">12:45 - 14:00</span>
                    </div>
                    <div class="session session-10 track-3dui" style="grid-column: track-4-start / track-4-end; grid-row: time-1400 / time-1730;">
                        <h3 class="session-title">Exhibition</h3><br>
                        <span class="session-time">14:00 - 17:30</span>
                    </div>
                    <!-- <div class="session session-11 track-5" style="grid-column: track-5-start / track-5-end; grid-row: time-1230 / time-1400;">
                        <h3 class="session-title"><a>Posters & Demos: session 2</a></h3>
                        <span class="session-time">12:30 - 14:00</span>
                    </div> -->
                    <!-- <div class="session session-12 track-6" style="grid-column: track-6-start / track-6-end; grid-row: time-1230 / time-1400;">
                        <h3 class="session-title"><a>3DUI Contest</a></h3>
                        <span class="session-time">12:30 - 14:00</span>
                    </div> -->
                    <!-- <div class="session session-13 track-orange" style="grid-column: track-7-start / track-7-end; grid-row: time-1230 / time-1400;">
                        <h3 class="session-title"><a>Videos</a></h3>
                        <span class="session-time">12:30 - 14:00</span>
                    </div> -->
                    <div class="session session-16 track-panel" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="/2023/program/panels/#P2">Panel2: Can a visual design and game approach for VR increase engagement with health issues?</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>
                    <div class="session session-14 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="/2023/program/papers/#15">Paper Session13 Gaze</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>
                    <div class="session session-14 track-3" style="grid-column: track-3-start / track-3-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="/2023/program/papers/#17">Paper Session14
                        Interaction</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div><p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <div class="session session-15 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1500 / time-1515;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">15:00 - 15:15</span>
                    </div>
                    <div class="session session-14 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-1515 / time-1615;">
                        <h3 class="session-title"><a href="/2023/program/papers/#10">Paper Session15 Accessibility and Applications</a></h3>
                        <span class="session-time">15:15 - 16:15</span>
                    </div>
                    <div class="session session-17 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1515 / time-1615;">
                        <h3 class="session-title"><a  href="/2023/program/papers/#18">Paper Session16 Interaction</a></h3>
                        <span class="session-time">15:15 - 16:15</span>
                    </div>
                    <div class="session session-17 track-3" style="grid-column: track-3-start / track-3-end; grid-row: time-1515 / time-1615;">
                        <h3 class="session-title"><a  href="/2023/program/papers/#13">Paper Session17 Display</a></h3>
                        <span class="session-time">15:15 - 16:15</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <div class="session session-15 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1615 / time-1630;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">16:15 - 16:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <div class="session session-19 track-break" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-1800;">
                        <h3 class="session-title">Set up for Banquet</h3>
                        <span class="session-time">17:00 - 18:00</span>
                    </div>
                     <div class="session session-19 track-break" style="grid-column: track-5-start / track-5-end; grid-row: time-1700 / time-1800;">
                        <h3 class="session-title">Set up for Banquet</h3>
                        <span class="session-time">17:00 - 18:00</span>
                    </div>
                    <div class="session session-19 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1630 / time-1730;">
                        <h3 class="session-title"><a href="/2023/program/papers/#20">Paper Session18 Medical</a></h3>
                        <span class="session-time">16:30 - 17:30</span>
                    </div>
                    <div class="session session-19 track-3" style="grid-column: track-3-start / track-3-end; grid-row: time-1630 / time-1730;">
                        <h3 class="session-title"><a href="/2023/program/papers/#16">Paper Session19 Haptics</a></h3>
                        <span class="session-time">16:30 - 17:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <div class="session session-3 track-event" style="grid-column: track-1-start / track-5-end; grid-row: time-1800 / time-2030;">
                        <h3 class="session-title"><a href="/2023/program/social-events/#banquet">Banquet</a> & <a href="/2023/program/keynote-speakers/#keynote-lin">Keynote</a></h3>
                        <span class="session-time">18:00 - 20:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1900;">19:00</p>
                    <p class="time-slot" style="grid-row: time-2000;">20:00</p>
                </div>
            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible29" class="toggle" type="checkbox" checked> <label for="collapsible29" class="lbl-toggle">Wednesday, March 29</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Shanghai, China, UTC+8</strong></center>
                <div class="schedule-wed-29" aria-labelledby="schedule-heading">
                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-5; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-6; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-7; grid-row: tracks;"></span>
                    <p class="time-slot" style="grid-row: time-0830;">08:30</p>
                    <div class="session session-1 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="/2023/program/papers/#19">Paper Session20 Gestures and Interaction</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>
                    <div class="session session-2 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="/2023/program/papers/#21">Paper Session21 Perception</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>
                    <div class="session session-3 track-panel" style="grid-column: track-3-start / track-3-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title"><a href="/2023/program/panels/#P3">Panel3 [online]: Standards for Virtual Reality</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-0930;">09:30</p>
                    <div class="session session-4 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-0930 / time-0945;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">9:30 - 9:45</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-0945;">09:45</p>
                    <div class="session session-5 track-keynote" style="grid-column: track-1-start / track-1-end; grid-row: time-0945 / time-1045;">
                        <h3 class="session-title"><a>Keynote3</a></h3>
                        <span class="session-time">09:45 - 10:45</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1045;">10:45</p>
                    <div class="session session-4 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1045 / time-1100;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">10:45 - 11:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>
                    <div class="session session-5 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title"><a href="/2023/program/papers/#22">Paper Session22 Perception</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                    </div>
                    <div class="session session-6 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title"><a href="/2023/program/papers/#23">Paper Session23 SocialEmotional</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                    </div>
                    <div class="session session-7 track-3" style="grid-column: track-3-start / track-3-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title"><a href="/2023/program/papers/#24">Paper Session24 Education and Medical</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>
                    <div class="session session-8 track-5" style="grid-column: track-1-start / track-3-end; grid-row: time-1200 / time-1245;">
                        <h3 class="session-title"><a>Posters & Demos & 3DUI Contest fast forward: session 3</a></h3>
                        <span class="session-time">12:00 - 12:45</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1245;">12:45</p>
                    <div class="session session-4 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1245 / time-1400;">
                        <h3 class="session-title">lunch</h3>
                        <span class="session-time">12:45 - 14:00</span>
                    </div>
                    <div class="session session-10 track-3dui" style="grid-column: track-4-start / track-4-end; grid-row: time-0830 / time-1245;">
                        <h3 class="session-title">Exhibition</h3><br>
                        <span class="session-time">08:30 - 12:45</span>
                    </div>
                    <div class="session session-10 track-poster" style="grid-column: track-4-start / track-4-end; grid-row: time-1245 / time-1400;">
                        <h3 class="session-title">Exhibition</h3><br>
                        <h3 class="session-title">Posters: session 3</h3>
                        <br>
                        <h3 class="session-title">Research Demos</h3>
                        <br>
                        <h3 class="session-title">3DUI Contest</h3>
                        <br>
                        <h3 class="session-title">Videos</h3>
                        <span class="session-time">12:45 - 14:00</span>
                    </div>
                    <div class="session session-10 track-3dui" style="grid-column: track-4-start / track-4-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title">Exhibition</h3><br>
                        <span class="session-time">14:00 - 17:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <div class="session session-14 track-panel" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="/2023/program/panels/#P4">Panel4: Challenges and Opportunities of XR Applications for High-Risk Incidents</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>
                    <div class="session session-14 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="/2023/program/papers/#25">Paper Session25 Multimodal and Haptics</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>
                    <div class="session session-14 track-3" style="grid-column: track-3-start / track-3-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title"><a href="/2023/program/papers/#26">Paper Session26 Agents and Perception</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <div class="session session-15 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1500 / time-1515;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">15:00 - 15:15</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1515;">15:15</p>
                    <div class="session session-16 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-1515 / time-1615;">
                        <h3 class="session-title"><a href="/2023/program/papers/#27">Paper Session27 FoveatedRendering, Gaze, and Haptics</a></h3>
                        <span class="session-time">15:15 - 16:15</span>
                    </div>
                    <div class="session session-17 track-2" style="grid-column: track-2-start / track-2-end; grid-row: time-1515 / time-1615;">
                        <h3 class="session-title"><a href="/2023/program/papers/#28">Paper Session28 InfoVis and TextEntry</a></h3>
                        <span class="session-time">15:15 - 16:15</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1615;">16:15</p>
                    <div class="session session-18 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1615 / time-1700;">
                        <h3 class="session-title">break</h3>
                        <span class="session-time">16:15 - 16:45</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1630;">16:30</p>
                    <div class="session session-19 track-1" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-1730;">
                        <h3 class="session-title"><a>Closing & Awards</a></h3>
                        <span class="session-time">17:00 - 17:30</span>
                    </div>
                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <!-- <div class="session session-11 track-5" style="grid-column: track-5-start / track-5-end; grid-row: time-1230 / time-1400;">
                        <h3 class="session-title"><a>Posters & Demos: session 3</a></h3>
                        <span class="session-time">12:30 - 14:00</span>
                    </div> -->
                    <!-- <div class="session session-12 track-6" style="grid-column: track-6-start / track-6-end; grid-row: time-1230 / time-1400;">
                        <h3 class="session-title"><a>3DUI Contest</a></h3>
                        <span class="session-time">12:30 - 14:00</span>
                    </div> -->
                    <!-- <div class="session session-13 track-orange" style="grid-column: track-7-start / track-7-end; grid-row: time-1230 / time-1400;">
                        <h3 class="session-title"><a>Videos</a></h3>
                        <span class="session-time">12:30 - 14:00</span>
                    </div> -->
                </div>
            </div>
        </div>
    </div>
</div>

<!--
<div>
    <div class="wrap-collabsible"> <input id="collapsible3" class="toggle" type="checkbox" checked> <label for="collapsible3" class="lbl-toggle">Monday, March 29</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Lisbon WEST, UTC+1</strong></center>
                <div class="schedule-with-expo" aria-labelledby="schedule-heading">

                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0830; text-decoration: none;">8:30</p>

                    <div class="session session-1 track-teal" style="grid-column: track-1-start / track-4-end; grid-row: time-0830 / time-1000;">
                        <h3 class="session-title"><a href="/2021/program/plenary-sessions/#O1">Opening</a></h3>
                        <span class="session-time">8:30 - 10:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1000;">10:00</p>

                    <div class="session session-2 track-break" style="grid-column: track-1-start / track-4-end; grid-row: time-1000 / time-1030;">
                        <h3 class="session-title">Break</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1030;">10:30</p>

                    <div class="session session-3 track-keynote" style="grid-column: track-1-start / track-4-end; grid-row: time-1030 / time-1130;">
                        <h3 class="session-title"><a href="http://ieeevr.org/2021/program/keynote-speakers/#keynote-mohler">Keynote by Betty Mohler, Self-avatars in Immersive Technology</a></h3>
                        <span class="session-time">10:30 - 11:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1130;">11:30</p>

                    <div class="session session-4 track-break" style="grid-column: track-1-start / track-4-end; grid-row: time-1130 / time-1200;">
                        <h3 class="session-title">Break</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>

                    <div class="session session-5 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#3.1">Augmented Reality</a></h3>
                        <span class="session-time">12:00 - 13:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-6 track-green" style="grid-column: track-3-start / track-4-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#3.2">VR/AR Displays</a></h3>
                        <span class="session-time">12:00 - 13:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <div class="session session-7 track-break" style="grid-column: track-1-start / track-4-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Lunch</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>

                    <div class="session session-8 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#5.1">Emotion and Cognition</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-9 track-green" style="grid-column: track-3-start / track-4-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#5.2">Holographic and Inertial Displays</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>
                    <div class="session session-10 track-orange" style="grid-column: track-1-start / track-2-end; grid-row: time-1500 / time-1630;">
                        <h3 class="session-title"><a href="/2021/program/posters/">Posters</a> and <a href="/2021/program/demos/">Demos</a></h3>
                        <span class="session-time">15:00 - 16:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A</a></span>
                    </div>

                    <div class="session session-ex track-purple" style="grid-column: track-3-start / track-4-end; grid-row: time-1500 / time-1630;">
                        <h3 id="EX1" class="session-title"><a href="/2021/program/exhibitors/">Exhibition Hours</a></h3>
                        <span class="session-time">15:00 - 16:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A and B</a></span>
                    </div>


                    <p class="time-slot" style="grid-row: time-1630;">16:30</p>

                    <div class="session session-5 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-1630 / time-1730;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#7.1">Embodiment</a></h3>
                        <span class="session-time">16:30 - 17:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-6 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-1630 / time-1730;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#7.2">Visualization</a></h3>
                        <span class="session-time">16:30 - 17:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <div class="session session-ex track-purple" style="grid-column: track-4-start / track-4-end; grid-row: time-1630 / time-1800;">
                        <h3 id="EX1" class="session-title">Expo Session:</h3>
                        <span class="session-time">16:30: Qualcomm</span>
                        <span class="session-time">16:35: <a style="color: white;" href="https://www.youtube.com/watch?v=Sgw1DSbbSMY">Microsoft</a></span>
                        <span class="session-time">16:40: <a style="color: white;" href="https://www.youtube.com/watch?v=nq0NdCiB3FI">Facebook</a></span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Theater</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1730;">17:30</p>
                    <div class="session session-10 track-teal" style="grid-column: track-1-start / track-2-end; grid-row: time-1730 / time-1930;">
                        <h3 class="session-title"><a href="/2021/program/plenary-sessions/#O2">Welcome Reception</a> (including <a href="/2021/awards/vgtc-award-winners/">VGTC Awards</a>)</h3>
                        <span class="session-time">17:30 - 19:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-ex track-purple" style="grid-column: track-3-start / track-3-end; grid-row: time-1730 / time-1900;">
                        <h3 id="EW" class="session-title"><a href="/2021/program/exhibitors/">Exhibitors: Welcome Reception</a></h3>
                        <span class="session-time"><a style="color: white;" href="https://www.youtube.com/watch?v=Et-8EIRN_mw&t=4s">Virbela</a></span>
                        <span class="session-time">17:30 - 18:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>


                </div>

            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible7" class="toggle" type="checkbox" checked> <label for="collapsible7" class="lbl-toggle">Tuesday, March 30</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Lisbon WEST, UTC+1</strong></center>
                <div class="schedule-with-expo" aria-labelledby="schedule-heading">


                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0830;">8:30</p>

                    <div class="session session-1 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#1.1">Collaboration</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-2 track-green" style="grid-column: track-3-start / track-4-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#1.2">Multimodal Interfaces</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-0930;">9:30</p>
                    <div class="session session-3 track-orange" style="grid-column: track-1-start / track-2-end; grid-row: time-0930 / time-1100;">
                        <h3 class="session-title"><a href="/2021/program/posters/">Posters</a> and <a href="/2021/program/demos/">Demos</a></h3>
                        <span class="session-time">9:30 - 11:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall B</a></span>
                    </div>

                    <div class="session session-ex track-purple" style="grid-column: track-3-start / track-4-end; grid-row: time-0930 / time-1100;">
                        <h3 id="EX2" class="session-title"><a href="/2021/program/exhibitors/">Exhibition Hours</a></h3>
                        <span class="session-time">9:30 - 11:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A and B</a></span>
                    </div>



                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>

                    <div class="session session-4 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#2.1">Security and Drone Teleoperation</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-5 track-green" style="grid-column: track-3-start / track-4-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#2.2">Embedded and Surround Videos</a></h3>
                        <span class="session-time">11:00 - 12:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>
                    <div class="session session-6 track-break" style="grid-column: track-1-start / track-4-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Lunch</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>

                    <div class="session session-7 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#4.1">Virtual Humans and Agents</a></h3>
                        <span class="session-time">13:00 - 14:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-8 track-green" style="grid-column: track-3-start / track-4-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#4.2">Hands, Gestures and Grasping</a></h3>
                        <span class="session-time">13:00 - 14:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>

                    <div class="session session-9 track-break" style="grid-column: track-1-start / track-4-end; grid-row: time-1400 / time-1430;">
                        <h3 class="session-title">Break</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1430;">14:30</p>

                    <div class="session session-10 track-keynote" style="grid-column: track-1-start / track-4-end; grid-row: time-1430 / time-1530;">
                        <h3 class="session-title">
                            <a href="http://ieeevr.org/2021/program/keynote-speakers/#keynote-oliver">Keynote by Nuria Oliver, Data Science to fight against COVID-19</a>
                        </h3>
                        <span class="session-time">14:30 - 15:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1530;">15:30</p>

                    <div class="session session-11 track-break" style="grid-column: track-1-start / track-4-end; grid-row: time-1530 / time-1600;">
                        <h3 class="session-title">Break</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <div class="session session-12 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-1600 / time-1700;">
                        <h3 class="session-title">Social Event: <a href="/2021/program/bofs/">Birds of a Feather</a></h3>
                        <span class="session-time">16:00 - 17:00</span>
                    </div>

                    <div class="session session-ex track-purple" style="grid-column: track-3-start / track-4-end; grid-row: time-1600 / time-1700;">
                        <h3 id="EX3" class="session-title"><a href="/2021/program/exhibitors/">Exhibition Hours</a></h3>
                        <span class="session-time">16:00 - 17:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A and B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>

                    <div class="session session-13 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-1700 / time-1800;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#8.1">Plausibility, Presence and Social VR</a></h3>
                        <span class="session-time">17:00 - 18:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-14 track-panel" style="grid-column: track-3-start / track-4-end; grid-row: time-1700 / time-1830;">
                        <h3 class="session-title"><a href="/2021/program/panels/#P1">Panel: Opportunities and Challenges in Harnessing VR Technology for Bias Mitigation</a></h3>
                        <span class="session-time">17:00 - 18:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <div class="session session-15 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-1800 / time-1900;">
                        <h3 class="session-title">Mixer</h3>
                        <span class="session-time">18:00 - 19:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Music Hall</a></span>
                        
                    </div>

                </div>

            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible4" class="toggle" type="checkbox" checked> <label for="collapsible4" class="lbl-toggle">Wednesday, March 31</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Lisbon WEST, UTC+1</strong></center>
                <div class="schedule-with-expo" aria-labelledby="schedule-heading">


                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-4; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0830;">8:30</p>

                    <div class="session session-1 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#1.3">Accessible VR</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-2 track-green" style="grid-column: track-3-start / track-4-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#1.4">Haptics</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-0930;">09:30</p>
                    <div class="session session-3 track-event" style="grid-column: track-1-start / track-2-end; grid-row: time-0930 / time-1030;">
                        <h3 class="session-title">Social Event: <a href="/2021/program/bofs/">Birds of a Feather</a></h3>
                        <span class="session-time">9:30 - 10:30</span>
                    </div>

                    <div class="session session-ex track-purple" style="grid-column: track-3-start / track-3-end; grid-row: time-0930 / time-1100;">
                        <h3 id="EX4" class="session-title"><a href="/2021/program/exhibitors/">Exhibition Hours</a></h3>
                        <span class="session-time">9:30 - 11:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A and B</a></span>
                    </div>

                    <div class="session session-ex track-purple" style="grid-column: track-4-start / track-4-end; grid-row: time-0930 / time-1030;">
                        <h3 id="EX1" class="session-title">Expo Session:</h3>
                        <span class="session-time">9:30: <a style="color: white;" href="https://youtu.be/17YUBD7V-KQ">HIT Lab NZ</a></span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Theater</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1030;">10:30</p>

                    <div class="session session-4 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1030 / time-1100;">
                        <h3 class="session-title">Break</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1100;">11:00</p>

                    <div class="session session-5 track-keynote" style="grid-column: track-1-start / track-4-end; grid-row: time-1100 / time-1200;">
                        <h3 class="session-title">Keynote
                            <a href="http://ieeevr.org/2021/program/keynote-speakers/#keynote-steinicke">Keynote by Frank Steinicke, B(l)ending Realities</a>
                        </h3>
                        <span class="session-time">11:00 - 12:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>
                    <div class="session session-6 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Lunch</h3>
                    </div>
                    <div class="session session-6fasgfsx track-3dui" style="grid-column: track-4-start / track-4-end; grid-row: time-1200 / time-1230;">
                        <h3 class="session-title"><a href="/2021/program/3dui-contest/">3DUI Contest Fast Forward</a></h3>
                        <span class="session-time">12:00 - 12:10</span>
                    </div>
                    
                    

                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>

                    
                    <div class="session session-7 track-event" style="grid-column: track-1-start / track-1-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Mixer</h3>
                        <span class="session-time">13:00 - 14:00</span>
                    </div>
                   

                    <div class="session session-8 track-green" style="grid-column: track-1-start / track-4-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#4.3">Redirected Locomotion</a></h3>
                        <span class="session-time">13:00 - 14:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <div class="session session-9 track-orange" style="grid-column: track-1-start / track-2-end; grid-row: time-1400 / time-1530;">
                        <h3 class="session-title"><a href="/2021/program/posters/">Posters</a> and <a href="/2021/program/demos/">Demos</a></h3>
                        <span class="session-time">14:00 - 15:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A and B</a></span>
                    </div>

                    <div class="session session-xxx track-3dui" style="grid-column: track-3-start / track-3-end; grid-row: time-1400 / time-1530;">
                        <h3 class="session-title"><a href="/2021/program/3dui-contest/">3DUI Contest</a></h3>
                        <span class="session-time">14:00 - 15:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A</a></span>
                    </div>

                    <div class="session session-ex track-purple" style="grid-column: track-4-start / track-4-end; grid-row: time-1400 / time-1530;">
                        <h3 id="EX5" class="session-title"><a href="/2021/program/exhibitors/">Exhibition Hours</a></h3>
                        <span class="session-time">14:00 - 15:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A and B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1530;">15:30</p>

                    <div class="session session-10 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-1530 / time-1630;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#6.1">Selection and Manipulation</a></h3>
                        <span class="session-time">15:30 - 16:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-11 track-panel" style="grid-column: track-3-start / track-4-end; grid-row: time-1530 / time-1700;">
                        <h3 class="session-title"><a href="/2021/program/panels/#P2">Panel: Shaping the Future of XR and Arts</a></h3>
                        <span class="session-time">15:30 - 17:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1630;">16:30</p>

                    <div class="session session-12 track-break" style="grid-column: track-1-start / track-2-end; grid-row: time-1630 / time-1700;">
                        <h3 class="session-title">Break</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>

                    <div class="session session-13 track-green" style="grid-column: track-1-start / track-2-end; grid-row: time-1700 / time-1800;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#8.2">Training and Learning</a></h3>
                        <span class="session-time">17:00 - 18:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-14 track-green" style="grid-column: track-3-start / track-4-end; grid-row: time-1700 / time-1800;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#8.3">Pen-based and Hands-free Interaction</a></h3>
                        <span class="session-time">17:00 - 18:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1800;">18:00</p>
                    <div class="session session-15 track-event" style="grid-column: track-1-start / track-4-end; grid-row: time-1800 / time-1900;">
                        <h3 class="session-title">Mixer</h3>
                        <span class="session-time">18:00 - 19:00</span>
                    </div>

                </div>

            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible5" class="toggle" type="checkbox" checked> <label for="collapsible5" class="lbl-toggle">Thursday, April 1</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Lisbon WEST, UTC+1</strong></center>
                <div class="schedule" aria-labelledby="schedule-heading">


                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0830;">8:30</p>

                    <div class="session session-1 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#1.5">Locomotion</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-2 track-green" style="grid-column: track-2-start / track-3-end; grid-row: time-0830 / time-0930;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#1.6">Rendering and Texture Mapping</a></h3>
                        <span class="session-time">8:30 - 9:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-0930;">09:30</p>
                    <div class="session session-3 track-event" style="grid-column: track-1-start / track-3-end; grid-row: time-0930 / time-1030;">
                        <h3 class="session-title">Social Event: <a href="/2021/program/bofs/">Birds of a Feather</a></h3>
                        <span class="session-time">9:30 - 10:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1030;">10:30</p>
                    <div class="session session-4 track-orange" style="grid-column: track-1-start / track-2-end; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title"><a href="/2021/program/posters/">Posters</a> and <a href="/2021/program/demos/">Demos</a></h3>
                        <span class="session-time">10:30 - 12:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A and B</a></span>
                    </div>


                    <div class="session session-ex track-purple" style="grid-column: track-3-start / track-3-end; grid-row: time-1030 / time-1200;">
                        <h3 id="EX6" class="session-title"><a href="/2021/program/exhibitors/">Exhibition Hours</a></h3>
                        <span class="session-time">10:30 - 12:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A and B</a></span>
                    </div>


                    <p class="time-slot" style="grid-row: time-1200;">12:00</p>

                    <div class="session session-5 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1200 / time-1300;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#3.3">Tracking, Vision and Sound</a></h3>
                        <span class="session-time">12:00 - 13:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-5 track-panel" style="grid-column: track-2-start / track-3-end; grid-row: time-1200 / time-1330;">
                        <h3 class="session-title"><a href="/2021/program/panels/#P3">Panel: What makes a virtual human human?</a></h3>
                        <span class="session-time">12:00 - 13:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <div class="session session-7 track-break" style="grid-column: track-1-start / track-1-end; grid-row: time-1300 / time-1400;">
                        <h3 class="session-title">Lunch</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>

                    <div class="session session-8 track-green" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#5.3">Perception</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-9 track-green" style="grid-column: track-2-start / track-3-end; grid-row: time-1400 / time-1500;">
                        <h3 class="session-title">Papers: <a href="/2021/program/papers/#5.4">VR Applications</a></h3>
                        <span class="session-time">14:00 - 15:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1500;">15:00</p>

                    <div class="session session-10 track-break" style="grid-column: track-1-start / track-3-end; grid-row: time-1500 / time-1530;">
                        <h3 class="session-title">Break</h3>
                    </div>

                    <p class="time-slot" style="grid-row: time-1530;">15:30</p>

                    <div class="session session-11 track-keynote" style="grid-column: track-1-start / track-3-end; grid-row: time-1530 / time-1630;">
                        <h3 class="session-title">
                            <a href="http://ieeevr.org/2021/program/keynote-speakers/#keynote-feiner">Keynote by Steven Feiner, AR Longa, VR Brevis? Thinking About Our Future</a>
                        </h3>
                        <span class="session-time">15:30 - 16:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1630;">16:30</p>

                    <div class="session session-2 track-teal" style="grid-column: track-1-start / track-2-end; grid-row: time-1630 / time-1800;">
                        <h3 class="session-title"><a href="/2021/program/plenary-sessions/#O3">Closing</a></h3>
                        <span class="session-time">16:30 - 18:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1730;">17:30</p>
                    <div class="session session-ex track-purple" style="grid-column: track-3-start / track-3-end; grid-row: time-1730 / time-1900;">
                        <h3 id="EX7" class="session-title"><a href="/2021/program/exhibitors/">Exhibition Hours</a></h3>
                        <span class="session-time">17:30 - 18:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Expo Hall A and B</a></span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<div>
    <div class="wrap-collabsible"> <input id="collapsible6" class="toggle" type="checkbox" checked> <label for="collapsible6" class="lbl-toggle">Friday, April 2</label>
        <div class="collapsible-content">
            <div class="content-inner">
                <center><strong>Lisbon WEST, UTC+1</strong></center>
                <div class="schedule-fri-2" aria-labelledby="schedule-heading">


                    <span class="track-slot" aria-hidden="true" style="grid-column: times; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-1; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-2; grid-row: tracks;"></span>
                    <span class="track-slot" aria-hidden="true" style="grid-column: track-3; grid-row: tracks;"></span>

                    <p class="time-slot" style="grid-row: time-0900;">9:00</p>
                    <div class="session session-1 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-0900 / time-1200;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#WEVR">Workshop: Everyday Virtual Reality (WEVR)</a></h3>
                        <span class="session-time">9:00 - 12:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1300;">13:00</p>
                    <div class="session session-ex track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-1300 / time-1600;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#EXR">Workshop: Ethics in VR (EXR)</a></h3>
                        <span class="session-time">13:00 - 16:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1400;">14:00</p>
                    <div class="session session-2 track-teal" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title"><a href="/2021/program/tutorials/#T3">Tutorial: bmlTUX – a simple toolkit for building experiments in Unity</a></h3>
                        <span class="session-time">14:00 - 16:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>
                    <div class="session session-3 track-teal" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1700;">
                        <h3 class="session-title"><a href="/2021/program/tutorials/#T5">Tutorial: Emotion in Virtual Reality</a></h3>
                        <span class="session-time">14:00 - 16:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1600;">16:00</p>
                    <div class="session session-4 track-green" style="grid-column: track-3-start / track-3-end; grid-row: time-1600 / time-2100;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#KELVAR">Workshop: K-12+ Embodied Learning through Virtual and Augmented Reality</a></h3>
                        <span class="session-time">16:00 - 21:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium C</a></span>
                    </div>

                    <p class="time-slot" style="grid-row: time-1700;">17:00</p>
                    <div class="session session-5 track-teal" style="grid-column: track-1-start / track-1-end; grid-row: time-1700 / time-2030;">
                        <h3 class="session-title">
                            <a href="/2021/program/tutorials/#T6S3">
                                Tutorial: Combining the Virtual and the Real, Session 3
                            </a>
                        </h3>
                        <span class="session-time">17:00 - 20:30</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium A</a></span>
                    </div>

                    <div class="session session-6 track-green" style="grid-column: track-2-start / track-2-end; grid-row: time-1700 / time-2100;">
                        <h3 class="session-title"><a href="/2021/contribute/workshoppapers/#Finding-a-way-forward-in-VR-locomotion">Workshop: Finding a way forward in VR locomotion</a></h3>
                        <span class="session-time">17:00 - 21:00</span>
                        <span class="session-title"><b style="color: white;">Location:</b> <a href="/2021/attend/virbela-instructions/#map">Auditorium B</a></span>
                    </div>
                </div>

            </div>
        </div>
    </div>
</div> -->
