---
layout: ieeevr-default
title: "Registration"
subtitle: "IEEE VR 2024"
title_separator: "|"
---
<script type="text/javascript">
    $( function() {
        $( "#accordion" ).accordion({
        	collapsible: true,
			heightStyle: "content",
			header: "h4"
        });
    } );

    $(document).ready(function(){
		var email = ""; 
		var domain = "ieeevr.org"; 
		var domain_ieee = "computer.org"; 

		email = "program2024"; 		
		$(".program").html("<span class='text-nowrap'><a href=javascript:location='" + "mail" + "to:" + email + "@" + domain + "'><i class='fas fa-fw fa-envelope-square emailIconSm' style=''></i><i class='emailTextSm'>" + email + "@" + domain + "</a></i></span>");   
	
	    email = "general2024"; 		
		$(".general").html("<span class='text-nowrap'><a href=javascript:location='" + "mail" + "to:" + email + "@" + domain + "'><i class='fas fa-fw fa-envelope-square emailIconSm' style=''></i><i class='emailTextSm'>" + email + "@" + domain + "</a></i></span>");  
		
	    email = "registration+VR"; 		
		$(".registration").html("<span class='text-nowrap'><a href=javascript:location='" + "mail" + "to:" + email + "@" + domain_ieee + "'><i class='fas fa-fw fa-envelope-square emailIconSm' style=''></i><i class='emailTextSm'>" + email + "@" + domain_ieee + "</a></i></span>");          

		email = "register2024"; 		
		register.innerHTML  = "<span class='text-nowrap'><a href=javascript:location='" + "mail" + "to:" + email + "@" + domain + "'><i class='fas fa-fw fa-envelope-square emailIconSm' style=''></i><i class='emailTextSm'>" + email + "@" + domain + "</a></i></span>";  

	});
</script>
<style>
 /*************************
    * Accordian Styling
    *************************/ 
    .ui-state-active,
    .ui-widget-content .ui-state-active,
    .ui-widget-header .ui-state-active,
    a.ui-button:active,
    .ui-button:active,
    .ui-button.ui-state-active:hover {
        border: 1px solid #12a6c9;
        background: #12a6c9;
        font-weight: normal;
        color: #ffffff;
    }
    .ui-icon-background,
    .ui-state-active .ui-icon-background {
        border: #12a6c9;
        background-color: #ffffff;
    }
</style>
<h1 id="registration">Registration  <div class="floatRight"><span id="register"></span></div></h1>
<p>
	<strong style="color: black">IEEE VR 2024: the 31<sup>st</sup> IEEE Conference on Virtual Reality and 3D User Interfaces</strong><br /> 
	March 16-21, 2024 | Orlando, Florida USA
</p>

