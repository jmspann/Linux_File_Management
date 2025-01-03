<h1>Managing Files and Users in Linux</h1>

<h2>Description</h2>
This lab utilizes basic Linux commands for a number of daily tasks a cybersecurity analyst may perform including: file management, updating authorization on files and directories, and managing users access.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux Command-Line</b> 

<h2>Environments Used </h2>

- <b>KALI LINUX</b>
- <b>Linux Bash Shell</b>

<h2>Program Walk-Through:</h2>

<h3>File Management</h3>

<p align="center">
Check that the APT is installed using the <em><strong>apt</strong></em> command: <br/>
<img src="https://i.imgur.com/YCsjA19.png" height="100%" width="100%" alt="Installation Steps"/>
<br />
<br />
Install tcpdump using the <em><strong>sudo</strong></em> command:  <br/>
<img src="https://i.imgur.com/PQwNPRE.png" height="100%" width="100%" alt="Installation Steps"/>
<br />
<br />
Verify tcpdump was installed successfully by typing <em><strong>apt list --installed</strong></em> in the command prompt: <br/>
<img src="https://i.imgur.com/1ub4E6G.png" height="100%" width="100%" alt="Installation Steps"/>
<br />
<br />
Install Suricata using the <em><strong>sudo</strong></em> command:  <br/>
<img src="https://i.imgur.com/28kvYXT.png" height="100%" width="100%" alt="Installation Steps"/>
<br />
<br />
Verify Suricata was installed successfully by typing the same command from above: <br/>
<img src="https://i.imgur.com/AHEFxA0.png" height="100%" width="100%" alt="Installation Steps"/>
</p>
<br />
<br />

<h3>Updating Authorizations</h3>

<p align="center">
Generate string outputs using the <em><strong>echo</strong></em> command:  <br/>
<img src="https://i.imgur.com/qtlhg6d.png" height="100%" width="100%" alt="Generate Outputs"/>
<br />
<br />
Now generate mathematical expressions using the <em><strong>expr</strong></em> command:  <br/>
<img src="https://i.imgur.com/l8hauds.png" height="100%" width="100%" alt="Generate Outputs"/>
</p>
<br />
<br />

<h3>Managing User Access</h3>

<p align="center">
Print the current working directory and list the contents using the <em><strong>pwd</strong></em> and <em><strong>ls</strong></em> commands:  <br/>
<img src="https://i.imgur.com/zpAXUZo.png" height="100%" width="100%" alt="Linux Navigation"/>
<br />
<br />
Now change directories to "reports" and list its contents using the <em><strong>cd</strong></em> command:  <br/>
<img src="https://i.imgur.com/avNLmjH.png" height="100%" width="100%" alt="Linux Navigation"/>
<br />
<br />
Navigate to the "users" directory and list its contents. After listing the contents, open a file using the <em><strong>cat</strong></em> command:  <br/>
<img src="https://i.imgur.com/In4Xm05.png" height="100%" width="100%" alt="Linux Navigation"/>
<br />
<br />
Now navigate to the "logs" directory and display the first 10 lines of the file it contains using the <em><strong>head</strong></em> command:  <br/>
<img src="https://i.imgur.com/iiUqgIf.png" height="100%" width="100%" alt="Linux Navigation"/>
</p>
<br />
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
