---
title: Error Logging in Prysm for Desktop


sidebar: product1_sidebar
permalink: ErrorLogging.html
folder: ApiDev
---
<html><body>
				   
			
			<p>Prysm for desktop includes error logging. You can open the logs to troubleshoot issues you might experience with the app.</p>
			<div class="Tip" data-mc-autonum="&lt;span style=&quot;color: #ff9933;&quot; class=&quot;mcFormatColor&quot;&gt;&lt;b&gt;Tip: &lt;/b&gt;&lt;/span&gt;"><span class="autonumber"><span><span style="color: #ff9933;" class="mcFormatColor"><b>Tip: </b></span></span></span> You can also contact Prysm support and share your logs with them to get help with issues.</div>
			<p>Both the main Prysm for desktop app and its companion Prysm Sharing Agent app include this error logging. The following sections include the details for both apps.</p>
			<h2>Opening Log Files</h2>
					<p>To open log files for troubleshooting, you locate and open the logs in the Logs folder:</p>
					<ol>
						<li value="1">On the device where Prysm for desktop is installed, <b>navigate</b> to:<br /><code>C:\Users\&lt;Username&gt;\AppData\Local\Packages\<br />PrysmInc.Prysm_gcnfe4jvxweze\LocalState\logs</code><div class="Note" data-mc-autonum="&lt;span style=&quot;color: #000099;&quot; class=&quot;mcFormatColor&quot;&gt;&lt;b&gt;Note: &lt;/b&gt;&lt;/span&gt;"><span class="autonumber"><span><span style="color: #000099;" class="mcFormatColor"><b>Note: </b></span></span></span>If you want to open log files for Prysm Sharing Agent, on the device where it's installed, navigate to:<br /><br /><code>C:\Users\&lt;Username&gt;\AppData\Local\Packages\<br />PrysmInc.PrysmSharingExtension_gcnfe4jvxweze\LocalState\logs</code></div></li>
						<li value="2">In the folder, you see the log files, which are .txt files named for the day of activities that the log contains, such as:
<ul><li><code>log-20180327.txt</code> (for Prysm for desktop)</li><li><code>prysm-desktop-ext-log-20180327.txt</code> (for Prysm Sharing Agent)</li></ul></li>
						<li value="3"><b>Open</b> the log file corresponding to the time your issue occurred (in Notepad or your preferred text editor).</li>
					</ol>
				</div>
			</div>
			<h2>Configuring Logging</h2>
					<p>Prysm recommends using the preconfigured logging settings. If you find that those aren't working for you, you can locate and edit the configuration .xml file to change the configuration: </p>
					<ol>
						<li value="1">On the device where Prysm for desktop is installed, <b>navigate</b> to:<br /><code>C:\Users\&lt;Username&gt;\AppData\Local\Packages\<br />PrysmInc.Prysm_gcnfe4jvxweze\LocalState\UserConfig.xml</code><br /><div class="Note" data-mc-autonum="&lt;span style=&quot;color: #000099;&quot; class=&quot;mcFormatColor&quot;&gt;&lt;b&gt;Note: &lt;/b&gt;&lt;/span&gt;"><span class="autonumber"><span><span style="color: #000099;" class="mcFormatColor"><b>Note: </b></span></span></span>If you're configuring logging for Prysm Sharing Agent, on the device where it's installed, navigate to:<br /><br /><code>C:\Users\&lt;Username&gt;\AppData\Local\Packages\<br />PrysmInc.PrysmSharingExtension_gcnfe4jvxweze\<br />LocalState\UserConfig.xml</code></div></li>
						<li value="2">Open <b>UserConfig.xml</b> (in Notepad or your preferred text editor).<br />The contents of the file look similar to the following:<br /><code>&lt;?xml version="1.0" encoding="utf-8" ?&gt;<br />&lt;configuration&gt;<br />  &lt;appSettings&gt;<br />      &lt;add key="AppInsightsLogLevel" value="Warning"&gt;<br />&lt;add key="LogFileLogLevel" value="Information"&gt;<br />&lt;add key="AllowRememberMe" value="false"/&gt;<br />   &lt;/appSettings&gt;<br />&lt;/configuration&gt;</code><br /><div class="Note" data-mc-autonum="&lt;span style=&quot;color: #000099;&quot; class=&quot;mcFormatColor&quot;&gt;&lt;b&gt;Note: &lt;/b&gt;&lt;/span&gt;"><span class="autonumber"><span><span style="color: #000099;" class="mcFormatColor"><b>Note: </b></span></span></span>The following line of the file is relevant only if you use Microsoft Azure Application Insights:<br /><br /><code>&lt;add key="AppInsightsLogLevel" value="Warning"&gt;<br /></code><br />You can set this Application Insights log level value to a different value than you set for LogFileLogLevel to configure different levels of logging for Application Insights and for the log file on the device.</div></li>
						<li value="3">If you need to change the preconfigured level of logging, change the values to other standard debugging level values, such as:
<ul><li>Information</li><li>Warning</li><li>Error</li><li>Trace</li><li>Fatal</li><li>All</li><li>Off</li></ul></li>
						<li value="4"><b>Save</b> and <b>close</b> the UserConfig.xml file.</li>
					</ol>

</body></html>
				
