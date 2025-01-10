# Windows 10 Privacy Settings

Go to Settings (Shortcut: `Windows key + i`).



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
- Do not link (use something else like [KDE Connect](https://kdeconnect.kde.org/), [LocalSend](https://localsend.org/), etc.)



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
Be sure not to uninstall anything important. If you have doubts about any app, search the net.



## Accounts

#### Your info
**This section is applicable only if you've signed in with a Microsoft account**

Delete your account picture and set it to default as mentioned below:
- Choose a file > Browse files
- Go to `C:\Users\JohnDoe\AppData\Roaming\Microsoft\Windows\AccountPictures` and delete your picture. (Replace `JohnDoe` with your username)
- Go to `C:\ProgramData\Microsoft\User Account Pictures` and select `guest.png`.

> :information_source: **NOTE**: `AppData` is a hidden folder by default. To enable: in file explorer on top click `View` > select `Hidden items`.

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

#### Inking & typing
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
Press `Windows key + r` > type `ncpa.cpl` > press enter

Right click on Ethernet or Wifi depending on what you are using > Properties

- Select Internet Protocol Version 4 (TCP/IPv4) > Properties > select Use the following DNS server addresses:
  - Preferred DNS server: enter IPv4 address of a provider from [this list](https://www.privacyguides.org/en/dns/#recommended-providers)

    Example: For Quad9, enter 9.9.9.9
  
  - Alternate DNS server: enter alternate IPv4 address of the same provider as above or a different provider

    Example: For Quad9, enter 149.112.112.112

  Click `OK`

- Select Internet Protocol Version 6 (TCP/IPv6) > Properties > select Use the following DNS server addresses:
  - Preferred DNS server: enter IPv6 address of a provider from [this list](https://www.privacyguides.org/en/dns/#recommended-providers)

    Example: For Quad9, enter 2620:fe::fe
  
  - Alternate DNS server: enter alternate IPv6 address of the same provider as above or a different provider

    Example: For Quad9, enter 2620:fe::9
  
  Click `OK`


---
---


## Disable ads in file explorer
Open file explorer > click `View` on top > Options > Change folder and search options
- Click `View` on top of the new popup >
  - Uncheck `Show sync provider notifications`
  - Click `Apply`
  - Also click `Apply to Folders` on top (if available)



## Disable telemetry service
Press `Windows key + r` > type `services.msc` > press enter

- Double-click on `Connected User Experiences and Telemetry` >
  - Service Status: Stopped (Click on `Stop`, if service is running)
  - Startup Type: Disabled
  - Click `OK`



## Block & uninstall Quick Assist
Reason: [Threat actors misusing Quick Assist in social engineering attacks leading to ransomware](https://www.microsoft.com/en-us/security/blog/2024/05/15/threat-actors-misusing-quick-assist-in-social-engineering-attacks-leading-to-ransomware/).

Press `Win key + r` > type `powershell` > press `ctrl + shift + enter` > Yes

- Type (or copy paste) the following in the powershell window & press enter:
  ```powershell
  notepad C:\Windows\System32\drivers\etc\hosts
  ```
- In this hosts file add the following line at the bottom & save it:
  ```
  0.0.0.0	remoteassistance.support.services.microsoft.com
  ```
- To uninstall, type (or copy paste) the following in the powershell window & press enter:
  ```powershell
  Get-AppxPackage -Name MicrosoftCorporationII.QuickAssist | Remove-AppxPackage -AllUsers
  ```



## Block all Microsoft telemetry
Press `Windows key + r` > type `powershell` > press `ctrl + shift + enter` > Yes

- Type (or copy paste) the following in the powershell window & press enter:
  ```powershell
  notepad C:\Windows\System32\drivers\etc\hosts
  ```
- Add everything from [this list](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/hosts/native.winoffice.txt) at the bottom of the hosts file & save it.

The list is updated regularly, so remember to check back often & replace old entries in the hosts file with the most recent ones.
Windows updates will function normally even with these additions.



## Disable search highlights in search bar
Right click on taskbar > Search > uncheck `Show search highlights`



## Disable trending searches & web search in search bar
<!--
Press `Win key + r` > type `regedit` > press enter > Yes

- Navigate to `Computer\HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Search`
- In the left navigation window, right click on `Search` > New > DWORD (32-bit) Value > name it `BingSearchEnabled`
- Double click it and make sure `Value data` is set to `0`
-->
Press `Windows key + r` > type `powershell` > press `ctrl + shift + enter` > Yes

- Type (or copy paste) the following in the powershell window & press enter:
  ```powershell
  New-ItemProperty -Path "HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Search" -Name "BingSearchEnabled" -Value 0 -PropertyType DWord -Force
  ```

- Open Task Manager > Processes > select `Windows Explorer` > Right click > Restart


---
---


- Microsoft 365/Office settings are available [here](https://github.com/StellarSand/privacy-settings/blob/main/Privacy%20Settings/Microsoft-365.md).
- Microsoft Edge Desktop settings are available [here](https://github.com/StellarSand/privacy-settings/blob/main/Privacy%20Settings/Microsoft-Edge.md).