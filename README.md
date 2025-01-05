<h1>Managing Files and Users in Linux</h1>

<h2>Description</h2>
This lab utilizes basic Linux commands for a number of daily tasks a cybersecurity analyst may perform including: file management, updating authorization on files and directories, and managing users.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux Command-Line</b> 

<h2>Environments Used </h2>

- <b>KALI LINUX</b>
- <b>Linux Bash Shell</b>

<h2>Program Walk-Through:</h2>

<h3>File Management</h3>

<p align="center">
The first step is to make a new subdirectory called "logs" to store future logs within the "analyst" directory using the <em><strong>mkdir</strong></em> command: <br/>
<img src="https://i.imgur.com/jkg9jf9.png" height="100%" width="100%" alt="File Management"/>
<br />
<br />
Next will be to remove the "temp" directory, since it will not longer be needed, using the <em><strong>rmdir</strong></em> command:  <br/>
<img src="https://i.imgur.com/tqItcWA.png" height="100%" width="100%" alt="File Management"/>
<br />
<br />
Now move the "Q3patches.txt" file from the "notes" directory to the "reports" directory using <em><strong>mv</strong></em>: <br/>
<img src="https://i.imgur.com/CNh1wLC.png" height="100%" width="100%" alt="File Management"/>
<br />
<br />
Next, delete the unused file "tempnotes.txt" from the "notes" directory using the <em><strong>rm</strong></em> command:  <br/>
<img src="https://i.imgur.com/LDYvIOc.png" height="100%" width="100%" alt="File Management"/>
<br />
<br />
Now, create a file named "tasks.txt" in the "notes" directory using the <em><strong>touch</strong></em> command: <br/>
<img src="https://i.imgur.com/GPJw9wY.png" height="100%" width="100%" alt="File Management"/>
<br />
<br />
Finally, edit the "tasks.txt" file using the nano text editor using the <em><strong>nano</strong></em> command. Add a note detailing the tasks completed, then save the changes made before exiting the text editor. Verify the changes were saved by opening the file afterwards: <br/>
<img src="https://i.imgur.com/bsBm9xJ.png" height="100%" width="100%" alt="File Management"/>
<img src="https://i.imgur.com/b9WOS12.png" height="100%" width="100%" alt="File Management"/>
</p>
<br />
<br />

<h3>Updating Authorizations</h3>

<p align="center">
We'll first start by listing all the files and permissions in the "projects" directory using the <em><strong>ls -la</strong></em> command:  <br/>
<img src="https://i.imgur.com/DQrGCGC.png" height="100%" width="100%" alt="File Permissions"/>
<br />
<br />
None of the files should allow write access for the "other" users. We'll remove this permission for any files using the <em><strong>chmod</strong></em> command:  <br/>
<img src="https://i.imgur.com/vY2aQTl.png" height="100%" width="100%" alt="File Permissions"/>
<br />
<br />
"project_m.txt" is a restricted file and should not have read or write access by the "group" or "other", so these permissions should be removed:  <br/>
<img src="https://i.imgur.com/xXtsABI.png" height="100%" width="100%" alt="File Permissions"/>
<br />
<br />
".project_x.txt" is a hidden file that has been archived and should not by written to by anyone. The user and group should still have read access to this file. Update the permissions accordingly:  <br/>
<img src="https://i.imgur.com/oVfdLIx.png" height="100%" width="100%" alt="File Permissions"/>
<br />
<br />
Finally, only the user should access to the "drafts" directory and its contents, which is execute privileges. Update the directory permissions to reflect this:  <br/>
<img src="https://i.imgur.com/R4R4BKR.png" height="100%" width="100%" alt="File Permissions"/>
</p>
<br />
<br />

<h3>Managing Users</h3>

<p align="center">
A new employee joined the Research department and needs to be added to the system using the <em><strong>useradd</strong></em> command. The new employee, "researcher9" also needs to be added to the "research_team" group as their primary group, which can be done using the <em><strong>usermod</strong></em> command and the <em><strong>-g</strong></em> option:  <br/>
<img src="https://i.imgur.com/i7HjuGX.png" height="100%" width="100%" alt="Manage Users"/>
<br />
<br />
Researcher9 will take responsibility of "project_r" which is located in the "projects" directory. The owner can be changed using the <em><strong>chown</strong></em> command:  <br/>
<img src="https://i.imgur.com/CH4co0v.png" height="100%" width="100%" alt="Manage Users"/>
<br />
<br />
Now researcher9 is working in the Sales department along with the Researcher department and needs to be added to a secondary group, "sales_team". This can be done using the <em><strong>-a</strong></em> option to add and the <em><strong>-G</strong></em> option to specify a supplemental group:  <br/>
<img src="https://i.imgur.com/wHGO4fa.png" height="100%" width="100%" alt="Manage Users"/>
<br />
<br />
Finally, researcher9 has completed their job is is leaving the company and they need to be removed from the system. This can be done using the <em><strong>userdel</strong></em> command. It's also good practice to remove the group Linux automatically creates with the same name using the <em><strong>groupdel</strong></em> command:  <br/>
<img src="https://i.imgur.com/xFLu2YG.png" height="100%" width="100%" alt="Manage Users"/>
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
