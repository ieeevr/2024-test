---
layout: ieeevr-default
title: "Workshops Call for paper"
subtitle: "IEEE VR 2024"
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
        <strong style="color: black">IEEE VR 2024: the 31<sup>st</sup> IEEE Conference on Virtual Reality and 3D User Interfaces </strong>
        <br>
        March 16-21, 2024 | Contemporary Resort, Walt Disney World, Orlando, Florida USA
        <br>
        <a href="https://ieeevr.org/2024/">https://ieeevr.org/2024/</a>
    </p>
    <p>
        IEEE VR 2024 seeks high-quality contributions to the following 18 workshops. 
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

    <!-- ------------------------------------------------MASSXR-------------------------------------------------------- -->

    <h2 id="MASSXR"> Multi-modal Affective and Social Behavior Analysis and Synthesis in Extended Reality (MASSXR) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/massxrworkshop2024" target="_blank">https://sites.google.com/view/massxrworkshop2024</a>
    </p>
    <ul>
        <li> Submission deadline: 9<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 27<sup>rd</sup> January 2024 </li>
    </ul>
    <p>
        The objective of this workshop on Multi-modal Affective and Social Behavior Analysis and Synthesis in Extended Reality is to bring together researchers and practitioners working in the field of social and affective computing with the ones on 3D computer vision and computer graphics/animation and discuss the current state and future directions, opportunities, and challenges. The workshop aims to establish a new platform for the development of immersive embodied intelligence at the intersection of Artificial intelligence (AI) and Extended Reality (XR). We expect that the workshop will provide an opportunity for researchers to develop new techniques and will lead to new collaboration among the participants. 
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Zerrin Yumak
    </p>

    <!-- ------------------------------------------------VR4Exergame-------------------------------------------------------- -->

    <h2 id="VR4Exergame"> First Workshop on VR for Exergaming (VR4Exergame) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'PrXR' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://altecresearch.com/vr4exergame/" target="_blank">https://altecresearch.com/vr4exergame/</a>
    </p>
    <ul>
        <li> Submission deadline: 6<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        VR exergames have potential to enable a broad spectrum of users to participate in fitness and rehabilitation activities in immersive social environments. Yet, consumer grade VR systems show only limited ability to realize the adoption of VR exergaming at such scale. Key challenges to enable VR as an engaging, interactive and social alternative to existing practices include – therapeutic benefits to fitness and rehabilitation activities; human factors including the ability to simulate real-world scenarios, long term usage comfort among others; and technical capabilities such as simplified system setup, low multi-user latency, and realistic whole-body immersion. This full-day workshop will bring researchers and industry practitioners together to discuss these new emerging research challenges and technologies. It will consist of keynote speakers, juried paper presentations, and a panel discussion. We invite authors to submit 6-page (plus 1-page for references) research or position papers.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Bhawna Shiwani
    </p>

    <!-- ------------------------------------------------KELVAR-------------------------------------------------------- -->

    <h2 id="KELVAR"> KELVAR Workshop: K-12&#43; Embodied Learning through Virtual and Augmented Reality (KELVAR) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
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
    {% endfor %}-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/site/vrkelvar/" target="_blank">https://sites.google.com/site/vrkelvar/</a>
    </p>
    <ul>
        <li> Submission deadline: 14<sup>rd</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        In this workshop we aim to bring together educators, developers and researchers who are interested in creating and deploying XR technologies for the educational contexts of the future.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Steven Cutchin
    </p>

    <!-- ------------------------------------------------TrainingXR-------------------------------------------------------- -->

    <h2 id="TrainingXR"> 4th Annual Workshop on 3D Content Creation for Simulated Training in eXtended Reality (TrainingXR) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'SIVE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/trainingxrieeevr2024/trainingxr" target="_blank">https://sites.google.com/view/trainingxrieeevr2024/trainingxr</a>
    </p>
    <ul>
        <li> Submission deadline: 12<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 27<sup>th</sup> January 2024 </li>
    </ul>
    <p>
        This workshop discusses and articulates research visions on using the latest extended reality (VR/AR/MR) technologies for education and training purposes, and on creating immersive 3D virtual content for delivering effective and personalized training experiences. This workshop will gather researchers and practitioners in a variety of computer disciplines related to XR training and content creation. This workshop will accept research papers on these topics. We will also invite renowned speakers from the research community and the industry to give talks related to XR-based training, to inspire the field to further explore this promising direction. 
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Lap Fai (Craig) Yu
    </p>

    <!-- ------------------------------------------------ENPT-XR-------------------------------------------------------- -->

    <h2 id="ENPT-XR"> Workshop on Emerging Novel Prototyping Techniques for XR (ENPT XR)   </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'DISCE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="http://www.xrprototyping.com" target="_blank">http://www.xrprototyping.com</a>
    </p>
    <ul>
        <li> Submission deadline: 15<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        This full-day workshop will bring together researchers and industry practitioners from different backgrounds to discuss the future of prototyping for VR, AR, and 3D User Interfaces, and help chart a course for the future of XR prototyping techniques. 

    </p>

    <p>
        <strong style="color:black;">Principal Organizer:</strong> Assem Kroma
    </p>

    <!-- ------------------------------------------------XRIOS-------------------------------------------------------- -->

    <h2 id="XRIOS"> 2nd International Workshop on eXtended Reality for Industrial and Occupational Support (XRIOS) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong>  <a href="https://sites.google.com/view/xrios" target="_blank">https://sites.google.com/view/xrios</a>
    </p> 
    
    <ul>
        <li> Submission deadline: 25<sup>th</sup> January 2024 </li>
        <li> Notification of results: 30<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 03<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        This workshop—eXtended Reality for Industrial and Occupational Supports (XRIOS)—aims to identify the current state of XR research and the gaps in the scope of human factors and ergonomics, mainly related to the industrial and occupational tasks, and discuss potential future research directions. XRIOS will build a community that bridges XR developers, human factors and ergonomics researchers interested in industrial and occupational applications.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Kangsoo Kim
    </p>

    <!-- ------------------------------------------------XRHealth-------------------------------------------------------- -->

    <h2 id="XRHealth"> 2nd XR Health workshop - XR Technologies for Healthcare and Wellbeing </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'DISCE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="{{"/assets/contribute/workshops/XR-HealthWorkshopIEEEVR2023-Matias-Volonte.pdf" | relative_url }}" target="_blank">Call for paper</a>
    </p>
    <ul>
        <li> Submission deadline: 10<sup>th</sup> January 2024 </li>
        <li> Notification of results: 13<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 16<sup>th</sup> January 2024 </li>
    </ul>
    <p>
        We aim to gather the intersection of researchers working in the areas of XR for healthcare and wellbeing from the HCI community to come together to share their ideas and discuss possible future grand challenges. 
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Matias Volonte
    </p>

    <!-- ------------------------------------------------ReDigiTS-------------------------------------------------------- -->

    <h2 id="ReDigiTS"> 3D Reconstruction, Digital Twinning, and Simulation for Virtual Experiences (ReDigiTS) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'WISP' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/redigits2024" target="_blank">https://sites.google.com/view/redigits2024</a>
    </p>
    <ul>
        <li> Submission deadline: 5<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 28<sup>th</sup> January 2024 </li>
    </ul>
    <p>
        The aim of this workshop is to attract a collection of high-quality submissions reporting state-of-the-art research activities targeted to the next generation of immersive experiences, reporting the latest methodologies, applications, standards, evaluations, and/or use cases for 3D reconstruction, digital twinning, and simulation for immersive experiences. Despite the pivotal role played by these research directions in the design and development of immersive experiences, they are only partially addressed in the topics of workshops organized in the previous editions of IEEE VR. 
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Alberto Cannavò
    </p>

    <!-- ------------------------------------------------Data4XR-------------------------------------------------------- -->

    <h2 id="Data4XR"> Data4XR: Datasets for Developing Intelligent XR Applications </h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'VHCIE2021' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/view/ieee-vr-data4xr" target="_blank">https://sites.google.com/view/ieee-vr-data4xr</a>
    </p>
    <ul>
        <li> Submission deadline: 9<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        With easy access to standard datasets, they can develop state-of-the-art AI algorithms to achieve excellent prediction performance. However, when XR researchers decide to import these algorithms for developing intelligent immersive interactive applications, the lack of publicly available datasets arises as a challenge despite advanced AI algorithms being developed.
 
    </p>
    <p>
        Many works related to datasets have been published, e.g., MINIST, ImageNet, CIFAR-10, etc. To unleash the full power of XR, the community also needs standard datasets for developing data-driven models with machine/deep learning. The 2nd workshop on Datasets for Developing Intelligent XR Applications (Data4XR), hosted by the IEEE VR 2024, proposes a meaningful platform for domain researchers to find valuable resources and develop collaborations across labs. It aims to promote XR research by involving artificial intelligence.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Yuyang Wang
    </p>

    <!-- ------------------------------------------------MixReal-------------------------------------------------------- -->

    <h2 id="MixReal"> Mixing Realities: Cross-reality Visualization, Interaction, and Collaboration </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="{{"/assets/contribute/workshops/MixingRealitiesIEEEVR2023-LingyunYu.pdf" | relative_url }}" target="_blank">Call for paper</a>
    </p>
    <ul>
        <li> Submission deadline: 15<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        Cross-reality systems offer different levels of virtuality/physicality to users and enable them to move back and forth between the reality-virtuality continuums in a seamless way. Immersive AR/VR HMDs  have become the main tools that enable cross-reality interaction. 
    </p>
    <p>
    Immersive analytics has become a significant research field with applications in natural sciences in contexts that require users’ understanding, exploration, and communication about high-dimensional data. Cross-reality provides users with the possibility of switching visual representations between systems using different degrees of virtuality and allows users to interact with data across multiple technologies. 
    </p>
    <p>
    The goal of the workshop is to provide an opportunity for researchers from VR/MR/AR, HCI and Visualization fields to submit their original ideas, work-in-progress contribution, and position papers on the design of interactive systems for effective cross-reality visualization, interaction, and collaboration.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Hai-Ning Liang
    </p>
    
    <!-- ------------------------------------------------WIVL-------------------------------------------------------- -->

    <h2 id="WIVL"> Workshop on Immersive Visualization Laboratories - Past, Present and Future.  </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'DISCE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://ivl-workshop.github.io/" target="_blank">https://ivl-workshop.github.io/</a>
    </p>
    <ul>
        <li> Submission deadline: 13<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        The goal of this workshop is to gather practitioners from immersive visualization laboratories to share their success stories, information about their hardware setups and the software they used and/or developed.  Discussion can also include "not-so-successful" stories with lessons learned and workshop participants will also come together to discuss the future of large-scale immersive visualization labs. We also hope to bring visualization practitioners together to advance the way our field works with immersive visualization hardware and software frameworks for a sustainable immersive visualization laboratory.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> William Sherman
    </p>

    <!-- ------------------------------------------------SecImmeWorld-------------------------------------------------------- -->

    <h2 id="SecImmeWorld"> First Workshop on Security and Privacy for Immersive Virtual Worlds (Secure Immersive Worlds) </h2>
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="{{"/assets/contribute/workshops/SecurityandPrivacyforSecureImmersiveWorlds-SeanBanerjee.pdf" | relative_url }}" target="_blank">Call for paper</a>
    </p>
    <ul>
        <li> Submission deadline: 6<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        As critical applications in healthcare, education, finance, teleoperation, and retail emerge in the future immersive worlds, ensuring security and privacy of users from internal and external attacks becomes vital. A significant quantity of sensitive data is likely to be generated by the widespread adoption of VR/XR/MR/AR technologies in "serious" immersive worlds. Traditional approaches for security and privacy fail to capture the subtleties of *R hardware/software systems and the impact of human behavior. The Secure Immersive Worlds workshop aims to cover these open research and technological challenges and garner ideas in ensuring continued security and privacy of users in serious immersive worlds. The full-day workshop will bring researchers and industry practitioners together to discuss these new emerging research challenges and technologies. The workshop will consist of keynote speakers, juried paper presentations, and a panel discussion. 
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Sean Banerjee
    </p>

    <!-- ------------------------------------------------EUCHS-------------------------------------------------------- -->

    <h2 id="EUCHS"> Enhancing User Comfort, Health and Safety in VR and AR  </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'DISCE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="{{"/assets/contribute/workshops/EUCHSARVR-CFP-ArashMahnan.pdf" | relative_url }}" target="_blank">Call for paper</a>
    </p>
    <ul>
        <li> Submission deadline: 10<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        Over the last few years, we have seen an increase in consumer AR and VR devices. Consequently, there is a plethora of new content being created for consumption such as games, social/meeting applications, therapeutic applications, and more. However, widespread acceptance of AR and VR is dependent on user comfort, health, and safety. So, these issues are becoming increasingly important aspects of AR and VR use to research and discuss. 

    </p>
    <p>
    This workshop will provide a venue to present, discuss, and brainstorm issues around user comfort, health and safety. The topics to be considered include, but are not limited to, visually induced motion sickness, perceptual and cognitive distraction, comfort, long-term use and other psychological and physical issues relevant to AR and VR usage. We are interested in all factors that may impact the adoption and retention of use of AR and VR in either the general public or in specific user groups such as medical professionals, industrial or knowledge workers.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Arash Mahnan
    </p>

    <!-- ------------------------------------------------WISP-------------------------------------------------------- -->

    <h2 id="WISP"> Workshop on Immersive Sickness Prevention (WISP) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://sites.google.com/umn.edu/wisp" target="_blank">https://sites.google.com/umn.edu/wisp</a>
    </p>
    <ul>
        <li> Submission deadline: 13<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 27<sup>th</sup> January 2024 </li>
    </ul>
    <p>
        The workshop is intended to foster discussion between researchers, developers, and practitioners interested in addressing cybersickness, one of the most significant usability issues in VR. Although immersive technologies have been advancing rapidly, their rate of public adoption has been slowed by the fact that many users experience physical discomfort during or after the use of VR devices, with symptomatic characteristics similar to motion sickness. The workshop will include research papers that report study results, novel interaction techniques, or technological interventions aimed towards understanding and mitigating cybersickness, as well as position papers describing early-stage concepts, preliminary results, or case studies from industry. We hope that the results of the workshop and the discussions will lead to improved design practices, new technological approaches, and a better understanding of the causes of immersive sickness.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Isayas Berhe Adhanom
    </p>

    <h2 id="ANIVAE-2024"> 6<sup>th</sup> IEEE VR Internal Workshop on Animation in Virtual and Augmented Environments (ANIVAE-2024) </h2>
    
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE-2024' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://anivae.fhstp.ac.at/" target="_blank"> https://anivae.fhstp.ac.at/ </a>
    </p>
    <ul>
        <li> Submission deadline: 2<sup>nd</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 30<sup>th</sup> January 2024 </li>
    </ul>
    <p>
        Connecting specialists from various digital humanities research areas (such as animation, games and media studies), with experts from both vision-oriented computer science areas (such as computer graphics or information visualization), and experts from technically-oriented computer science areas (such as data integration, internet-of-things or smart automation), the ANIVAE workshops aims to create an open and exciting environment. By encouraging synergies of interdisciplinary approaches, the workshop maps animation within the AVR context from different angles and creates new knowledge in this research field.   
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Thomas Moser
    </p>
    
    <!-- ------------------------------------------------I-Meta-------------------------------------------------------- -->

    <h2 id="I-Meta"> Industrial Metaverse (I-Meta) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="{{"/assets/contribute/workshops/Industrial-Metaverse.pdf" | relative_url }}" target="_blank">Call for paper</a>
    </p>
    <ul>
        <li> Submission deadline: 15<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
        I-Meta intends to invite all researchers and practitioners to participate and discuss new theories, architectures, technologies, patterns, or application scenarios of industrial metaverse, to share new scientific findings or practical achievements, and to describe the future vision of industrial metaverse for fostering new ideas.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Hongming Cai, Shuangjiu Xiao, Bingqing Shen
    </p>

    <!-- ------------------------------------------------ARES-------------------------------------------------------- -->

    <h2 id="ARES"> ARES - Augmented Reality Enabling Superhuman Sports + Serious Games (2nd Annual Workshop) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'DISCE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://wiki.tum.de/pages/viewpage.action?pageId=1003688592" target="_blank">https://wiki.tum.de/pages/viewpage.action?pageId=1003688592</a>
    </p>
    <ul>
        <li> Submissions due: 10<sup>th</sup> January 2024 </li>
        <li> Notification of results: 20<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 3<sup>rd</sup> February 2024 </li>
    </ul>
    <p>
    <ul>
        <li>a. Introduction to the topic of Serious Games and Superhuman Sports (Organizers)</li>
        <li>b. Overview about the current research (Organizers)</li>
        <li>c. Paper Presentations (Organizers & Participants)</li>
        <li>d. Discussion, Future Work, Collaboration</li>
    </ul>
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Christian Eichhorn
    </p>
    

