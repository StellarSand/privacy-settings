# Windows 11 Privacy Settings

Go to Settings.



## System

#### Notifications
- Additional settings >
  - Suggest ways to get the most out of Windows and finish setting up this device: Off
  - Get tips and suggestions when using Windows: Off

#### Nearby sharing
- Off (Enable this only when needed. Remember to turn it off when no longer required.)

#### Remote Desktop
**This feature is not available in Home editions**
- Off (Enable this only when needed. Remember to turn it off when no longer required.)
- Require device to use Network Level Authentication to connect: On



## Bluetooth & devices

#### Phone Link
Do not link

#### AutoPlay
- Use AutoPlay for all media and devices: Off



## Network & internet

#### Ethernet
- DNS server assignment > Edit >
  - Edit DNS settings: Manual
  - IPv4: On
    - Preferred DNS: enter IPv4 address of a provider from [this list](https://www.privacyguides.org/dns/)

      Example: For Quad9, enter 9.9.9.9
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
    - Alternate DNS: enter alternate IPv4 address of the same provider as above or a different provider

      Example: For Quad9, enter 149.112.112.112
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
  - IPv6: On
    - Preferred DNS: enter IPv6 address of a provider from [this list](https://www.privacyguides.org/dns/)

      Example: For Quad9, enter 2620:fe::fe
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
    - Alternate DNS: enter alternate IPv6 address of the same provider as above or a different provider

      Example: For Quad9, enter 2620:fe::9
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off

#### Wi-Fi
- Random hardware addresses: On
- Hardware properties > DNS server assignment > Edit
  - Edit DNS settings: Manual
  - IPv4: On
    - Preferred DNS: enter IPv4 address of a provider from [this list](https://www.privacyguides.org/dns/)

      Example: For Quad9, enter 9.9.9.9
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
    - Alternate DNS: enter alternate IPv4 address of the same provider as above or a different provider

      Example: For Quad9, enter 149.112.112.112
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
  - IPv6: On
    - Preferred DNS: enter IPv6 address of a provider from [this list](https://www.privacyguides.org/dns/)

      Example: For Quad9, enter 2620:fe::fe
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
    - Alternate DNS: enter alternate IPv6 address of the same provider as above or a different provider

      Example: For Quad9, enter 2620:fe::9
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off



## Personalization

#### Lock screen
- Personalize your lock screen
  - select Picture or Slideshow
  - Get fun facts, tips, tricks and more on your lock screen: Off

#### Device usage
- Turn everything off



## Apps

#### Installed apps
Uninstall anything you don't use like XBox, candy crush, some other preinstalled apps/games etc.
Be sure not to uninstall anything important. If you have doubts about any app, either ask or search the net.



## Accounts

#### Your info
Delete your account picture and set it to default.
- Choose a file > Browse files
- Go to C:\Users\Username\AppData\Roaming\Microsoft\Windows\AccountPictures and delete your picture.
- Go to C:\ProgramData\Microsoft\User Account Pictures and select any one.

NOTE: AppData is a hidden folder by default.
- To enable: in file explorer on top click View > Show > select Hidden items.

#### Sign-in options
- Show account details such as my email address on the sign-in screen: Off




## Time & language

#### Typing
- Show text suggestions when typing on the physical keyboard: Off
- Typing insights: Off



## Privacy & security

#### Windows Security
- Virus & threat protection > Virus & threat protection settings > Manage settings > All protections on (Except automatic sample submission)
- Firewall & network protection > Firewall should be on for domain, public and private networks.

#### Find my device
- Find my device: Off

#### General
- All off

#### Speech
- Online speech recognition: Off

#### Inking & typing personalization
- Personal inking and typing dictionary: Off

#### Diagnostics & feedback
- Diagnostic data > Send optional diagnostic data: Off
- Improve inking & typing: Off
- Tailored experiences: Off
- Delete diagnostic data: Delete

#### Activity history
- Send my activity history to Microsoft: Off

#### Search permissions
- Cloud content search
  - Microsoft account: Off
  - Work or School account: Off
- More settings
  - Show search highlights: Off

#### App permissions
- Review each permission and disable accordingly (choose which apps can have access to location, camera, microphone, notifications etc. If any app doesn't need something, turn it off.)
- App diagnostics > Toggle off both



## Windows Update

#### Advanced options
- Delivery Optimization > Allow downloads from other PCs: Off


---
---


## Disable ads in file explorer
Open file explorer. Click 3 dots menu on top, located to the right of "View" > Options >
  - Click "View" on top of the new popup >
    - Uncheck "Show sync provider notifications"
    - Click Apply
    - Also click "Apply to Folders" on top (if available)



## Disable telemetry service
Win key + r > type services.msc > press enter

- Double-click on "Connected User Experiences and Telemetry" >
  - Service Status: Stopped (Click on Stop, if service is running)
  - Startup Type: Disabled 
  - Click OK



## Disable trending searches & web search in search bar
Win key + r > type regedit > press enter > Yes

- Navigate to `Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Search`
- Right click > New > DWORD (32-bit) Value > name it as `BingSearchEnabled`
- Double click it and make sure "Value data" is set to 0
- Open Task Manager > Processes > select Windows Explorer > Right click > Restart