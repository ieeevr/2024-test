---
layout: ieeevr-default
title: "Program Overview"
---
<link rel="stylesheet" href="{{ '/assets/css/calendar.css' | relative_url }}?version=20240108_1">
    
<script>
    (function($) {
        $(function() {
            $("#accordion > div").accordion({ header: "h4", heightStyle: "content", active: false, collapsible: true });
        })
    })(jQuery);

   $(document).ready(function(){
		$('#day1').click(); 
		$('#day2').click(); 
		$('#day3').click(); 
		$('#day4').click(); 
		$('#day5').click(); 
		$('#day6').click(); 
    });   
</script>

<h1 id="schedule-heading">Program Overview</h1>
<div class="notice--info alignCenter bold" style="font-size: 0.9em !important;">
    Please note that all times are given in Orlando, Florida USA local time, EDT (UTC-4).
</div>
<div class="clear"></div>
<div id="accordion">
    <div>
        <h4 id="day1">Saturday, 16 March 2024</h4>
        <div class="schedule-sat" aria-labelledby="Saturday, 16 March 2024Workshop Schedule"> 
            <p class="time-slot" style="grid-row: time-0800;">8:00</p>             
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'XRGaming' %}
                    <div class="session session-w1a track-blue" style="grid-column: track-1; grid-row: time-0800 / time-1000;">                    
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}   
            {% endfor %}             
            {% for workshop in site.data.workshops %}   
                {% if workshop.id == 'WSR' %}
                    <div class="session session-w2a track-blue" style="grid-column: track-2; grid-row: time-0800 / time-1000;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>         
                {% endif %}     
            {% endfor %}                  
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'XRIOS' %}
                    <div class="session session-w3a track-blue" style="grid-column: track-3; grid-row: time-0800 / time-1000;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>        
                {% endif %}   
            {% endfor %}                  
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'LocXR' %}
                    <div class="session session-w4a track-blue" style="grid-column: track-4; grid-row: time-0800 / time-1000;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}    
            {% endfor %}                  
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'KELVAR' %}
                    <div class="session session-w5a track-blue" style="grid-column: track-5; grid-row: time-0800 / time-1000;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}     
            {% endfor %}                            
            {% for workshop in site.data.workshops %}    
                {% if workshop.id == 'IDEATExR' %}
                    <div class="session session-w6a track-blue" style="grid-column: track-6; grid-row: time-0800 / time-1000;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}     
            {% endfor %}               
            <p class="time-slot" style="grid-row: time-0830;">8:30</p>    
            {% for tutorial in site.data.tutorials %}  
                {% if tutorial.id == 'T1' %}
                    <div class="session session-t1a track-tutorials" style="grid-column: track-7; grid-row: time-0830 / time-1000;">                    
                        <h3 class="session-title">Tutorial<br /><a href="{{ '/program/tutorials/' | relative_url }}#{{ tutorial.id }}">{{ tutorial.title }}</a></h3><br/>
                        <span class="session-time">8:30-10:00</span>
                        <span class="session-presenter">{{ tutorial.authors }}</span>
                    </div>
                {% endif %}   
            {% endfor %}     
            <p class="time-slot" style="grid-row: time-1000;">10:00</p>
            <div class="session session-16 track-all" style="grid-column:  track-1-start / track-7-end; grid-row: time-1000 / time-1030;">
                <h3 class="session-title">Break: 10:00-10:30 (Catered)</h3>
            </div>   
             <p class="time-slot" style="grid-row: time-1030;">10:30</p>             
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'XRGaming' %}
                    <div class="session session-w1b track-blue" style="grid-column: track-1; grid-row: time-1030 / time-1200;">                    
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}   
            {% endfor %}           
            {% for workshop in site.data.workshops %}   
                {% if workshop.id == 'WSR' %}
                    <div class="session session-w2b track-blue" style="grid-column: track-2; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>         
                {% endif %}     
            {% endfor %}                  
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'XRIOS' %}
                    <div class="session session-w3b track-blue" style="grid-column: track-3; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>        
                {% endif %}   
            {% endfor %}                  
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'LocXR' %}
                    <div class="session session-w4b track-blue" style="grid-column: track-4; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}    
            {% endfor %}                  
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'KELVAR' %}
                    <div class="session session-w5b track-blue" style="grid-column: track-5; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}     
            {% endfor %}                            
            {% for workshop in site.data.workshops %}    
                {% if workshop.id == 'IDEATExR' %}
                    <div class="session session-w6b track-blue" style="grid-column: track-6; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}     
            {% endfor %}              
             {% for tutorial in site.data.tutorials %}  
                {% if tutorial.id == 'T1' %}
                    <div class="session session-t1b track-tutorials" style="grid-column: track-7; grid-row: time-1030 / time-1200;">                    
                        <h3 class="session-title">Tutorial (cont)<br /><a href="{{ '/program/tutorials/' | relative_url }}#{{ tutorial.id }}">{{ tutorial.title }}</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ tutorial.authors }}</span>
                    </div>
                {% endif %}   
            {% endfor %}               
            <p class="time-slot" style="grid-row: time-1200;">12:00</p> 
            <div class="session session-lunch track-all" style="grid-column: track-1-start / track-7-end; grid-row: time-1200 / time-1330;">
                <h3 class="session-title">Lunch: 12:00-13:30 (Not Catered)</h3>
            </div>            
            <p class="time-slot" style="grid-row: time-1330;">13:30</p>   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'WISP' %}
                    <div class="session session-7a track-blue" style="grid-column: track-1; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>            
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'GEMINI' %}
                    <div class="session session-8a track-blue" style="grid-column: track-2; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>              
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'VHCIE' %}
                    <div class="session session-9a track-blue" style="grid-column: track-3; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>            
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'CLEVER' %}
                    <div class="session session-10a track-blue" style="grid-column: track-4; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'ENPTXR' %}
                    <div class="session session-11a track-blue" style="grid-column: track-5; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'IDEATExR' %}
                    <div class="session session-6c track-blue" style="grid-column: track-6; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}       
            {% endfor %}   
            <p class="time-slot" style="grid-row: time-1530;">15:30</p>
            <div class="session session-16 track-all" style="grid-column:  track-1-start / track-7-end; grid-row: time-1530 / time-1600;">
                <h3 class="session-title">Break: 15:30-16:00 (Catered)</h3>
            </div>    
            <p class="time-slot" style="grid-row: time-1600;">16:00</p>   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'WISP' %}
                    <div class="session session-7b track-blue" style="grid-column: track-1; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>            
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'GEMINI' %}
                    <div class="session session-8b track-blue" style="grid-column: track-2; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>              
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'VHCIE' %}
                    <div class="session session-9b track-blue" style="grid-column: track-3; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>            
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'CLEVER' %}
                    <div class="session session-10b track-blue" style="grid-column: track-4; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'ENPTXR' %}
                    <div class="session session-11b track-blue" style="grid-column: track-5; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}     
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'IDEATExR' %}
                    <div class="session session-6d track-blue" style="grid-column: track-6; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}       
            {% endfor %}                      
             {% for tutorial in site.data.tutorials %}  
                {% if tutorial.id == 'T2' %}
                    <div class="session session-t2a track-tutorials" style="grid-column: track-7; grid-row: time-1600 / time-1730;">                    
                        <h3 class="session-title">Tutorial<br /><a href="{{ '/program/tutorials/' | relative_url }}#{{ tutorial.id }}">{{ tutorial.title }}</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ tutorial.authors }}</span>
                    </div>
                {% endif %}   
            {% endfor %}  
        </div> 
    </div>
    <div>
        <h4 id="day2">Sunday, 17 March 2024</h4> 
        <div class="schedule-sun" aria-labelledby="Sunday, 17 March 2024Workshop Schedule"> 
            <p class="time-slot" style="grid-row: time-0800;">8:00</p>
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'MASSXR' %}
                    <div class="session session-w12a track-blue" style="grid-column: track-1; grid-row: time-0800 / time-1000;">                        
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %} 
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'IVL' %}
                    <div class="session session-w13a track-blue" style="grid-column: track-2; grid-row: time-0800 / time-1000;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>         
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'ReDigiTS' %}
                    <div class="session session-w14a track-blue" style="grid-column: track-3; grid-row: time-0800 / time-1000;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>        
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'NIDIT' %}
                    <div class="session session-w15a track-blue" style="grid-column: track-4; grid-row: time-0800 / time-1000;"> 
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'Data4XR' %}
                    <div class="session session-w16a track-blue" style="grid-column: track-5; grid-row: time-0800 / time-1000;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}  
            {% for workshop in site.data.workshops %}   
                {% if workshop.id == 'PANDAS' %}
                    <div class="session session-w17a track-blue" style="grid-column: track-6; grid-row: time-0800 / time-1000;">                   
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">8:00-10:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}                          
             {% for tutorial in site.data.tutorials %}  
                {% if tutorial.id == 'T3' %}
                    <div class="session session-t3a track-tutorials" style="grid-column: track-8; grid-row: time-0830 / time-1000;">                    
                        <h3 class="session-title">Tutorial<br /><a href="{{ '/program/tutorials/' | relative_url }}#{{ tutorial.id }}">{{ tutorial.title }}</a></h3><br/>
                        <span class="session-time">8:30-10:00</span>
                        <span class="session-presenter">{{ tutorial.authors }}</span>
                    </div>
                {% endif %}   
            {% endfor %}                  
             <div class="session session-f31 track-f3" style="grid-column: track-7; grid-row: time-0830 / time-0845;">                        
                <h3 class="session-title"><a href="{{ '/program/future-faculty-forum/' | relative_url }}">Future Faculty Forum (F3)</a></h3>
            </div>    
            <p class="time-slot" style="grid-row: time-0845;">8:45</p>         
            <div class="session session-f32 track-f3" style="grid-column: track-7; grid-row: time-0845 / time-0900;">                        
                <h3 class="session-title"><a href="{{ '/program/future-faculty-forum/' | relative_url }}">F3</a> | Welcome & Opening Remarks</h3>
                <span class="session-time">8:45-9:00</span>
            </div>                
            <p class="time-slot" style="grid-row: time-0900;">9:00</p>           
            <div class="session session-f33 track-f3" style="grid-column: track-7; grid-row: time-0900 / time-1000;">  
                <h3 class="session-title"><a href="{{ '/program/future-faculty-forum/' | relative_url }}">F3</a> | Tutorial: Professor Application Process</h3>                      
                <span class="session-time">9:00-10:00</span>
            </div>            
            <p class="time-slot" style="grid-row: time-1000;">10:00</p>
            <div class="session session-b track-all" style="grid-column:  track-1-start / track-8-end; grid-row: time-1000 / time-1030;">
                <h3 class="session-title">Break: 10:00-10:30 (Catered)</h3>
            </div> 
            <p class="time-slot" style="grid-row: time-1030;">10:30</p>
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'MASSXR' %}
                    <div class="session session-w12b track-blue" style="grid-column: track-1; grid-row: time-1030 / time-1200;">                        
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %} 
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'IVL' %}
                    <div class="session session-w13b track-blue" style="grid-column: track-2; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>         
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'ReDigiTS' %}
                    <div class="session session-w14b track-blue" style="grid-column: track-3; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>        
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'NIDIT' %}
                    <div class="session session-w15b track-blue" style="grid-column: track-4; grid-row: time-1030 / time-1200;"> 
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'Data4XR' %}
                    <div class="session session-w16b track-blue" style="grid-column: track-5; grid-row: time-1030 / time-1200;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}  
            {% for workshop in site.data.workshops %}   
                {% if workshop.id == 'PANDAS' %}
                    <div class="session session-w17b track-blue" style="grid-column: track-6; grid-row: time-1030 / time-1200;">                   
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}                          
            {% for tutorial in site.data.tutorials %}  
                {% if tutorial.id == 'T3' %}
                    <div class="session session-t3b track-tutorials" style="grid-column: track-8; grid-row: time-1030 / time-1200;">                    
                        <h3 class="session-title">Tutorial (cont)<br /><a href="{{ '/program/tutorials/' | relative_url }}#{{ tutorial.id }}">{{ tutorial.title }}</a></h3><br/>
                        <span class="session-time">10:30-12:00</span>
                        <span class="session-presenter">{{ tutorial.authors }}</span>
                    </div>
                {% endif %}   
            {% endfor %}   
            <div class="session session-f34 track-f3" style="grid-column: track-7; grid-row: time-1030 / time-1115;">                        
                <h3 class="session-title"><a href="{{ '/program/future-faculty-forum/' | relative_url }}">F3</a> | Panel 1: Differences in Universities (Geo, Research vs. Teaching Alloc.)</h3>
                <span class="session-time">10:30-11:15</span>
            </div>      
            <p class="time-slot" style="grid-row: time-1115;">11:15</p>          
            <div class="session session-f35 track-f3" style="grid-column: track-7; grid-row: time-1115 / time-1200;">                        
                <h3 class="session-title"><a href="{{ '/program/future-faculty-forum/' | relative_url }}">F3</a> | Panel 2: Lab Formation & Management</h3>
                <span class="session-time">11:15-12:00</span>
            </div>   
            <p class="time-slot" style="grid-row: time-1200;">12:00</p>
            <div class="session session-l track-all" style="grid-column: track-1-start / track-8-end; grid-row: time-1200 / time-1330;">
                <h3 class="session-title">Lunch: 12:00-13:30 (Not Catered)</h3>
            </div>             
            <p class="time-slot" style="grid-row: time-1330;">13:30</p>             
            {% for workshop in site.data.workshops %} 
                {% if workshop.id == 'AVR' %}
                    <div class="session session-8 track-blue" style="grid-column: track-1; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>            
                {% endif %}      
            {% endfor %}  
            {% for workshop in site.data.workshops %}   
                {% if workshop.id == 'OAT' %}
                    <div class="session session-9 track-blue" style="grid-column: track-2; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>              
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'TrainingXR' %}
                    <div class="session session-10 track-blue" style="grid-column: track-3; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>            
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'NIDIT' %}
                    <div class="session session-11 track-blue" style="grid-column: track-4; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}  
            {% for workshop in site.data.workshops %}   
                {% if workshop.id == 'xrWORKS' %}
                    <div class="session session-12 track-blue" style="grid-column: track-5; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'ANIVAE' %}
                    <div class="session session-13 track-blue" style="grid-column: track-6; grid-row: time-1330 / time-1530;">
                        <h3 class="session-title">Workshop<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">13:30-15:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}       
            {% endfor %}           
            <div class="session session-19 track-f3" style="grid-column: track-7; grid-row: time-1330 / time-1415;">                  
                <h3 class="session-title"><a href="{{ '/program/future-faculty-forum/' | relative_url }}">F3</a> | Panel 3: Challenges & Opportunities&nbsp;of Interdisciplinary Research</h3>
                <span class="session-time">13:30-14:15</span>
            </div>  
            <p class="time-slot" style="grid-row: time-1400;">14:00</p> 
            {% for tutorial in site.data.tutorials %}  
                {% if tutorial.id == 'T4' %}
                    <div class="session session-t3b track-tutorials" style="grid-column: track-8; grid-row: time-1400 / time-1530;">                    
                        <h3 class="session-title">Tutorial<br /><a href="{{ '/program/tutorials/' | relative_url }}#{{ tutorial.id }}">{{ tutorial.title }}</a></h3><br/>
                        <span class="session-time">14:00-15:30</span>
                        <span class="session-presenter">{{ tutorial.authors }}</span>
                    </div>
                {% endif %}   
            {% endfor %}  
            <p class="time-slot" style="grid-row: time-1415;">14:15</p>          
            <div class="session session-20 track-f3" style="grid-column: track-7; grid-row: time-1415 / time-1530;">                        
                <h3 class="session-title"><a href="{{ '/program/future-faculty-forum/' | relative_url }}">F3</a> | Tutorial: Review & Critique of Application Materials (Research, Teaching & Diversity Statements)</h3>
                <span class="session-time">14:15-15:30</span>
            </div>
            <p class="time-slot" style="grid-row: time-1530;">15:30</p>
            <div class="session session-16 track-all" style="grid-column: track-1 / track-8; grid-row: time-1530 / time-1600;">
                <h3 class="session-title">Break: 15:30-16:00 (Catered)</h3>
            </div>  
            <p class="time-slot" style="grid-row: time-1600;">16:00</p>
            {% for workshop in site.data.workshops %} 
                {% if workshop.id == 'AVR' %}
                    <div class="session session-8 track-blue" style="grid-column: track-1; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>            
                {% endif %}      
            {% endfor %}  
            {% for workshop in site.data.workshops %}   
                {% if workshop.id == 'OAT' %}
                    <div class="session session-9 track-blue" style="grid-column: track-2; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>              
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'TrainingXR' %}
                    <div class="session session-10 track-blue" style="grid-column: track-3; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>            
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'NIDIT' %}
                    <div class="session session-11 track-blue" style="grid-column: track-4; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}  
            {% for workshop in site.data.workshops %}   
                {% if workshop.id == 'xrWORKS' %}
                    <div class="session session-12 track-blue" style="grid-column: track-5; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}      
            {% endfor %}   
            {% for workshop in site.data.workshops %}  
                {% if workshop.id == 'ANIVAE' %}
                    <div class="session session-13 track-blue" style="grid-column: track-6; grid-row: time-1600 / time-1730;">
                        <h3 class="session-title">Workshop (cont)<br/><a href="{{ '/program/workshop/' | relative_url }}#{{ workshop.id }}">{{ workshop.title }} ({{ workshop.id }})</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ workshop.organiser }}</span>
                    </div>
                {% endif %}       
            {% endfor %}          
            <div class="session session-22 track-f3" style="grid-column: track-7; grid-row: time-1600 / time-1645;">                        
                <h3 class="session-title"><a href="{{ '/program/future-faculty-forum/' | relative_url }}">F3</a> | Speed Advising</h3>
                <span class="session-time">16:00-16:45</span>
            </div>       
            {% for tutorial in site.data.tutorials %}  
                {% if tutorial.id == 'T5' %}
                    <div class="session session-t3b track-tutorials" style="grid-column: track-8; grid-row: time-1600 / time-1730;">                    
                        <h3 class="session-title">Tutorial<br /><a href="{{ '/program/tutorials/' | relative_url }}#{{ tutorial.id }}">{{ tutorial.title }}</a></h3><br/>
                        <span class="session-time">16:00-17:30</span>
                        <span class="session-presenter">{{ tutorial.authors }}</span>
                    </div>
                {% endif %}   
            {% endfor %}     
            <p class="time-slot" style="grid-row: time-1645;">16:45</p>   
            <div class="session session-23 track-f3" style="grid-column: track-7; grid-row: time-1645 / time-1700;">                        
                <h3 class="session-title"><a href="{{ '/program/future-faculty-forum/' | relative_url }}">F3</a> | Closing Remarks & Feedback for Future F3 Events</h3>
                <span class="session-time">16:45-17:00</span>
            </div> 
        </div> 
    </div> 
    <div>
        <h4 id="day3">Monday, 18 March 2024</h4>
        <div class="schedule-mon" aria-labelledby="Monday, 18 March 2024-Main Conference"> 
            <p class="time-slot" style="grid-row: time-0830;">8:30</p>
            <div class="session track-green" style="grid-column: track-1-start / track-3-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Opening & Awards</h3>
                <span class="session-time">8:30-9:45</span>
            </div>            
            <p class="time-slot" style="grid-row: time-0945;">9:45</p>
            <div class="session track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-0945 / time-1015;">
                <h3 class="session-title">Break: 9:45-10:15 (Catered)</h3>
            </div> 
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-0945 / time-1015;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">9:45-10:00</span>
            </div>                         
            <p class="time-slot" style="grid-row: time-1015;">10:15</p>
            <div class="session track-keynote" style="grid-column: track-1-start / track-3-end; grid-row: time-1015 / time-1115;">
                <h3 class="session-title">Keynote Speaker<br/><a href="{{ '/program/keynote-speakers/' | relative_url }}#keynote-azenkot">Prof. Shiri Azenkot</a></h3>                
                <span class="session-title"><a href="{{ '/program/keynote-speakers/' | relative_url }}#keynote-azenkot">XR Access: Making Virtual and Augmented Reality Accessible to People with Disabilities</a></span>
                <span class="session-time">10:15-11:15</span>                
            </div> 
            <p class="time-slot" style="grid-row: time-1115;">11:15</p>  
            <div class="session track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1115 / time-1130;">
                <h3 class="session-title">Stretch Break (Not Catered): 11:15-11:30</h3>
            </div>             
            <p class="time-slot" style="grid-row: time-1130;">11:30</p>
            <div class="session track-special-session" style="grid-column: track-1-start / track-3-end; grid-row: time-1130 / time-1230;">
                <h3 class="session-title">Special Session</h3>
                <h3 class="session-title">VR for All: Achieving Longterm DEIA Success in the VR Community</h3>
                <span class="session-time">11:30-12:30</span>
            </div>             
            <p class="time-slot" style="grid-row: time-1230;">12:30</p>
            <div class="session track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1230 / time-1330;">
                <h3 class="session-title">Lunch: 12:30-13:30 (Not Catered)</h3>
            </div>  
            <p class="time-slot" style="grid-row: time-1300;">13:00</p>
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-1300 / time-1330;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">13:00-13:30</span>
            </div>                        
            <p class="time-slot" style="grid-row: time-1330;">13:30</p>  
            <div class="session track-demos" style="grid-column: track-1-start / track-3-end; grid-row: time-1330 / time-1400;">
                <h3 class="session-title">Research Demos and 3DUI Contest Fast Forward</h3>
                <span class="session-time">13:30-14:00</span>
            </div>  
            <p class="time-slot" style="grid-row: time-1400;">14:00</p>
            <div class="session track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1400 / time-1500;">
                <h3 class="session-title">Papers 41</h3>
                <span class="session-time">14:00-15:00</span>
            </div>  
            <div class="session track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1400 / time-1500;">
                <h3 class="session-title">Papers 45</h3>
                <span class="session-time">14:00-15:00</span>
            </div>  
            <div class="session track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1400 / time-1500;">
                <h3 class="session-title">Papers 46</h3>
                <span class="session-time">14:00-15:00</span>
            </div> 
            <p class="time-slot" style="grid-row: time-1500;">15:00</p>
            <div class="session track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1500 / time-1530;">
                <h3 class="session-title">Break: 15:00-15:30 (Catered)</h3>
            </div>    
            <div class="session session-6 track-pd3dui" style="grid-column: track-4-start; grid-row: time-1500 / time-1530;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">15:00-15:30</span>
            </div>  
            <p class="time-slot" style="grid-row: time-1530;">15:30</p> 
            <div class="session track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1530 / time-1700;">
                <h3 class="session-title">Papers 15</h3>
                <span class="session-time">15:30-17:00</span>
            </div>  
            <div class="session track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1530 / time-1700;">
                <h3 class="session-title">Papers 30</h3>
                <span class="session-time">15:30-17:00</span>
            </div>  
            <div class="session track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1530 / time-1700;">
                <h3 class="session-title">Papers 33</h3>
                <span class="session-time">15:30-17:00</span>
            </div>  
            <p class="time-slot" style="grid-row: time-1700;">17:00</p>                
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-1700 / time-1730;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">17:00-17:30</span>
            </div>
            <p class="time-slot" style="grid-row: time-1730;">17:30</p> 
            <div class="session track-green" style="grid-column: track-1-start / track-3-end; grid-row: time-1730 / time-1900;">
                <h3 class="session-title">Welcome Reception</h3>
                <span class="session-time">17:30-19:00</span>
            </div>  
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-1730 / time-1900;">
                <h3 class="session-title">Research Demos & 3DUI Contest</h3>
                <span class="session-time">17:30-19:00</span>
            </div>
        </div> 
    </div>
    <div>
        <h4 id="day4">Tuesday, 19 March 2024</h4>
        <div class="schedule-tue" aria-labelledby="Tuesday, 19 March 2024-Main Conference"> 
            <p class="time-slot" style="grid-row: time-0830;">8:30</p>          
            <div class="session track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Papers 7</h3>
                <span class="session-time">8:30-9:45</span>
            </div> 
            <div class="session track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Papers 8</h3>
                <span class="session-time">8:30-9:45</span>
            </div> 
            <div class="session track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Papers 19</h3>
                <span class="session-time">8:30-9:45</span>
            </div> 
            <p class="time-slot" style="grid-row: time-0945;">9:45</p>  
            <div class="session track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-0945 / time-1015;">
                <h3 class="session-title">Break: 9:45-10:15 (Catered)</h3>
            </div> 
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-0945 / time-1015;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">9:45-10:00</span>
            </div>     
            <p class="time-slot" style="grid-row: time-1015;">10:15</p>            
             <div class="session track-keynote" style="grid-column: track-1-start / track-3-end; grid-row: time-1015 / time-1115;">
                <h3 class="session-title">Keynote Speaker<br/><a href="{{ '/program/keynote-speakers/' | relative_url }}#keynote-tschanz">Michael Tschanz</a></h3>                
                <span class="session-title"><a href="{{ '/program/keynote-speakers/' | relative_url }}#keynote-tschanz">Disney's Industrial Controls Design and Data Analytics Ecosystem</a></span>
                <span class="session-time">10:15-11:15</span>                
            </div> 
            <p class="time-slot" style="grid-row: time-1115;">11:15</p>  
            <div class="session track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1115 / time-1130;">
                <h3 class="session-title">Stretch Break (Not Catered): 11:15-11:30</h3>
            </div> 
            <p class="time-slot" style="grid-row: time-1130;">11:30</p>
            <div class="session track-special-session" style="grid-column: track-1-start / track-3-end; grid-row: time-1130 / time-1230;">
                <h3 class="session-title">Special Session</h3>
                <h3 class="session-title">The Reviewing Crisis</h3>
                <span class="session-time">11:30-12:30</span>
            </div> 
            <p class="time-slot" style="grid-row: time-1230;">12:30</p>
            <div class="session track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1230 / time-1330;">
                <h3 class="session-title">Lunch: 12:30-13:30 (Not Catered)</h3>
            </div>  
            <p class="time-slot" style="grid-row: time-1300;">13:00</p>
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-1300 / time-1330;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">13:00-13:30</span>
            </div>   
            <p class="time-slot" style="grid-row: time-1330;">13:30</p>
            <div class="session track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1330 / time-1500;">
                <h3 class="session-title">Papers 43</h3>
                <span class="session-time">13:30-15:00</span>
            </div>  
            <div class="session track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1330 / time-1500;">
                <h3 class="session-title">Papers 1</h3>
                <span class="session-time">13:30-15:00</span>
            </div>  
            <div class="session track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1330 / time-1500;">
                <h3 class="session-title">Papers 5</h3>
                <span class="session-time">13:30-15:00</span>
            </div> 
            <p class="time-slot" style="grid-row: time-1500;">15:00</p>
            <div class="session track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1500 / time-1530;">
                <h3 class="session-title">Break: 15:00-15:30 (Catered)</h3>
            </div>    
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-1500 / time-1530;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">15:00-15:30</span>
            </div>   
            <p class="time-slot" style="grid-row: time-1530;">15:30</p>  
            <div class="session track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1530 / time-1700;">
                <h3 class="session-title">Papers 6</h3>
                <span class="session-time">15:30-17:00</span>
            </div>  
            <div class="session track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1530 / time-1700;">
                <h3 class="session-title">Papers 36</h3>
                <span class="session-time">15:30-17:00</span>
            </div>  
            <div class="session track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1530 / time-1700;">
                <h3 class="session-title">Papers 27</h3>
                <span class="session-time">15:30-17:00</span>
            </div>  
            <p class="time-slot" style="grid-row: time-1700;">17:00</p>                
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-1700 / time-1730;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">17:00-17:30</span>
            </div>
        </div> 
    </div>
    <div>
        <h4 id="day5">Wednesday, 20 March 2024</h4>
        <div class="schedule-wed" aria-labelledby="March 20-Main Conference"> 
            <p class="time-slot" style="grid-row: time-0830;">8:30</p>            
            <div class="session session-1 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Papers 23</h3>
                <span class="session-time">8:30-9:45</span>
            </div>  
            <div class="session session-2 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Papers 24</h3>
                <span class="session-time">8:30-9:45</span>
            </div>  
            <div class="session session-3 track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Papers 25</h3>
                <span class="session-time">8:30-9:45</span>
            </div>   
            <p class="time-slot" style="grid-row: time-0945;">9:45</p>
            <div class="session session-4 track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-0945 / time-1015;">
                <h3 class="session-title">Break: 9:45-10:15</h3>
            </div>  
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-0945 / time-1015;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">9:45-10:00</span>
            </div>   
            <p class="time-slot" style="grid-row: time-1015;">10:15</p>
           <div class="session session-1 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1015 / time-1115;">
                <h3 class="session-title">Papers 3</h3>
                <span class="session-time">10:15-11:15</span>
            </div>  
            <div class="session session-2 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1015 / time-1115;">
                <h3 class="session-title">Papers 4</h3>
                <span class="session-time">10:15-11:15</span>
            </div>  
            <div class="session session-3 track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1015 / time-1115;">
                <h3 class="session-title">Papers 10</h3>
                <span class="session-time">10:15-11:15</span>
            </div>   
            <p class="time-slot" style="grid-row: time-1115;">11:15</p>
            <div class="session session-6 track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1115 / time-1130;">
                <h3 class="session-title">Stretch Break (Not Catered): 11:15-11:30</h3>
            </div> 
            <p class="time-slot" style="grid-row: time-1130;">11:30</p>
            <div class="session session-1 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1130 / time-1230;">
                <h3 class="session-title">Papers 20</h3>
                <span class="session-time">11:30-12:30</span>
            </div>  
            <div class="session session-2 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1130 / time-1230;">
                <h3 class="session-title">Papers 21</h3>
                <span class="session-time">11:30-12:30</span>
            </div>  
            <div class="session session-3 track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1130 / time-1230;">
                <h3 class="session-title">Papers 22</h3>
                <span class="session-time">11:30-12:30</span>
            </div> 
            <p class="time-slot" style="grid-row: time-1230;">12:30</p>
            <div class="session session-8 track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1230 / time-1330;">
                <h3 class="session-title">Lunch: 12:30-13:30 (Not Catered)</h3>
            </div> 
            <p class="time-slot" style="grid-row: time-1300;">13:00</p>
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-1300 / time-1330;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">13:00-13:30</span>
            </div> 
            <p class="time-slot" style="grid-row: time-1330;">13:30</p>
            <div class="session session-9 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1330 / time-1500;">
                <h3 class="session-title">Papers 34</h3>
                <span class="session-time">13:30-15:00</span>
            </div>  
            <div class="session session-10 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1330 / time-1500;">
                <h3 class="session-title">Papers 11</h3>
                <span class="session-time">13:30-15:00</span>
            </div>  
            <div class="session session-11 track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1330 / time-1500;">
                <h3 class="session-title">Papers 42</h3>
                <span class="session-time">13:30-15:00</span>
            </div> 
            <p class="time-slot" style="grid-row: time-1500;">15:00</p> 
            <div class="session session-12 track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1500 / time-1530;">
                <h3 class="session-title">Break: 15:00-15:30 (Catered)</h3>
            </div>     
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-1500 / time-1530;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">15:00-15:30</span>
            </div> 
            <p class="time-slot" style="grid-row: time-1700;">17:00</p>                
            <div class="session track-pd3dui" style="grid-column: track-4-start; grid-row: time-1700 / time-1730;">
                <h3 class="session-title">Posters, Research Demos & 3DUI Contest</h3>
                <span class="session-time">17:00-17:30</span>
            </div> 
            <p class="time-slot" style="grid-row: time-1800;">18:00</p>                
            <div class="session track-green" style="grid-column: track-1-start / track-3-end; grid-row: time-1800 / time-2100;">
                <h3 class="session-title">Conference Banquet with Keynote Speaker</h3>
                <span class="session-title"><a href="{{ '/program/keynote-speakers/' | relative_url }}#keynote-richir">Prof. Simon Richir</a></span>
                <span class="session-title"><a href="{{ '/program/keynote-speakers/' | relative_url }}#keynote-richir">The Laval Phenomenon: A Deep Dive into France's VR Capital</a></span>
                <span class="session-time">18:00-21:00</span>
                <span class="session-track">Fantasia Ballroom</span>
            </div>            
        </div> 
    </div>
    <div>
        <h4 id="day6">Thursday, 21 March 2024</h4>
        <div class="schedule-thu" aria-labelledby="Thursday, 21 March 2024-Main Conference"> 
            <p class="time-slot" style="grid-row: time-0830;">8:30</p>         
            <div class="session session-1 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Papers 29</h3>
                <span class="session-time">8:30-9:45</span>
            </div>   
            <div class="session session-2 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Papers 32</h3>
                <span class="session-time">8:30-9:45</span>
            </div>  
            <div class="session session-3 track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-0830 / time-0945;">
                <h3 class="session-title">Papers 37</h3>
                <span class="session-time">8:30-9:45</span>
            </div> 
            <p class="time-slot" style="grid-row: time-0945;">9:45</p>  
            <div class="session session-4 track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-0945 / time-1015;">
                <h3 class="session-title">Break: 9:45-10:15 (Catered)</h3>
            </div>  
            <p class="time-slot" style="grid-row: time-1015;">10:15</p>
           <div class="session session-1 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1015 / time-1115;">
                <h3 class="session-title">Papers 12</h3>
                <span class="session-time">10:15-11:15</span>
            </div>  
            <div class="session session-2 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1015 / time-1115;">
                <h3 class="session-title">Papers 13</h3>
                <span class="session-time">10:15-11:15</span>
            </div>  
            <div class="session session-3 track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1015 / time-1115;">
                <h3 class="session-title">Papers 18</h3>
                <span class="session-time">10:15-11:15</span>
            </div>  
            <p class="time-slot" style="grid-row: time-1115;">11:15</p>
            <div class="session session-6 track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1115 / time-1130;">
                <h3 class="session-title">Stretch Break (Not Catered): 11:15-11:30</h3>
            </div> 
            <p class="time-slot" style="grid-row: time-1130;">11:30</p> 
            <div class="session session-1 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1130 / time-1230;">
                <h3 class="session-title">Papers 28</h3>
                <span class="session-time">11:30-12:30</span>
            </div>  
            <div class="session session-2 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1130 / time-1230;">
                <h3 class="session-title">Papers 38</h3>
                <span class="session-time">11:30-12:30</span>
            </div>  
            <div class="session session-3 track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1130 / time-1230;">
                <h3 class="session-title">Papers 40</h3>
                <span class="session-time">11:30-12:30</span>
            </div> 
            <p class="time-slot" style="grid-row: time-1230;">12:30</p>
            <div class="session session-8 track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1230 / time-1330;">
                <h3 class="session-title">Lunch: 12:30-13:30 (Not Catered)</h3>
            </div> 
            <p class="time-slot" style="grid-row: time-1330;">13:30</p>
            <div class="session session-9 track-papers" style="grid-column: track-1-start / track-1-end; grid-row: time-1330 / time-1500;">
                <h3 class="session-title">Papers 14</h3>
                <span class="session-time">13:30-15:00</span>
            </div>  
            <div class="session session-10 track-papers" style="grid-column: track-2-start / track-2-end; grid-row: time-1330 / time-1500;">
                <h3 class="session-title">Papers 16</h3>
                <span class="session-time">13:30-15:00</span>
            </div>  
            <div class="session session-11 track-papers" style="grid-column: track-3-start / track-3-end; grid-row: time-1330 / time-1500;">
                <h3 class="session-title">Papers 26</h3>
                <span class="session-time">13:30-15:00</span>
            </div>
            <p class="time-slot" style="grid-row: time-1500;">15:00</p>  
            <div class="session session-12 track-all" style="grid-column: track-1-start / track-3-end; grid-row: time-1500 / time-1530;">
                <h3 class="session-title">Break: 15:00-15:30 (Catered)</h3>
            </div>  
            <p class="time-slot" style="grid-row: time-1530;">15:30</p>   
            <div class="session session-11 track-green" style="grid-column: track-1-start / track-3-end; grid-row: time-1530 / time-1700;">
                <h3 class="session-title">Closing & Awards</h3>
                <span class="session-time">15:30-17:00</span>
            </div>            
        </div> 
    </div>
</div>