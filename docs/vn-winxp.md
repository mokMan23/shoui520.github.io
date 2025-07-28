# Running Old Visual Novels on Windows XP
Occasionally, you'll find VNs that either have compatibility issues, or won't work at all in modern versions of Windows.
Note: This guide assumes you know how to create VMs, and will only focus on Windows XP. These steps can also be followed if you have hardware capable of running XP.

## Requirements
	
Virtualization Software (e.g. QEMU or Oracle VM VirtualBox) & AMD-V/VT-x enabled

Windows XP ISO & Product Key - Google is your friend, SP3 Professional VL ISOs are highly recommended.

## Setup

At least 512MB is recommended for a basic XP SP3 install, 1-2 GB for networking. You shouldn't need more than 2GB.

Disable networking in your Virtualization software unless you plan to update XP and go online.

1. You will be greeted with a blue installation screen. Follow the instructions until you're asked to format your drive. Choose NTFS ("Quick" format, if it's available) 
2. During the graphical phase of installation, you'll see `Regional and Language Options`. When this window appears, click `Customize`. In the window that pops up, click on the `Languages` tab on the top left and check `Install files for East Asian Languages`. Click `OK` and click on the `Regional Options` tab. Set `Standards and Formats` to `Japanese`, and `Location` to `Japan`.  Lastly, click on the `Advanced` tab and change `Language for non-Unicode Programs` to `Japanese`. Click `OK`, and wait for the files to install. 

Some VNs check your format, location, and time zone as a method of region-locking. A non-Japanese locale on your system will break text, showing garbage instead. Note that multilingual programs will now default to Japanese. If you still want/need English standards & formats, create another user.

3. Enter your Name, Company (can be anything), and Product Key.
4. Change your `Time Zone` to `(GMT +9:00) Osaka, Sapporo, Tokyo`. Wait until you reboot.

	4.1. If you set up networking, you'll be asked to configure it. Customize these settings as necessary, or click `Next` twice and wait for your system to reboot.

5. Before the OOBE starts, you'll see a window. Click `OK`, then `Next` to apply the resolution change. 
6. In the OOBE (Out-of-Box Experience): Click `Next` twice.

	6.1. If the OOBE detects your Network, you'll be asked about how your network is configured and whether you want to activate Windows (on a retail copy of XP). Select `Yes, this computer will connect through a local area network or home network` and `No, remind me every few days` (for retail copies of XP), as online activation is broken. Click `Next`. Fill in `Your Name` (the Administrator account) and other users' names as necessary, click `Next`, then `Finish`.

6. Wait until the welcome screen shows. Nostalgic, isn't it?
7. (Optional) To get rid of the annoying "Your PC may be at risk" balloon, click on the red X shield on your Taskbar, then click `Recommendations...` under `Virus Protection`. Check `I have an antivirus program that I'll monitor myself` and click OK.
Congratulations, you now have a VN-ready XP install!
## Optional Software
[MacType](https://github.com/snowie2000/mactype/releases/download/2019.1-beta6/MacTypeInstaller_2019.1-beta6.exe) - Fix pixelated CJK font. Use registry mode. :slight_smile:  

[Legacy Update](https://legacyupdate.net/) - Updates your system to XP's EOL point (POSReady 2009, too, if you enable it)

[xp_activate32](https://archive.org/download/xp_activate32_202305/xp_activate32.zip) - Activates retail copies of XP

[Supermium](https://www.win32subsystem.live/supermium/) - Modern Chromium on Windows XP

[MyPal](https://github.com/Feodor2/Mypal68/releases/latest) - Firefox-based browser for Windows XP, less resource intensive than Supermium

## Using ITHVNR for text hooking
[ITHVNR](https://drive.proton.me/urls/C2QY84DYX0#vRIWAHdwnAb0) is an XP-supported alternative of Texthooker. Install [Visual C++ Redistributable 2013](https://aka.ms/highdpimfc2013x86enu) first, then extract the RAR file using [7-Zip](https://www.7-zip.org/). 

From now on, you can either use shared clipboards (if your virtualization software *supports* it) and use your host OS for Yomitan reading practice, or do it all inside the VM. Here's examples of


### The former
![Image](img/winxp1.jpg)
![Image](img/winxp2.jpg)  
### and the latter.
(add image here)

If you choose the former, the tutorial ends here. For those choosing the latter, download the old 

<h3>Found this useful? Consider supporting me on Patreon!</h3>   

[:fontawesome-brands-patreon: Support me on Patreon](https://www.patreon.com/shoui){: .md-button }
