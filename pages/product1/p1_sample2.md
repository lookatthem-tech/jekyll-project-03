---
title: SMS Integration with Twilio Marketplace

sidebar: product1_sidebar
permalink: p1_sample2.html
folder: product1
---
<html><body>  

<p>The SMS Integration with Twilio provides the ability to configure Short Messaging Service (SMS) notifications within the <MadCap:conditionalText data-mc-conditions="UKGRConditionTags.WFR">UKG Ready</MadCap:conditionalText> application. When this integration is added and set up, SMS message configuration will be available in the following areas:</p>
<ul>
	<li>
		<p>Global Notifications</p>
	</li>
	<li>
		<p>Workflow Notifications</p>
	</li>
	<li>
		<p>Communication Templates (HR only)</p>
	</li>
</ul>
<p>Twilio offers a global platform that makes sending SMS notifications easy.</p>
<ul>
	<li>
		<p>Send SMS messages with local and toll-free numbers, short codes, custom alphanumeric sender IDs, or by using your own existing phone numbers.</p>
	</li>
	<li>
		<p>Send Multimedia Messaging Service (MMS) messages. Outside the U.S. and Canada, attachments are sent as links.</p>
	</li>
	<li>
		<p>Send text messages over the carrier network to any phone, anywhere in the world.</p>
	</li>
	<li>
		<p>Automatic route monitoring ensures that long-code phone numbers are used to send messages when a carrier is unable to receive messages from short codes, and that global messages always take the best path.</p>
	</li>
	<li>
		<p>Send long messages and Twilio will automatically segment and reassemble them.</p>
	</li>
	<li>
		<p>Messages sent to the same person automatically uses a previously recognizable phone number to create a consistent experience and maintain conversation history.</p>
	</li>
</ul>
<p>You must set up an account with Twilio prior to using this functionality with Workforce Ready. We have provided links under the <b>Pricing</b> tab of the Marketplace product to help you contact them, view Twilio pricing structures, and other Twilio support information.</p>


<h1>Requirements and Prerequisites</h1>
<p>To take advantage of SMS functionality, you must complete a few steps prior to using it. First, you must add the <b>SMS Integration with Twilio</b> marketplace product. Once added, there are a few housekeeping steps to complete in your company. Once that is done you will then be able to select SMS options within company notifications.</p>
<h2>Download the Marketplace Product</h2>
<p>To add the marketplace product, navigate to <b>Marketplace &gt; Marketplace Setup</b> and add the <b>SMS Integration with Twilio</b> marketplace product to the company.</p>
<div class="Note" data-mc-autonum="&lt;span style=&quot;color: #000099;&quot; class=&quot;mcFormatColor&quot;&gt;&lt;b&gt;Note: &lt;/b&gt;&lt;/span&gt;"><span class="autonumber"><span><span style="color: #000099;" class="mcFormatColor"><b>Note: </b></span></span></span>The marketplace product contains links and information to Twilio. You must create a Twilio account and gather information from them before you can complete the final installation of the product.</div>
<ul>
	<li>
		<p>From the <b>Home</b> or <b>Search/Browse</b> tab, locate and click the <b>SMS Integration with Twilio </b>product hyperlink.</p>
	</li>
	<li>
		<p>Click <b>Add To Company</b>. You will be prompted to sign the <b>Terms And Conditions</b> page.</p>
	</li>
	<li>
		<p>After signing the <b>Terms And Conditions</b>, select a security profile for the users who will manage this product. This is typically the Company Administrator.</p>
	</li>
	<li>
		<p>After clicking <b>OK</b>, the system will process for a bit and when finished, a <b>Success</b> message will display.</p>
	</li>
	<li>
		<p>You can verify the installation on the <b>Installed</b> tab.</p>
	</li>
</ul>
<p>After you’ve created your Twilio account, the next step is to edit the marketplace product settings and add your Twilio information.</p>
<ul>
	<li>
		<p>Under the <b>Installed</b> tab, click the edit icon for the product.</p>
	</li>
	<li>
		<p>Input the Twilio <b>Account SID</b>, <b>Authentication Token</b>, and <b>Messaging Service SID</b> into the appropriate fields.</p>
	</li>
</ul>
<h3>Global Setup</h3>
<p>Once your marketplace product is installed and completed, you will then need to edit a few settings in your company.</p>
<p>Enable SMS notifications globally. Multiple options are available. After selecting an option here, SMS fields will then become available in the application. Skipping this step will result in no SMS settings being available. Optionally, you can configure a custom SMS Header that will be appended to the front of each SMS notification.</p>
<p>Navigate to the <b>Company Configuration</b> widget under the <b>Company Info</b> tab, located under <b>Company Settings &gt; Global Setup &gt; Company Setup</b>, and select an SMS option in the <b>Notifications Through</b> field.</p>
												  <p><b>SMS</b>: Will use only SMS messaging.</p>