<p class="alignCenter">
	<a href="https://services10.ieee.org/as/authorization.oauth2?response_type=code&client_id=PF_AS_FOR_PA&redirect_uri=https%3A%2F%2Fservices16.ieee.org%2Fpa%2Foidc%2Fcb&state=eyJ6aXAiOiJERUYiLCJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2Iiwia2lkIjoiMnMiLCJzdWZmaXgiOiJuenV2c0YuMTcwNDY1ODAyMCJ9..q_dFVfhhl3vkCVRojhpOZA.1AWYBbEEjsZ6X6v_ihgJkWbYLxI5BbNYFITc1iV2qnddfiH-ll5JEeD8aWEMUz6Z8-uSO6-eEyUwgQU6SEdJKA1wy84NgEdL8pLDODCiodNhEPhEc6F3gfnz-BjIOBtwRan75Jvis_rnTfREW7LdTC8UgvDFCbJg8p7h0oye5WnAeBeMwzacY8j4lZhk6yCRCXtvxACYeY-Q3IcEWl3YVjuJi03Wjn73VtPwJmqFA4O8XXoPFD_WdelUiLs4ns93odCE6vxacFF0laptAhBBodBd4zrAbkQMsj7XaYJ7T4sMs8yghGrNyhYqIMavy6_vS03mgkVIIIy1OJICBf9Fkcllhj1pPdz-x8kqLqbyUgs.At6CM33Tw2rNjpwG1O9aPg&nonce=GsPERIKhJhNdopM_5XiRw4YU_7HS6LzvtidwaC-S2rA&acr_values=stm%20sts%20prf%20crt%20msp%20col%20otk%20cmc%20cmp%20spe&scope=openid%20profile%20address%20email%20phone&vnd_pi_requested_resource=https%3A%2F%2Fservices16.ieee.org%2Fccs%3Fcvent_url%3Dhttps%3A%2F%2Fcvent.me%2F7Eg4zQ%26reg_code%3DH%2CLF%2CLM%2CLS%2CGSM%2CStM%2CC016%2CSM%2CAM%2CF%2CM%26account_type%3DMCE%26e%3D88db5352-a5af-4db9-ab08-f18f7d191ade%26TARGET%3Dhttps%253A%252F%252Fweb.cvent.com%252Fevent%252F88db5352-a5af-4db9-ab08-f18f7d191ade%252Fregister%253FRefId%253DMember%2526rp%253D0de61eb8-a37d-4c24-8e84-924449030b8e&vnd_pi_application_name=CVENT_CCS" class="btn registration_button" style="" target="_blank">IEEE Member Registration</a>
	<a href="https://web.cvent.com/event/88db5352-a5af-4db9-ab08-f18f7d191ade/regPage:3d64a89a-bbcd-48df-af2b-3bcd0a58ae90?RefId=Non-Member&rp=c6b95094-fb90-4bbb-af7b-67e7d743a184" class="btn registration_button" style="" target="_blank">IEEE Non-Member Registration</a>
	<a href="https://web.cvent.com/event/88db5352-a5af-4db9-ab08-f18f7d191ade/summary#" class="btn registration_button" style="" target="_blank">Modify Registration</a>
</p>

