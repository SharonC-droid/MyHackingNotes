🐱‍💻 Installing Kali Linux on VirtualBox (Step-by-Step Guide)
🧰 Requirements :

> VirtualBox installed: https://www.virtualbox.org/
> Kali Linux ISO: Download from https://www.kali.org/get-kali/#kali-installer-images
> Minimum 4GB RAM, 20GB disk space

🪟 Step 1: Install VirtualBox
Go to VirtualBox Download Page.
Choose your host OS (e.g., Windows, macOS, Linux).
Download and install using the setup wizard.
Install Extension Pack (optional but recommended) for USB and host enhancements.

🐧 Step 2: Download Kali Linux ISO
Go to Kali Linux Downloads.
Download the Installer ISO (not VirtualBox image).
Prefer the 64-bit ISO unless your system is very old.

📦 Step 3: Create a New Virtual Machine in VirtualBox
Open VirtualBox → Click New.

Name: Kali Linux
Type: Linux
Version: Debian (64-bit)
Click Next.

💾 Step 4: Allocate RAM
Allocate at least 2 GB (2048 MB) RAM.

For smoother performance: 4096 MB (4 GB) if available.

🧱 Step 5: Create a Virtual Hard Disk
Choose Create a virtual hard disk now → Create.

File type: VDI (VirtualBox Disk Image) → Next.
Storage: Dynamically allocated → Next.
Size: 20 GB or more → Click Create.

📂 Step 6: Mount Kali Linux ISO
Select your Kali VM → Click Settings.

>Go to Storage tab.
>Under Controller: IDE, click Empty → then the disc icon → Choose a disk file.
>Select your downloaded Kali Linux ISO.
>Click OK.

🚀 Step 7: Start the Kali Linux Installation
Select the Kali VM → Click Start.

Choose Graphical Install (recommended).

Follow setup:
Language, Region, Keyboard layout
Hostname: kali
Username: Set a user and password (don’t forget it!)
Disk Partitioning: Choose Guided - use entire disk
Confirm installation and wait.

🔐 Step 8: Final Setup
After installation completes, eject ISO:

Settings → Storage → Remove disk from virtual drive.

Boot into Kali.
Login using the username and password you set.
✅ You're Done!

 ⚠️ Common Problems & Troubleshooting
❌ "Invalid settings detected" in VirtualBox
Fix:

Go to Settings → System → Enable EFI or disable Floppy.

Allocate more RAM if it’s below 2048 MB.

❌ No 64-bit option in VirtualBox
Fix:

Enable Virtualization in BIOS/UEFI:

Restart → Enter BIOS (F2/F10/Del during boot)

Enable Intel VT-x / AMD-V

Save & exit.

❌ Mouse/Keyboard not working in Kali
Fix:

Install VirtualBox Extension Pack

Reboot the VM after installing.

Enable USB 2.0 (EHCI) under Settings > USB.

 