<p><b>SMS &amp; Email</b>: Will use SMS messaging and allow the email option as well.</p>
<p><b>SMS &amp; Mailbox</b>: Will use SMS messaging and allow the user’s mailbox to receive messages.</p>
<p><b>Email &amp; Mailbox &amp; SMS</b>: Will use SMS messaging, user mailboxes, and email.</p>
<p><b>SMS Header: </b>In this field, you can optionally type a customized header that will be appended to the front of each SMS message sent from the system. For example, you may want to alert recipients who the alert is coming from by entering your company name in this field, i.e., OURCOMPANY: rest of header.</p>
<p>Employees can enable/disable SMS in notification preferences. End users will be able to toggle their own SMS notification preferences under <b>My Info</b> &gt; <b>My Information &gt; Notification Preferences</b>.</p>

<p>Broadcast Messaging can be turned off by unchecking the related boxes for Broadcast Email, Broadcast Mailbox, and Broadcast Message SMS. Unchecking these has no effect on the options under them for Primary Email, Mailbox, and SMS. If&#160;Primary Email, Mailbox or SMS are disabled, the corresponding Broadcast Messaging option is disabled as well.</p>

<div class="Note" ><b>Note: </b></span></span></span>To comply with Twilio and industry standards, end users will be able to reply with STOP, CANCEL, etc. to any SMS notification. If they do, notification preferences will be updated in the application to disable SMS. Notification preference changes can be audited in the Account Audit Trail report as well.</div>




<h1>Configuring Communications with SMS</h1>
<p>You can configure the system to use SMS&#160;in notifications, workflows, and recruitment.</p>
<h2>SMS in Notifications</h2>
<p>Once your company has been edited to enable SMS messaging fields, you can then begin using SMS messages in notifications. Notifications are configured under <b>Company Settings &gt; Global Setup &gt; Notifications</b>.</p>
<p>Depending what was selected in <b>Company Setup</b> will determine the fields available in notifications. The <b>SMS Message</b> will be disabled by default. Check the <b>Enabled</b> checkbox to activate the message options. Once enabled, you can then type a customized message and use the system tags to create a message. The messages have a 1400-character limit.</p>


<h2>SMS in Workflows</h2>
<p>SMS notifications can also be added to the <b>Generate Notification</b> step in workflows. This will generate a SMS message to the designated recipient when the workflow proceeds to the <b>Generate Notification</b> step. Workflows are located under <b>Company Settings &gt; Global Setup &gt; Workflows</b>. The <b>SMS Enabled</b> checkbox will be unchecked by default. Check to activate the SMS messaging options.</p>

<h2>Two-Way SMS in Workflows</h2>
<p>When using workflows, users can leverage Two-Way SMS functionality when it comes to approvals or rejections of actions within the particular workflow. This is configured in the same place as mentioned above (in the Generate Notifications step). You will want to apply this to the notifications step that comes before the Approval/Reject Manager step.</p>

<p>As you click the SMS Enabled checkbox, you will see another option for Two Way SMS Enabled that will need to be checked.</p>

<p>As the SMS Message text space appears, configure your message using free text and tags as normal.</p>

<p>When the workflow is triggered and the notification is sent, the manager will see the message as formatted by the user in configuration. This will immediately be followed by a canned set of instructions to explain how to advance the workflow: Please reply Y/N followed by this code &lt;code&gt; to Approve/Reject this request. The code is very important as this is a unique value tied to each request. As a manager, you could receive multiple requests for one workflow and the system needs to know which specific request is being approved or denied.</p>

<p>There is error proofing built into this process as well. If an incorrect code is entered, the system will let you know (similarly if you enter the same code twice).</p>
<h3>Two-Way SMS Workflows: Required Comment</h3>
<p>You can configure a Workflow to allow for a SMS response to Approve or Reject, plus any required Comment, so that users can Approve/Reject a Workflow that includes a Comment and submit it via SMS. When the Workflows listed below are sent through SMS Two-Way, the user is notified that a Comment is required in addition to their Approve/Reject and unique code.</p>
<ul>
	<li>
		<p>Time Off Request</p>
	</li>
	<li>
		<p>Timesheet</p>
	</li>
	<li>
		<p>Timesheet Change Request</p>
	</li>
	<li>
		<p>Schedule</p>
	</li>
	<li>
		<p>Schedule Open Shift</p>
	</li>
	<li>
		<p>Schedule Request for Coverage</p>
	</li>
	<li>
		<p>Schedule Shift Swap</p>
	</li>
	<li>
		<p>Compensation Proposal Request</p>
	</li>
