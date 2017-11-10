<span><span style="font-variant:small-caps;">Not released for distribution - Experimental use only.</span></span>

Required
========

Required to retain control of the Kindle firmware version and make the *Update Your Kindle* (UYK) menu item available.

Prevent OTA Update
------------------

In the topmost visible level of USB storage, add the OTA blocking directory name.  
The blocking directory name is:  
*update.bin.tmp.partial*  
Use that exact name, no additional extension.

Register the Kindle
-------------------

With some firmware versions, you can not access the *Update Your Kindle* (UYK) menu unless the device is registered.  
All of the KOA2 experimental <span>\*</span>.bin packages install with UYK.  
Using MrPI is not required.

Recommended
===========

The following changes are all in support of recovering the Kindle should start-up problems occur.  
Each can prevent the export of USB storage until a touch screen action is taken.  
But most start-up problems occur before the touch screen is up and working.

-   Remove any passcode protection.

-   Remove any parental controls.

-   Have special offers removed.

Check current firmware
======================

Test if the Kindle can be jail broken with the current firmware.

Note: Firmware 5.9.2 can not (yet) be jail broken.

-   Download the [Device Jail Break](https://www.adrive.com/public/U3AVtU/main-htmlviewer.tar.gz)

Do not let your PC open that archive or otherwise convert it to a *safe* archive.  
The archive content structure makes it a tar bomb, it is suppose to be a tar bomb, that is what makes it work.  
Owners of <span><span style="font-variant:small-caps;">MacOS</span></span> systems should be aware that the default settings will open and convert this archive to a *safe* archive, which prevents it from working as intended.

1.  Place in topmost visible level of USB storage.

2.  Safely remove the USB cable.

3.  In the search bar of the home screen, enter:  
    ;installHtml  
    The semi-colon is part of the command and the command is case sensitive.

4.  Did you have a *JailBroken* document appear on your Kindle?

-   Yes it did appear: The device jail break is now installed, you can skip the installation of a *Factory Use Only* firmware build.  
Continue with the section: [#Install-the-Jailbreak-Survival-Code](Install the Jailbreak Survival Code).

-   No it did not appear: To be certain, use your PC to look for it in the /documents folder.  
In this case you will have to install a *Factory Use Only* firmware build as described next.

Install a *Factory Use Only* firmware build
===========================================

In this case, the firmware version numbers before and after this step are not significant.

The use of the word *Update* means the label on the button in the settings menu, it does not describe the action performed.

1.  Download the firmware image that was intended to only be used on the factory production line: [Factory-5.9.0.6](https://www.adrive.com/public/RyfAaK/update_kindle_oasis_9th_factory_5.9.0.6.bin).

2.  Place in the topmost visible level of USB storage.

3.  Remove USB cable.

4.  Home -&gt; Menu -&gt; Settings -&gt; Menu -&gt; Update (Your Kindle - UYK)

5.  Wait.  
    Do not panic. These factory image package may take as long as 5 minutes to install.

Install Device Jail Break
=========================

Note: Customer firmware 5.9.2 can not (yet) be jail broken.

-   Download the [Device Jail Break](https://www.adrive.com/public/U3AVtU/main-htmlviewer.tar.gz)

Do not let your PC open that archive or otherwise convert it to a *safe* archive.  
The archive content structure makes it a tar bomb, it is suppose to be a tar bomb, that is what makes it work.  
Owners of <span><span style="font-variant:small-caps;">MacOS</span></span> systems should be aware that the default settings will open and convert this archive to a *safe* archive, which prevents it from working as intended.

1.  Place in topmost visible level of USB storage.

2.  Safely remove the USB cable.

3.  In the search bar of the home screen, enter:  
    ;installHtml  
    The semi-colon is part of the command and the command is case sensitive.

4.  Did you have a *JailBroken* document appear on your Kindle?

-   <span><span style="font-variant:small-caps;">Yes it did appear:</span></span> The device jail break is now installed, continue with the next section.

-   <span><span style="font-variant:small-caps;">No it did not appear:</span></span> To be certain, use your PC to look for it in the /documents folder.  
In this case something unexpected has happened, contact the developers.

Install the Jailbreak Survival Code
===================================

This package has also been known as the *hotfix* package.

This installs both the Bridge Code that auto-reinstalls the device jailbreak and it installs the application keys required to run some of the add-in applications.

-   This step may have to be repeated after every change in registration status.

1.  Download the [Jailbreak Survival Code](https://www.adrive.com/public/Srz2x2/Update_jailbreak_hotfix_1.15_koa2.bin)

2.  Place in the topmost visible level of USB storage.

3.  Safely remove the USB cable.

4.  Home -&gt; Menu -&gt; Settings -&gt; Menu -&gt; Update (Your Kindle - UYK)

5.  Watch the screen while waiting.  
    The wait should only be that involved in any package installation.

Notice
======

Any other *update\_<span>\*</span>.bin* name format package used <span><span style="font-variant:small-caps;">must</span></span> be re-installed after an Amazon update.

Only the *Device Jail Break* and components of the *Jail Break Survival Code* are auto-reinstalled.

In the usual case, KUAL extensions do not need to be re-installed, but if anything seems to be broken, re-install it.

Experimental KOA2 Packages
==========================

All of these packages are built to install using the UYK (Update Your Kindle) menu entry.

The Mobileread Package Installer (MrPI) is not required for installing these packages.

All of these are the package only, refer to the original release post for directions and/or the directions included in the corresponding archives in the listings at [NiLuJe’s Snapshots thread](https://www.mobileread.com/forums/showthread.php?t=225030)

Required
--------

With very few exceptions, these items are required.

-   KUAL Launcher Provides the application launcher menu.

    -   Release post: [Kindle Unified Application Launcher](https://www.mobileread.com/forums/showthread.php?t=203326)

    -   Install: [KUAL Booklet install](https://www.adrive.com/public/9g9eX9/Update_KUALBooklet_v2.7_koa2_nomax_install.bin)

    -   Status: Tested, Some Undescribed Problems Reported

        -   coplate: “Works for me.”

    -   Uninstall: [KUAL Booklet uninstall](https://www.adrive.com/public/3VEpNg/Update_KUALBooklet_v2.7_koa2_nomax_uninstall.bin)

    -   Status: Not Tested

Suggested
---------

-   Rescue Pack Adds SSH server to Diags system and restores the detection of ENABLE\_DIAGS in the topmost level of USB storage.

    -   Release post: .

    -   Install: .

    -   Status: Tested, Broken, Do Not Use

    -   Uninstall: Never provided.

    -   Status: N/A

-   Coward’s Rescue Pack An optional add-on to the Rescue Pack. Provides control of Rescue Pack by detecting USB cable connection.

    -   Release post: [Coward’s Rescue Pack, a Rescue Pack add-on](https://www.mobileread.com/forums/showthread.php?t=232507)

    -   Install: [Coward’s Rescue Pack install](https://www.adrive.com/public/g6WJSG/Update_crp_2.N_install_koa2_nomax.bin)

    -   Status: Not usable, requires Rescue Pack

    -   Uninstall: [Coward’s Rescue Pack uninstall](https://www.adrive.com/public/bSbTA2/Update_crp_2.N_uninstall_koa2_nomax.bin)

    -   Status: Not tested.

Available
---------

-   USB Networking Includes both ssh and telnet servers.  
Many bonus items also included.  
Note: The Amazon/Lab126 version may be included in some Factory Use firmware builds. Detail undetermined at this time.

    -   Release post: [USB Networking](https://www.mobileread.com/forums/showthread.php?t=186645)

    -   Install: [USB Networking install](https://www.adrive.com/public/DhYefd/Update_usbnet_0.21.N_install_mx7_koa2_nomax.bin)

    -   Status: Tested, working with some problems

        -   coplate: “stopping usbnetworking (with KUAL) crashes Kindle, requires a reboot”

    -   Uninstall: [USB Networking uninstall](https://www.adrive.com/public/JVtudU/Update_usbnet_0.21.N_uninstall_koa2_nomax.bin])

    -   Status: Not tested.

Packaging Tools
---------------

Tools and utilities for the examination and maintenance of *update\_<span>\*</span>.bin* packages.

-   KindleTool Binaries KindleTool both creates new and opens existing *update\_<span>\*</span>.bin* format packages. Both those of Amazon/Lab126 and those of Mobileread.

    -   Release post: [NiLuJe’s KindleTool](https://www.mobileread.com/forums/showthread.php?t=187880)

    -   Linux x86\_64: [KindleTool Linux x86\_64](https://www.adrive.com/public/WkZAZR/KindleTool-v1.6.4.108-ge16765c-linux-x86_64.zip)

    -   Status: Working, in-use

    -   Windows native 64bit<span><span style="font-variant:small-caps;">:</span></span> .

    -   Status: Not yet available.

-   Repackaging Script The script contains a table format listing of Mobileread update\_<span>\*</span>.bin packages.

    <span>Script:</span> [mkpkgs batch script](https://www.adrive.com/public/mZkvMb/mkpkgs.sh.zip)

    <span>Status:</span> Working, in use.

Historical Interest Only
------------------------

-   Old factory images Not intended to be used but may have some forensic value. Any or all of these may be corrupt.

    -   Main system: [update\_main\_5.9.0.5.1-007](https://www.adrive.com/public/DTYvtt/update-J9.0.5.1-zelda_cognac-007.bin)

    -   Main system: [update\_main\_5.9.0.5.1-008](https://www.adrive.com/public/uqYyFZ/update-J9.0.5.1-zelda_cognac-008.bin)

    -   Diag system:<span> <span style="font-variant:small-caps;"></span> </span>[update\_diags\_001.059](https://www.adrive.com/public/SaRXg2/update-J9-zelda_cognac-001.059-diags.bin)

KUAL Extensions
---------------

KUAL extensions typically are not provided in an update\_<span>\*</span>.bin name format package.  
The are distributed in archives to be un-archived to the topmost visible level of USB storage.

-   Kindle Terminal<span> <span style="font-variant:small-caps;"></span> </span>Provides an interactive, command line, terminal with on-screen keyboard.

    -   Release Post:<span> <span style="font-variant:small-caps;"></span> </span>[Terminal Emulator for Touchscreen Kindles](https://www.mobileread.com/forums/showthread.php?t=20279)

    -   Archive: [kTerm](https://www.adrive.com/public/P46YNY/kterm-kindle-2.4.zip)

    -   Status: Not tested.


