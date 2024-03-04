<h1>CompTIA A+ 1102 lesson 1.3</h1>



<h2>Description</h2>
Microsoft Management Consoles (MMCs) provide a standard interface for advanced configuration and management of Windows desktops and servers. You can use these consoles to manage security settings, set up scheduled tasks, and manage the disk subsystem. Additionally, when a configuration setting is not exposed in any of the normal GUI tools, you will need to use the Registry Editor to solve some types of issues.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Run Command</b> 

<h2>Environments Used </h2>

- <b>Windows </b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
launch run command using windows key and "r": <br/>
<img src="https://i.imgur.com/0aR4zH5.png" height="80%" width="80%" alt="device manager"/>
<br />
<br />
type devmgmt.msc and hit enter:  <br/>
<img src="https://i.imgur.com/WmNeEll.png" height="80%" width="80%" alt="Device manager"/>
<br />
<br />
Device Manager (devmgmt.msc) allows you to view and edit the properties of installed hardware. You can change hardware configuration settings, update drivers, or remove/disable devices. To update or troubleshoot a device manually, in the Device Manager hardware tree, locate the device, right-click it, and select Properties to display the device settings. The General tab displays status information for the device. Use the Update Driver button on the Drivers tab to install a new driver: <br/>
<img src="https://i.imgur.com/mYl9sLz.png" height="80%" width="80%" alt="device manager properties"/>
<br />
<br />
in the device manager you can dissable a device and roll back drivers if a new driver doesnt work well.<br/>
next is the disk management console. The Disk Management (diskmgmt.msc) console displays a summary of any fixed and removable disks—hard disk drives (HDDs), solid state drives (SSDs), and optical drives—attached to the system. HDDs and SSDs can be divided into logical partitions. Each partition is represented as a volume in the top pane:  <br/>
<img src="https://i.imgur.com/mpkb0r3.png" height="80%" width="80%" alt="Disk management"/>
<br />
<br />
One of the disks (typically Disk 0) will be the one holding the operating system. This disk will have at least three volumes.  <br/>
Next is the disk defragmentation tool. The Defragment and Optimize Drives tool (dfrgui.exe) runs various operations to speed up the performance of HDDs and SSDs:<br/>
<img src="https://i.imgur.com/u572Okz.png" height="80%" width="80%" alt="Disk defrag"/>
<br />
Windows automatically schedules the disk optimizer to run using Task Scheduler. You should check for any issues, such as it not running successfully.
<br />
The Disk Clean-up (cleanmgr.exe) tool tracks files that can be safely erased to reclaim disk space. These files include ones deleted but still available in the Recycle Bin and various temporary files and caches. The tool can be run in administrator mode using the Clean up system files option to reclaim data from caches such as Windows Update and Defender.  <br/>
<img src="https://i.imgur.com/gu1Z1bp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  The Task Scheduler (tasksch.msc) runs commands and scripts automatically. Many of Windows's processes come with predefined schedules. Tasks can be run once at a future date or time or according to a recurring schedule. A task can be a simple application process (including switches, if necessary) or a batch file or script. Other features include:
<br />
<ul>
<li>A trigger can be an event rather than a calendar date/time. For example, a task can be set to run when the user signs in or when the machine wakes from sleep or hibernation.</li>
<li>Each task can include multiple actions.</li>
<li>All activity is logged so that you can investigate failed tasks.</li>
</ul> 
</p>
<p align="center">
<br />
<img src="https://i.imgur.com/NBS0U64.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
The Local Users and Groups (lusrmgr.msc) console provides an advanced interface for creating, modifying, disabling, and deleting user accounts. You can also reset the password for an account.
<br />
<img src="https://i.imgur.com/Wr2PrM9.png" height="80%" width="80%" alt="local users and groups"/>
<br />
A digital certificate is a means of proving the identity of a subject, such as a user, computer, or service. The validity of each certificate is guaranteed by the issuing certification authority (CA). The Certificate Manager console (certmgr.msc) shows which certificates have been installed and provides a mechanism for requesting and importing new certificates.
<br />
<img src="https://i.imgur.com/1WA1MhJ.png" height="80%" width="80%" alt="certificate manager"/>
<br />
GUI tools such as Settings and Control Panel make changes to user profiles and the system configuration that are ultimately stored in a database called the registry. However, the registry also contains thousands of other settings that are not configurable via these tools. The Group Policy Editor (gpedit.msc) provides a more robust means of configuring many of these Windows settings than editing the registry directly. Also, vendors can write administrative templates to make third-party software configurable via policies.
<br />
<img src="https://i.imgur.com/G9qNHgn.jpg" height="80%" width="80%" alt="group editor"/>
<br />
The Windows registry provides a remotely accessible database for storing operating system, device, and software application configuration information. You can use the Registry Editor (regedit.exe) to view or edit the registry.
The registry is structured as a set of five root keys that contain computer and user databases. The HKEY_LOCAL_MACHINE (HKLM) database governs system-wide settings. The HKEY_USERS database includes settings that apply to individual user profiles, such as desktop personalization. HKEY_CURRENT_USER is a subset of HKEY_USERS with the settings for logged in user.
<br />
<img src="https://i.imgur.com/zYWa9tW.png" height="80%" width="80%" alt="group editor"/>
<br />
A Microsoft Management Console (MMC) is a container for one or more snap-ins. For example, Device Manager, Disk Management, Group Policy Editor, and Certificate Manager are all snap-ins. The mmc command allows you to perform MMC customization and create a console with a personal selection of snap-ins. The console can be saved to the Administrative Tools folder as a file with an MSC extension.
<br />
<img src="https://i.imgur.com/DmU34Cp.png" height="80%" width="80%" alt="group editor"/>
<br />
Conclusion:
Microsoft Management Consoles (MMCs) provide a standard interface for advanced configuration and management of Windows desktops and servers. You can use these consoles to manage security settings, set up scheduled tasks, and manage the disk subsystem. Additionally, when a configuration setting is not exposed in any of the normal GUI tools, you will need to use the Registry Editor to solve some types of issues.
</p>