</ul>
<h2>SMS in Recruitment</h2>
<p>If you are using the Recruitment marketplace product, SMS communication can be configured in communication templates. This will allow managers, hiring managers, and HR professionals to communicate with applicants via SMS messaging.</p>
<h3>Communication Templates</h3>
<p>Communication Templates can be selected by the manager or HR professional when communicating with an applicant. The communication templates are located at <b>Company Settings &gt; HR Setup &gt; Applicant Tracking/Recruitment &gt; Templates Library &gt;&#160;Communication Templates</b>. The <b>SMS Enabled</b> checkbox will be unchecked by default. Check to activate the SMS messaging options.</p>
<div class="Tip" data-mc-autonum="&lt;span style=&quot;color: #ff9933;&quot; class=&quot;mcFormatColor&quot;&gt;&lt;b&gt;Tip: &lt;/b&gt;&lt;/span&gt;"><span class="autonumber"><span><span style="color: #ff9933;" class="mcFormatColor"><b>Tip: </b></span></span></span>Make sure to check the Active checkbox in the notification to make it available.</div>

<h3>Communications with Applicants</h3>
<p>When managers or HR professionals choose to communicate with an applicant, they can choose one of the preconfigured communication templates or create a customized message. Managers can communicate with applicants in the following areas:</p>
<ul>
	<li>
		<p>
			<MadCap:conditionalText data-mc-conditions="UKGRConditionTags.WFR"><b>Team &gt; </b>
			</MadCap:conditionalText><b>Recruitment &gt; Candidates &gt; Applicants</b>
		</p>
	</li>
	<li>
		<p>
			<MadCap:conditionalText data-mc-conditions="UKGRConditionTags.WFR"><b>Team &gt; </b>
			</MadCap:conditionalText><b>Recruitment &gt; Candidates &gt; Job Applications</b>
		</p>
	</li>
</ul>
<p>In both areas, users will select one or more applicants or job applications and select the <b>Communicate To Selected</b> button. In the pop-up, you can select a communication template from the <b>Template To Use</b> icon. When selecting a template, it will populate the Email area (if enabled at the company level), and the SMS area with content from the template. Users can edit as needed.</p>
<p>If not using a template, users can create their own customized messages and use system tags to complete the message.</p>
<h4>Applicants and Job Applications</h4>
<p>After selecting one or more entries and clicking the <b>Communicate To Selected</b> button, the pop-ups will allow you select a template, create customized messages, or turn off/on certain communication methods.</p>


<h4>Job Requisitions and Applicant Information</h4>
<p>When opening a Job Requisition for viewing or editing, an option is available to <b>Notify Applicant</b> which is a manual method of encouraging an applicant to apply for the job. After selecting the option and adding an applicant, a communication pop-up will display where you can craft a communication to the applicant. You can select a communication template or create a customized message. The options available here will depend on what was selected on the <b>Company Setup</b> page (Email, SMS, etc.).</p>
<p>Job Requisitions are located under <MadCap:conditionalText data-mc-conditions="UKGRConditionTags.WFR"><b>Team &gt; </b></MadCap:conditionalText><b>Recruitment &gt; Job Requisitions</b>.</p>

<p>When viewing or editing an applicant, the <b>Applicant Information</b> page will open and contains multiple tabs and <b>Jump To</b> links. On the <b>Communications</b> tab, you can select various communication options. In the <b>Interviews</b> widget, in the Actions ellipses, you can add an interview (if none are listed). Once added, the Actions ellipses in the entry will have the <b>Communicate</b> option. When selected, a pop-up will display. This pop-up contains the SMS option, as well as the iCalendar Attachment option. The options available here will depend on what was selected on the <b>Company Setup</b> page (Email, SMS, etc.)</p>
<p>If there are multiple options in the lists, and you want to send the same communication to all selected, you can select the entries and then click the <b>Communicate</b> button on the page.</p>
<p>Applicant Information is located under <MadCap:conditionalText data-mc-conditions="UKGRConditionTags.WFR"><b>Team &gt; </b></MadCap:conditionalText><b>Recruitment &gt; Candidates &gt; Applicants</b>. Then open/view an applicant from the list.</p>


<p>In the pop-ups, you will have the option to turn off or on each area of communication via the slider bubble.</p>
<p><b>On</b>
</p>

<p><b>Off:</b> The content will remain, but will be grayed out.</p>

<div class="Tip" data-mc-autonum="&lt;span style=&quot;color: #ff9933;&quot; class=&quot;mcFormatColor&quot;&gt;&lt;b&gt;Tip: &lt;/b&gt;&lt;/span&gt;"><span class="autonumber"><span><span style="color: #ff9933;" class="mcFormatColor"><b>Tip: </b></span></span></span>If iCalendar Attachment is enabled within any of these areas, an iCalendar attachment will be delivered with the notification in the form of an MMS message.</div>




</body></html>                                                   