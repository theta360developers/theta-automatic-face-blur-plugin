# Automatic Face Blur plug-in

# 1. Overview
This plug-in detects faces from spherical pictures and blur them.

# 2. Terms of Service

> You agree to comply with all applicable export and import laws and regulations applicable to the jurisdiction in which the Software was obtained and in which it is used. Without limiting the foregoing, in connection with use of the Software, you shall not export or re-export the Software into any U.S. embargoed countries (currently including, but necessarily limited to, Crimea – Region of Ukraine, Cuba, Iran, North Korea, Sudan and Syria) or to anyone on the U.S. Treasury Department’s list of Specially Designated Nationals or the U.S. Department of Commerce Denied Person’s List or Entity List.  By using the Software, you represent and warrant that you are not located in any such country or on any such list.  You also agree that you will not use the Software for any purposes prohibited by any applicable laws, including, without limitation, the development, design, manufacture or production of missiles, nuclear, chemical or biological weapons.

By using the Automatic Face Blur plug-in, you are agreeing to the above and the license terms, [license.txt](license.txt).

Copyright &copy; 2018 Ricoh Company, Ltd.

# 3. Build and Use Environment

## 3-1. Hardware

* RICOH THETA V
* Firmware ver.2.31.1 and above

    > Information on checking and updating the firmware is [here](https://theta360.com/en/support/manual/v/content/pc/pc_09.html).

## 3-2.  Development Environment

This plug-in has been built under the following conditions.

#### Operating System

* Windows&trade; 10 Version 1709
* macOS&reg; High Sierra ver.10.13

#### Development environment

* Android&trade; Studio 3.1+
* gradle 3.1.3
* Android SDK (API Level 25)
* compileSdkVersion 26
* buildToolsVersion "27.0.3"
* minSdkVersion 25
* targetSdkVersion 25

# 4. Install
Android Studio install apk after build automatically. Or use the following command after build.

```
adb install -r app-debug.apk
```

### Give permissions for this plug-in.

  Using desktop viewing app as Vysor, open Settings app and turns on the permissions at "Apps" > "Automatic Face Blur" > "Permissions"

# 5. How to Use
1. Turn on the THETA.
2. Open RICOH THETA app on your Win/Mac.
3. Set this plug-in as an active plugin from "File" > "Plug-in management..."
4. Connect THETA V to Wireless-LAN by client mode or access point mode.
   To connect THETA V to Wireless-LAN by client mode,
   for example, let's assume that there is a macOS machine,
   a THETA V and an iPhone on the same wireless LAN.  
   We also recommend that the THETA V be close to fully charged with an AC-USB adapter.
5. Set default plug-in  
   Open the THETA mobile app on an iOS/Android smartphone
   Tap "Settings" at right bottom corner  
   Confirm "Connection" is "Wi-Fi" or "Wi-Fi+Bluetooth".  
   Tap "Camera settings"  
   Tap "Plug-in"  
   Select "Automatic Face Blur"  
6. Check IP address of the camera
   Back to the Camera settings  
   Check IP-address of THETA V on smartphone app
   If you use macOS type "dns-sd -q THETAYL01234567.local" in Terminal. Here "THETAYL01234567" is an example, please change to your serial number.
7. Launch plug-in
      Press Mode button till LED2 turns white or Open from the smartphone app (RICOH THETA)

8. If you use WebUI of the plug-in,
    when you connect with THETA V by access point mode,
    open the URL (http://192.168.1.1/:8888) on the browser.
    When you connect with THETA V by client mode,
    open the URL (http://(ip-address):8888) on the browser.
    Here, (ip-address) is example. Change it to your THETA V's IP address.
9. You can set options like shooting mode, shutter speed, ISO sensitivity, White balance and EV by WebUI of the plug-in.
10. Position the camera and press the shutter button on the WebUI of the plug-in to take a picture that will be blurred.
11. If you do not use WebUI of the plug-in,
    position the camera and press the shutter button to take a picture that will be blurred.
12. Audio will sound when you press the shutter button. Audio will sound when Automatic face blur process starts and finishes.
13. Press the Mode Button more than 2 seconds to finish this plugin.

# 6. History
* ver.1.01.00 (2018/07/25): Initial version for github.
* ver.1.02.00 (2018/08/08): Bug fix.
* ver.1.03.00 (2018/10/05): Bug fix.
* ver.1.04.00 (2018/11/05): Check remaining space of Theta.
* ver.1.05.00 (2018/12/04): Terminate the plug-in when there is no space for Theta to take picture.

---

## Trademark Information

The names of products and services described in this document are trademarks or registered trademarks of each company.

* Android, Nexus, Google Chrome, Google Play, Google Play logo, Google Maps, Google+, Gmail, Google Drive, Google Cloud Print and YouTube are trademarks of Google Inc.
* Apple, Apple logo, Macintosh, Mac, Mac OS, OS X, AppleTalk, Apple TV, App Store, AirPrint, Bonjour, iPhone, iPad, iPad mini, iPad Air, iPod, iPod mini, iPod classic, iPod touch, iWork, Safari, the App Store logo, the AirPrint logo, Retina and iPad Pro are trademarks of Apple Inc., registered in the United States and other countries. The App Store is a service mark of Apple Inc.
* Microsoft, Windows, Windows Vista, Windows Live, Windows Media, Windows Server System, Windows Server, Excel, PowerPoint, Photosynth, SQL Server, Internet Explorer, Azure, Active Directory, OneDrive, Outlook, Wingdings, Hyper-V, Visual Basic, Visual C ++, Surface, SharePoint Server, Microsoft Edge, Active Directory, BitLocker, .NET Framework and Skype are registered trademarks or trademarks of Microsoft Corporation in the United States and other countries. The name of Skype, the trademarks and logos associated with it, and the "S" logo are trademarks of Skype or its affiliates.
* Wi-Fi™, Wi-Fi Certified Miracast, Wi-Fi Certified logo, Wi-Fi Direct, Wi-Fi Protected Setup, WPA, WPA 2 and Miracast are trademarks of the Wi-Fi Alliance.
* The official name of Windows is Microsoft Windows Operating System.
* All other trademarks belong to their respective owners.

![Analytics](https://ga-beacon.appspot.com/UA-73311422-5/face-blur)