<div id="accordion">
	<h4>IEEE VR 2024 Registration</h4>	
	<div>		
		<p>We are looking forward to you joining us for this special week of workshops, tutorials and presentations of innovative research and advances in VR and 3D interfaces. After reviewing the sections below, use the buttons above to register for IEEE VR 2024.</p>
		<ul>
			<li><b>14 February, 2024</b>: Deadline for paper authors to register and for work to be included in conference program and publications.</li>
			<li><b>14 February, 2024</b>: Early registration ends.</li>		
			<li><b>Author/Submission Questions</b>: Contact IEEE VR 2024 Program Chairs at <span class="program"></span>.</li>	
			<li><b>Visa Information Contact</b>: Contact Carolina Cruz-Neira and Gregory Welch at <span class="general"></span>.</li>
			<li><b>Conference Registration Services</b>: Contact Registration Services at <span class="registration"></span>.</li>	
		</ul>
		<p class="italic">
			Note: All deadlines are at 11:59 PM AOE on the stated date and all rates listed are in USD.			
		</p>
	</div>

	<h4>Important Information for Paper Authors</h4>
	<div>
		<p>
			At least one author per paper must be registered as an <b>AUTHOR</b> at the full Member/Non-Member registration rate, regardless of whether or not they are students.
		</p>
		<ul>
			<li>The registration deadline for authors is <span class="bold">14 February, 2024.</span></li>
			<li>Author registrations are <span class="bold">not refundable</span> and must be processed no later than <span class="bold">February 14, 2024</span> for their work to be included in the conference program and publications.</li>		
			<li>Registration requires a paper ID.</li>
			<li>To register, select the fee under <span class="bold">Full Conference Registration (Saturday–Thursday) – Paper Authors</span>.</li>		
			<li>Each author registration is valid for <span class="bold">FOUR</span> papers.</li>		
			<li>For questions regarding paper submissions, please contact IEEE VR 2024 Program Chairs at <span class="program"></span>.</li>
		</ul>
	</div>

	<h4>What is Included for Each Type of Registration?</h4>
	<div>
		<p>
			<span class="bold">Full Conference (Saturday-Thursday)</span>
			<ul>
				<li>Access to the Workshops & Tutorials (Saturday–Sunday)</li>
				<li>Main Conference (Monday–Thursday)</li>
				<li>Exhibitor Reception (Monday night)</li>
				<li>VR Banquet (Wednesday night)</li>
			</ul>
		</p>
		<p>
			<span class="bold">Main Conference (Monday – Thursday)</span>
			<ul>
				<li>Main Conference (Monday–Thursday)</li>
				<li>Exhibitor Reception (Monday night)</li>
				<li>VR Banquet (Wednesday night)</li>
			</ul>
		</p>
		<p>
			<span class="bold">Main Conference One-Day Only</span>
			<ul>
				<li>Access to the Technical Sessions and Breaks for one day only.</li>
				<li>Depending on the chosen day it could include Exhibits, Research Demonstrations, Panels, and Posters.</li>
				<li>Tickets to any social events must be purchased separately during the registration.</li>
			</ul>
		</p>
		<p>
			<span class="bold">Workshops & Tutorials (Saturday–Sunday)</span>
			<ul>
				<li>Access to the Workshops & Tutorials (Saturday–Sunday)</li>
			</ul>
		</p>
		<p>
			<span class="bold">Workshops & Tutorials One-Day Only</span>
			<ul>
				<li>Access to the Workshops & Tutorials on either Saturday or Sunday.</li>
			</ul>
		</p>
		<p>
			<span class="bold">Additional Tickets</span>
			<ul>
				<li>Reception on Monday night, March 18th</li>
				<li>Banquet on Wednesday night, March 20th</li>
			</ul>
		</p>
	</div>	
	<h4>Fees: Early Registration Ending 14 February, 2024</h4>
	<div>
		<table class="registration-table">
			<tr>
				<th>Registration Categories</th>
				<th>Author</th>				
				<th>Full Conference</th>				
				<th>Main Conference Only<br>(Mon-Thurs)</th>				
				<th>Main Conference<br>One Day</th>				
				<th>Workshops&nbsp;& Tutorials<br>(Sat-Sun)</th>				
				<th>Workshops&nbsp;& Tutorials<br>One Day</th>
			</tr>
			<tr>
				<td>IEEE Member</td>
				<td>$840</td>
				<td>$1,075</td>
				<td>$840</td>
				<td>$350</td>
				<td>$600</td>
				<td>$450</td>
			</tr>
			<tr>
				<td>Non-Member</td>
				<td>$1,010</td>
				<td>$1,290</td>
				<td>$1,010</td>
				<td>$420</td>
				<td>$720</td>
				<td>$540</td>
			</tr>
			<tr>
				<td>IEEE Student Member</td>
				<td>$590</td>
				<td>$755</td>
				<td>$590</td>
				<td>$245</td>
				<td>$420</td>
				<td>$315</td>
			</tr>
			<tr>
				<td>Student Non-Member</td>
				<td>$710</td>
				<td>$910</td>
				<td>$710</td>
				<td>$295</td>
				<td>$505</td>
				<td>$380</td>
			</tr>
			<tr>
				<td><a href="https://www.ieee.org/communities/life-members/index.html" target="_blank">IEEE Life Member</a></td>
				<td>$465</td>
				<td>$595</td>
				<td>N/A</td>
				<td>N/A</td>
				<td>N/A</td>
				<td>N/A</td>
			</tr>
		</table>
	</div>
	<h4>Fees: Registration After 14 February 2024</h4>
	<div>
		<table class="registration-table">
			<tr>
				<th>Registration Categories</th>
				<th>Author</th>				
				<th>Full Conference</th>				
				<th>Main Conference Only<br>(Mon-Thurs)</th>				
				<th>Main Conference<br>One Day</th>				
				<th>Workshops&nbsp;& Tutorials<br>(Sat-Sun)</th>				
				<th>Workshops&nbsp;& Tutorials<br>One Day</th>
			</tr>
			<tr>
				<td>IEEE Member</td>
				<td rowspan="5" style="border: 1px solid #152840 !important">Authors<br>must do<br>early<br>registration</td>
				<td>$1,300</td>
				<td>$1,010</td>
				<td>$420</td>
				<td>$720</td>
				<td>$540</td>
			</tr>
			<tr>
				<td>Non-Member</td>
				<td>$1,560</td>
				<td>$1,215</td>
				<td>$505</td>
				<td>$865</td>
				<td>$650</td>
			</tr>
			<tr>
				<td>IEEE Student Member</td>
				<td>$910</td>
				<td>$710</td>
				<td>$295</td>
				<td>$505</td>
				<td>$380</td>
			</tr>
			<tr>
				<td>Student Non-Member</td>
				<td>$1,095</td>
				<td>$855</td>
				<td>$355</td>
				<td>$610</td>
				<td>$460</td>
			</tr>
			<tr>
				<td><a href="https://www.ieee.org/communities/life-members/index.html" target="_blank">IEEE Life Member</a></td>
				<td>$715</td>
				<td>N/A</td>
				<td>N/A</td>
				<td>N/A</td>
				<td>N/A</td>
			</tr>
		</table>
	</div>
	<h4>Fees: Workshops Onsite Registration</h4>
	<div>
		<table class="registration-table">
			<tr>
				<th class="valignBottom alignCenter">Registration Categories</th>
				<th class="valignBottom alignCenter">Workshops&nbsp;& Tutorials<br>(Sat-Sun)</th>				
				<th class="valignBottom alignCenter">Workshops&nbsp;& Tutorials<br>One Day</th>
			</tr>
			<tr>
				<td>IEEE Member</td>
				<td>$790</td>
				<td>$595</td>
			</tr>
			<tr>
				<td>Non-Member</td>
				<td>$950</td>
				<td>$715</td>
			</tr>
			<tr>
				<td>IEEE Student Member</td>
				<td>$555</td>
				<td>$420</td>
			</tr>
			<tr>
				<td>Student Non-Member</td>
				<td>$670</td>
				<td>$505</td>
			</tr>
			<tr>
				<td><a href="https://www.ieee.org/communities/life-members/index.html" target="_blank">IEEE Life Member</a></td>
				<td>N/A</td>
				<td>N/A</td>
			</tr>
		</table>
	</div>
	<h4>Fees: Additional Reception/Banquet Tickets</h4>
	<div>
		<p>If you need to purchase additional tickets for the reception or banquet, the prices are:</p>
		<ul>
			<li><b>Reception on Monday night, 18 March 2024</b>: $65.00</li>
			<li><b>Banquet on Wednesday night, 20 March 2024</b>: $120.00</li>		
		</ul>
	</div>
	<h4>Visa Invitation Letters</h4>
	<div>
		<p>
			If you require a visa invitation letter, one will be automatically generated using your name, organization, and address. <span style="color: red;">Please note that if you request a visa letter, your registration cannot be cancelled.</span> Requests for letters containing additional information, such as date of birth or passport information (number, date of issue, expiration date, place of issue), may be e-mailed to: Carolina Cruz-Neira and Gregory Welch at <span class="general"></span>. 
		</p>
		<p>
			Website for Visa information: <a href="https://ieeevr.org/2018/attend/visa">https://ieeevr.org/2018/attend/visa</a>
		</p>
	</div>	
	<h4>Cancellation Policy</h4>
	<div>
		<p>
			All refund/cancellation requests must be received in writing to <span class="registration"></span> by <b>15 February, 2024 11:59 PM AoE Time</b>. There will be an administrative fee of US$150 for cancelled registrations and US$150 deducted for One-Day/Workshop/Tutorial registrations from each cancellation.
		</p>
		<p>
			Note:
			<ul>
				<li>Author registrations are non-refundable.</li>
				<li>Registrations where a Visa invitation was requested can not be cancelled.</li>
			</ul>
		</p>
	</div>
</div>