---
title: Error Logging in Prysm for Desktop


sidebar: developer_sidebar
permalink: ErrorLogging.html
folder: ApiDev
---

				   
			
<p>Prysm for desktop includes error logging. You can open the logs to troubleshoot issues you might experience with the app.</p>
	
<p>You can also contact Prysm support and share your logs with them to get help with issues.</p>

<p>Both the main Prysm for desktop app and its companion Prysm Sharing Agent app include this error logging. The following sections include the details for both apps.</p>

<h1>Opening Log Files</h1>
	
<p>To open log files for troubleshooting, you locate and open the logs in the Logs folder:</p>

<ol>
<li>On the device where Prysm for desktop is installed, navigate to:<br /><br />
	
<code>C:\Users\&lt;Username&gt;\AppData\Local\Packages\<br />PrysmInc.Prysm_gcnfe4jvxweze\LocalState\logs</code>
	
<p>If you want to open log files for Prysm Sharing Agent, on the device where it's installed, navigate to:<br /><br /><code>C:\Users\&lt;Username&gt;\AppData\Local\Packages\<br />
PrysmInc.PrysmSharingExtension_gcnfe4jvxweze\LocalState\logs</code></p></li>
	
<li>In the folder, you see the log files, which are .txt files named for the day of activities that the log contains, such as:
	
<ul><li><code>log-20180327.txt</code> (for Prysm for desktop)</li>
<li><code>prysm-desktop-ext-log-20180327.txt</code> (for Prysm Sharing Agent)</li>
</ul></li>

<li>Open the log file corresponding to the time your issue occurred (in Notepad or your preferred text editor).</li>
</ol>

	
<h1>Configuring Logging</h1>
	
	
<p>Prysm recommends using the preconfigured logging settings. If you find that those aren't working for you, you can locate and edit the configuration .xml file to change the configuration:</p>

<ol>

<li>On the device where Prysm for desktop is installed, navigate to:<br /><br />
	
<code>C:\Users\&lt;Username&gt;\AppData\Local\Packages\<br />
PrysmInc.Prysm_gcnfe4jvxweze\LocalState\UserConfig.xml</code><br />
	
<p>If you're configuring logging for Prysm Sharing Agent, on the device where it's installed, navigate to:<br /><br />
	
<code>C:\Users\&lt;Username&gt;\AppData\Local\Packages\<br />
PrysmInc.PrysmSharingExtension_gcnfe4jvxweze\<br />
LocalState\UserConfig.xml</code>
</li>

	
<li>Open <b>UserConfig.xml</b> (in Notepad or your preferred text editor).<br />
	
The contents of the file look similar to the following:<br /><br />
	
<code>&lt;?xml version="1.0" encoding="utf-8" ?&gt;<br />
&lt;configuration&gt;<br />
&lt;appSettings&gt;<br />
&lt;add key="AppInsightsLogLevel" value="Warning"&gt;<br />
&lt;add key="LogFileLogLevel" value="Information"&gt;<br />
&lt;add key="AllowRememberMe" value="false"/&gt;<br />
&lt;/appSettings&gt;<br />
&lt;/configuration&gt;</code>
	
<p>The following line of the file is relevant only if you use Microsoft Azure Application Insights:<br /><br />
	
<code>&lt;add key="AppInsightsLogLevel" value="Warning"&gt;</code>
	
<p>You can set this Application Insights log level value to a different value than you set for LogFileLogLevel to configure different levels of logging for Application Insights and for the log file on the device.</p>
</li>
	
<li>If you need to change the preconfigured level of logging, change the values to other standard debugging level values, such as:

<ul>
<li>Information</li>
<li>Warning</li>
<li>Error</li>
<li>Trace</li>
<li>Fatal</li>
<li>All</li>
<li>Off</li>
</ul></li>
<li><b>Save</b> and <b>close</b> the UserConfig.xml file.</li>
</ol>


				
