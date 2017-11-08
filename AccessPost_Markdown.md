*Preparation:*

a. *Prevent OTA update*
In the topmost visible level of USB storage, add the OTA blocking directory name.
The blocker directory is named:
update.bin.tmp.partial
Use that exact name, no additional extension.
b. *Required*
   * *Register the Kindle*
Without registration, you can not access the UYK (Update Your Kindle) menu entry.
*Note:* This varies with firmware version, some allow, some do not allow.
All of these experimental packages install with UYK, using MrPI is not required.
c. *Recommended*
The following changes are all in support of recovering the Kindle should start-up problems occur.
Each of them can prevent the export of USB storage until a touch screen action is taken.
But the problems occur before the touch screen is up and working.
   * Remove any pass-code protection.
   * Remove any parental controls.
   * Have Special Offers removed.
d. *Test if Kindle can be jail broken with firmware it shipped with.*
Note: Firmware 5.9.2 can not (yet) be jail broken.
Download:
Device Jail Break (https://www.adrive.com/public/U3AVtU/main-htmlviewer.tar.gz)
*DO NOT* let your PC open that archive or otherwise convert it to a "safe" archive.
Owners of MacOS systems should be aware that the default settings will open and convert this archive to a "safe" archive, which prevents it from working as intended.
   1. Place in topmost visible level of USB storage.
   2. Remove USB cable.
   3. In search bar of home screen, enter:
;installHtml
That semi-colon is part of the command and the command is case sensitive.
   4. Did you have a "JailBroken" document appear on your Kindle?
      * Yes it did appear:
The device jail break is now installed, you can skip the following step to install a "Factory Use Only" firmware build.
      * No, if did not appear (be sure, use your pc to look for it in /documents folder):
You will have to install a "Factory Use Only" firmware build as described below.


*Install "Factory Use Only" firmware build:*
If the "JailBroken" document showed up on your Kindle when you did the last item in the above section, you may skip this section.

1. *Replace your "Customer Use" firmware build with a "Factory Use Only" firmware build.*
In this case, the firmware version numbers before and after this step are not significant.
The use of the word "Update" means the label on the button in the settings menu, it does not describe the action performed.
   a. Download the firmware that was intend to only be used on the factory production line:
Factory Use Only Image (https://www.adrive.com/public/RyfAaK/update_kindle_oasis_9th_factory_5.9.0.6.bin)
   b. Place in topmost visible level of USB storage.
   c. Remove USB cable
   d. Home -> Menu -> Settings -> Menu -> Update (your Kindle)
Wait.
Do not panic, this firmware will often required as long as 5 minutes to install.
2. *Install the device jail break:*
Note: Firmware 5.9.2 can not (yet) be jail broken.
Download:
Device Jail Break (https://www.adrive.com/public/U3AVtU/main-htmlviewer.tar.gz)
*DO NOT* let your PC open that archive or otherwise convert it to a "safe" archive.
Owners of MacOS systems should be aware that the default settings will open and convert this archive to a "safe" archive, which prevents it from working as intended.
   1. Place in topmost visible level of USB storage.
   2. Remove USB cable.
   3. In search bar of home screen, enter:
;installHtml
That semi-colon is part of the command and the command is case sensitive.
   4. Did you have a "JailBroken" document appear on your Kindle?
      * Yes it did appear:
The device jail break is now installed. It is alright to continue.
      * No, if did not appear (be sure, use your pc to look for it in /documents folder):
Something unexpected has gone wrong, PM for help.


*Install the "Jailbreak Survial Code":*
This installs both the "Bridge Code" that auto-reinstalls the jailbreak and it installs the application keys required to run some of the add-in applications.
*Note:*This step should be repeated after every change in the registration status.
Download:
Jailbreak Survial Code (https://www.adrive.com/public/xpYGey/Update_jailbreak_hotfix_1.15_koa2.bin)
This is also refered to as the "hotfix" package.

1. Place in topmost visible level of USB storage.
2. Remove USB cable.
3. Home -> Menu -> Settings -> Menu -> UYK (Update Your Kindle)



=3D =3D =3D =3D

Any other *.bin package used *MUST* be re-installed after an Amazon update!
Only the jailbreak and the components of the "Jail Break Survival Code" is auto-reinstalled.

=3D =3D =3D =3D

*Experimental KOA2 Packages:*
All of these packages are built to install using UYK (Update Your Kindle) menu entry.
The Mobileread Package Installer (MrPI) is not required for installing these packages.

* *Required*
  * *KUAL Launcher*
Provides the application launcher menu.
    * Install:
KUAL Booklet Install (https://www.adrive.com/public/9g9eX9/Update_KUALBooklet_v2.7_koa2_nomax_install.bin)
    * Status: Tested, *Some Problems Reported*
      * coplate: "Works for me."
    * Uninstall:
KUAL Booklet Uninstall (https://www.adrive.com/public/3VEpNg/Update_KUALBooklet_v2.7_koa2_nomax_uninstall.bin)
    * Status: Not Tested
* *Suggested*
  * *Rescue Pack*
Adds SSH server to "Diags" system and restores the detection of: "ENABLE_DIAGS" in top of USB storage.
    * Install:
RP Install (https://www.adrive.com/public/Hkd8VF/Update_rp_20131220.N_install_koa2_nomax.bin)
    * Status: Tested - *Broken - Do Not Use*
A script to recover from a broken RP installation is in the works.
    * Uninstall: Never Provided
    * Status: N/A
  * *Coward's Rescue Pack*
An optional add-on to the Rescue Pack.
Provides control of Rescue Pack by detecting USB cable connection.
    * Install:
CRP Install (https://www.adrive.com/public/g6WJSG/Update_crp_2.N_install_koa2_nomax.bin)
    * Status: Not Tested
    * Uninstall:
CRP Uninstall (https://www.adrive.com/public/bSbTA2/Update_crp_2.N_uninstall_koa2_nomax.bin)
    * Status: Not Tested
* *Available*
  * *USB Networking*
*Note:* If running the "Factory Firmware" build, you may already have USBnetworking installed.
Details of how to use it (such as username:password pairs) are still to be discovered.
Includes both ssh and telnet servers.
Lots of bonus items also included.
    * Install:
USBnetworking Install (https://www.adrive.com/public/DhYefd/Update_usbnet_0.21.N_install_mx7_koa2_nomax.bin)
    * Status: Tested, working *with some problems*
      * coplate: "stopping usbnetworking (with KUAL) crashes the Kindle, requires a reboot"
    * Uninstall:
USBnetworking Uninstall (https://www.adrive.com/public/JVtudU/Update_usbnet_0.21.N_uninstall_koa2_nomax.bin)
    * Status: Not Tested
* *Packaging*
Tools and utilities for examination and maintenance of packaging.
  * *KindleTool binaries*
KindleTool both creates new and opens existing "update_*.bin" packages.
Both those of Amazon/Lab126 and of Mobileread.
    * Linux x86-64:
KindleTool, Linux-x86_64 (https://www.adrive.com/public/WkZAZR/KindleTool-v1.6.4.108-ge16765c-linux-x86_64.zip)
    * Status: Working, in-use
    * Windows native x86_64:
    * Status: Not yet available
  * *Batch Re-packaging Script*
Script contains a table format listing of Mobileread "update_*.bin" packages and allows the selective re-packaging of the listed packages.
Packaging parameters currently set to generate these koa2_nomax type packages.
The only documentation is the comments in the script.
    * Script:
mkpkgs batch re-packaging script (https://www.adrive.com/public/mZkvMb/mkpkgs.sh.zip)
    * Status: Working, in-use
* *Historical Interest Only*
  * *Old factory images*
    * 'Main' system:
update_main_5.9.0.5.1-007 (https://www.adrive.com/public/DTYvtt/update-J9.0.5.1-zelda_cognac-007.bin)
    * 'Main' system:
update_main_5.9.0.5.1-008 (https://www.adrive.com/public/uqYyFZ/update-J9.0.5.1-zelda_cognac-008.bin)
    * 'Diags' system:
update_diags_001.059 (https://www.adrive.com/public/SaRXg2/update-J9-zelda_cognac-001.059-diags.bin)
* *KUAL Extensions*
  * *kTerm*
Kindle Terminal
    * Archive:
kTerm (https://www.adrive.com/public/P46YNY/kterm-kindle-2.4.zip)
    * Status: Not tested.


***************

