# Visual novels on a Windows XP Virtual Machine

Some old visual novels will refuse to run on modern versions of Windows. For special cases like these you need to run Windows XP in order to play them. This guide will *not* cover setting up the VM itself, only Windows XP with a few helpful tips for VM creation.

## Requirements
	
Virtualization Software (e.g. QEMU or Oracle VM VirtualBox) & AMD-V/VT-x enabled

Windows XP ISO & Product Key - Google is your friend, SP3 VL ISOs are highly recommended.

## Setup

At least 512MB is recommended for SP3 XP, preferably 1GB.
Disable networking in your Virtualization software unless you plan to update XP, and a faster setup.

1. You will be greeted with a blue installation screen. Follow the instructions until you're asked to reboot.
2. During the graphical phase of installation, you'll see `Regional and Language Options`. When this window appears, click `Customize`. In the window that pops up, set `Standards and Formats` to `Japanese`, and `Location` to `Japan`. Go to the `Languages` tab and check `Install files for East Asian Languages`. Lastly, go to the `Advanced` tab and change `Language for non-Unicode Programs` to `Japanese`. Click `OK`, and wait for the files to install.
3. Enter your Name, Company (can be anything), and Product Key.
4. Change your `Time Zone` to `(GMT +9:00) Osaka, Sapporo, Tokyo`. Wait until you reboot.
5. Before the OOBE starts, you'll see a window. Click `OK`, then `Next` to apply the resolution change. Click `Next`, `Not right now`, and `Next`. Enter `Your Name`, click `Next`, then `Finish`.
6. Wait until Windows XP boots. Nostalgic, isn't it?
7. (Optional) To get rid of the annoying "Your PC may be at risk" balloon, click on the red X shield on your Taskbar, then click `Recommendations...` under `Virus Protection`. Check `I have an antivirus program that I'll monitor myself` and click OK.
Now, go and install some software. I recommend you download these on your actual PC and just drag and drop it into your VM.  
		[7-Zip (32 bit)](https://www.7-zip.org/)  	
		[ITHVNR](https://drive.proton.me/urls/C2QY84DYX0#vRIWAHdwnAb0) - because Textractor is not supported on XP. Install vcredist_x86 to make it work.  
		[MacType](https://github.com/snowie2000/mactype/releases/download/2019.1-beta6/MacTypeInstaller_2019.1-beta6.exe) - Fix pixelated CJK font. Use registry mode. :slight_smile:  
		[Legacy Update](https://legacyupdate.net/) - Updates your system 
30. In "Devices" enable bidirectional clipboard.
31. Download your visual novel of choice and drag and drop it to your VM. If it needs to be installed, then install it.
32. Open ITHVNR and your VN. In ITHVNR, go in "Process", find the process of the VN, then click "Attach" and "OK"
33. Advance some text in the VN. Now cycle through the hooks in ITHVNR and find the right hook.
34. ITHVNR will automatically copy text to your clipboard, which is shared with your actual PC. I recommend you use [Yomichan](/yomichan)'s clipboard monitor :)
35. Phew, that's pretty much it, have fun!
![Image](img/winxp1.jpg)
*from vm*
![Image](img/winxp2.jpg)  
*from actual pc*  

<h3>Found this useful? Consider supporting me on Patreon!</h3>   

[:fontawesome-brands-patreon: Support me on Patreon](https://www.patreon.com/shoui){: .md-button }
