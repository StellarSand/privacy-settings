# Windows 10 Privacy Settings

Go to Settings.



## System

#### Notifications & actions
- Show notifications on the lock screen: Off
- Show reminders and incoming VoIP calls on the lock screen: Off
- Suggest ways I can finish setting up my device to get the most out of Windows: Off
- Get tips, tricks and suggestions as you use Windows: Off

#### Shared experiences
- Nearby sharing: Off (Enable this only when needed. Remember to turn it off when no longer required.)
- Share across devices: Off

#### Remote Desktop
**This feature is not available in Home editions**
- Off (Enable this only when needed. Remember to turn it off when no longer required.)
- Require device to use Network Level Authentication to connect: On



## Devices

#### Typing
- Spelling
  - Autocorrect misspelled words: Off
  - Highlight misspelled word: Off
- Typing
  - Show text suggestions as I type on the software keyboard: Off
- Hardware keyboard
  - Show text suggestions as I type: Off
  - Autocorrect misspelled words I type: Off
- Multilingual text suggestions
  - Show text suggestions based on the recognized languages you're typing in: Off

#### AutoPlay
- Use AutoPlay for all media and devices: Off


## Phone
Do not link



## Network & Internet

#### Wi-Fi
- Random hardware addresses (if available): On



## Personalization

#### Lock screen
- Background: select Picture or Slideshow
- Get fun facts, tips, tricks and more on your lock screen: Off

#### Start
- Show suggestions occasionally in Start: Off



## Apps

#### Apps & features
Uninstall anything you don't use like XBox, candy crush, some other preinstalled apps/games etc.
Be sure not to uninstall anything important. If you have doubts about any app, either ask or search the net.



## Accounts

#### Your info
Delete your account picture and set it to default. Under Create your picture, click on Browse for one.
- Go to C:\Users\Username\AppData\Roaming\Microsoft\Windows\AccountPictures and delete your picture.
- Go to C:\ProgramData\Microsoft\User Account Pictures and select any one.

NOTE: AppData is a hidden folder by default.
- To enable: in file explorer on top click View > select Hidden items.

#### Sign-in options
- Require sign-in: When PC wakes up from sleep
- Privacy
  - Show account details such as my email address on the sign-in screen: Off



## Search

#### Permissions & History
- Cloud content search
  - Microsoft account: Off
  - Work or school account: Off
- History
  - Search history on this device: Off
  - Clear device search history



## Privacy

#### General
- All off

#### Speech
- Online speech recognition: Off

#### Inking & typing personalization
- Getting to know you: Off

#### Diagnostics & feedback
- Diagnostic data: Required diagnostic data
- Improve inking & typing recognition: Off
- Tailored experiences: Off
- Delete diagnostic data: Delete

#### Activity history
- Send my activity history to Microsoft: Off

#### App permissions
- Review each permission and disable accordingly (choose which apps can have access to camera, microphone, gps, notifications etc. If any app doesn't need something, turn it off.)
- App diagnostics > Change > Off



## Update & Security

#### Delivery Optimization
- Allow downloads from other PCs: Off

#### Windows Security

- Virus & threat protection > Virus & threat protection settings > Manage settings > All protections on (Except automatic sample submission)
- Firewall & network protection > All firewalls should be on for domain, public and private networks.



## Encrypted DNS
Win key + r > type ncpa.cpl > press enter

Right click on Ethernet or Wifi depending on what you are using > Properties

- Select Internet Protocol Version 4 (TCP/IPv4) > Properties > select Use the following DNS server addresses:
  - Preferred DNS server: enter IPv4 address of a provider from [this list](https://www.privacyguides.org/dns/)

    Example: For Quad9, enter 9.9.9.9
  
  - Alternate DNS server: enter alternate IPv4 address of the same provider as above or a different provider

    Example: For Quad9, enter 149.112.112.112

  Click OK

- Select Internet Protocol Version 6 (TCP/IPv6) > Properties > select Use the following DNS server addresses:
  - Preferred DNS server: enter IPv6 address of a provider from [this list](https://www.privacyguides.org/dns/)

    Example: For Quad9, enter 2620:fe::fe
  
  - Alternate DNS server: enter alternate IPv6 address of the same provider as above or a different provider

    Example: For Quad9, enter 2620:fe::9
  
Click OK