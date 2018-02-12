Firmware versions
=================

The process described here applies to only two firmware versions.

If the Kindle has either of these versions installed when first taken out of the box:

-   5.9.0.5.1

-   5.9.2.0.1

Then this process should work.

Highly recommended
==================

To retain control of the Kindle firmware version, in the topmost visible level of USB storage, add the OTA blocking directory name. The blocking directory name is:
*update.bin.tmp.partial*
Use that exact name, no additional extension.

There is no guarantee that this will block the download of an OTA update.

There have not been any firmware versions reported (yet) that can over-ride this blocking.

It is possible that Amazon/Lab126 will change this situation at any time, without notice.

Recommended
===========

The following changes are all in support of recovering the Kindle should start-up problems occur.

Each can prevent the export of USB storage until a touch screen action is taken. Most start-up problems occur before the touch screen is up and working.

-   Register the Kindle.

-   Remove any passcode protection.

-   Remove any parental controls.

-   Have special offers removed.

Install a *Factory Use Only* firmware build
===========================================

The firmware version numbers before and after this step are not significant.

The use of the word *Update* means the label on the button in the settings menu, it does not describe the action performed.

1.  Download the firmware image that was intended to only be used on the factory production line: [Factory-5.9.0.6](https://www.adrive.com/public/RyfAaK/update_kindle_oasis_9th_factory_5.9.0.6.bin).

2.  md5sum: 18624db8c1838ec2b5b8bfb3406ac041

3.  Place in the topmost visible level of USB storage.

4.  Remove USB cable.

5.  Home -&gt; Menu -&gt; Settings -&gt; Menu -&gt; Update (Your Kindle - UYK)

6.  Wait.
    Do not panic. This factory image package may take as long as 5 minutes to install.

Install Device Jail Break
=========================

Customer firmware versions other than the two listed above can not (yet) be jail broken.

-   Download the [Device Jail Break](https://www.adrive.com/public/U3AVtU/main-htmlviewer.tar.gz)

Do not let your PC open the archive or otherwise convert it to a *safe* archive. The archive content structure makes it a tar bomb, it is suppose to be a tar bomb, that is what makes it work. Owners of <span><span style="font-variant:small-caps;">MacOS</span></span> systems should be aware that the default settings will open and convert this archive to a *safe* archive, which prevents it from working as intended.

1.  md5sum: 8d4ef0528bc1d72576b890a72840780a
    This value will match if the download was without error and if your PC has not tried to safely re-pack it.

2.  Place in topmost visible level of USB storage.

3.  Safely remove the USB cable.

4.  In the search bar of the home screen, enter:
    ;installHtml
    The semi-colon is part of the command and the command is case sensitive.

5.  Did you have a *JailBroken* document appear on your Kindle?

-   <span><span style="font-variant:small-caps;">Yes it did appear:</span></span> The device jail break is now installed, continue with the next section.

-   <span><span style="font-variant:small-caps;">No it did not appear:</span></span> To be certain, use your PC to look for it in the /documents folder. In this case something unexpected has happened, contact the developers.

Install the Jailbreak Survival Code
===================================

This package has also been known as the *hotfix* package.

This installs both the Bridge Code that auto-reinstalls the device jailbreak and it installs the application keys required to run some of the add-in applications.

-   This step may have to be repeated after every change in registration status.

1.  Download the [Jailbreak Survival Code](https://www.adrive.com/public/Srz2x2/Update_jailbreak_hotfix_1.15_koa2.bin)

2.  md5sum: 19857c59d350470afff27f4249be8bac

3.  Place in the topmost visible level of USB storage.

4.  Safely remove the USB cable.

5.  Home -&gt; Menu -&gt; Settings -&gt; Menu -&gt; Update (Your Kindle - UYK)

6.  Watch the screen while waiting.
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

Available
---------

-   USB Networking Includes both ssh and telnet servers. Many bonus items also included. Note: Without an application launcher (KUAL), you will have to use the ;un searchbar command to toggle between USBnetworking and USBmass storage modes.

    -   Release post: [USB Networking](https://www.mobileread.com/forums/showthread.php?t=186645)

    -   Install: [USB Networking install](https://www.adrive.com/public/DhYefd/Update_usbnet_0.21.N_install_mx7_koa2_nomax.bin)

    -   Status: Tested, working.

    -   Uninstall: [USB Networking uninstall](https://www.adrive.com/public/JVtudU/Update_usbnet_0.21.N_uninstall_koa2_nomax.bin])

    -   Status: Not tested.

Packaging Tools
---------------

Tools and utilities for the examination and maintenance of *update\_<span>\*</span>.bin* packages.

-   KindleTool Binaries KindleTool both creates new and opens existing *update\_<span>\*</span>.bin* format packages. Both those of Amazon/Lab126 and those of Mobileread.

    -   Release post: [NiLuJe’s KindleTool](https://www.mobileread.com/forums/showthread.php?t=187880)

    -   Current builds: [KindleTool for Linux, MacOS and Windows](https://www.mobileread.com/forums/showthread.php?t=225030)

    -   Status: Working, in-use

-   Repackaging Script The script contains a table format listing of Mobileread update\_<span>\*</span>.bin packages.

    <span>Script:</span>  
    [mkpkgs batch script](https://www.adrive.com/public/mZkvMb/mkpkgs.sh.zip)

    <span>Status:</span>  
    Working, in use.

KUAL Extensions
---------------

Since a usable version of KUAL does not exist, KUAL extensions must be started using the searchbar command: ;log runme along with a custom script in USB storage.

A collection of “RUNME.sh” scripts is being made in this thread: [Collection of runme scripts](https://www.mobileread.com/forums/showthread.php?t=292382)

-   Kindle Terminal<span> <span style="font-variant:small-caps;"></span> </span>Provides an interactive, command line, terminal with on-screen keyboard.

    -   Release Post:<span> <span style="font-variant:small-caps;"></span> </span>[Terminal Emulator for Touchscreen Kindles](https://www.mobileread.com/forums/showthread.php?t=179286)

    -   Public repository: [Source code repository](https://github.com/bfabiszewski/kterm)

    -   Archive: [kTerm](https://www.adrive.com/public/P46YNY/kterm-kindle-2.4.zip)

    -   md5sum: 5f943d7928d6fa206514241a7f245081

    -   Status: A working runme script has been contributed.