<!-- ------------------------------------------------OAT-------------------------------------------------------- -->

    <h2 id="OAT"> Open Access Tools and libraries for virtual reality (OAT) </h2>
    <!-- TAKE ME TO THE EVENT START -->
    <!--{% for event in site.data.events %}
    {% if event.id == 'ANIVAE' %}
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
    {% endfor %}-->
    <!-- TAKE ME TO THE EVENT END-->
    
    <p>
        <strong style="color:black;">Website:</strong> <a href="https://openvrlab.github.io/" target="_blank">https://openvrlab.github.io/</a>
    </p>
    <ul>
        <li> Submission deadline: 13<sup>th</sup> January 2024 </li>
        <li> Notification of results: 16<sup>th</sup> January 2024 </li>
        <li> Camera-ready submission due: 29<sup>th</sup> January 2024 </li>
    </ul>
    <p>
        Virtual reality researchers and developers need tools to develop state of the art technologies that will help advance knowledge. The goal of this workshop is promoting open-Source tools which can be modified or redistributed. Open access tools are critical to eliminate redundancies and increase world research collaboration in VR. At a time that academic research needs to move as fast as the industry, collaboration and shared tools are the best way to do it.
    </p>
    <p>
        <strong style="color:black;">Principal Organizer:</strong> Matias Volonte
    </p>
    






    
</div> 