# Windows 11 Privacy Settings

Go to Settings (Shortcut: `Windows key + i`).



## System

#### Notifications
- Additional settings >
  - Show the Windows welcome experience after updates and when signed in to show what's new and suggested: Off
  - Suggest ways to get the most out of Windows and finish setting up this device: Off
  - Get tips and suggestions when using Windows: Off

#### Nearby sharing
- Off (Enable this only when needed. Remember to turn it off when no longer required.)

#### Remote Desktop
**This feature is not available in Home editions**
- Off (Enable this only when needed. Remember to turn it off when no longer required.)
- Require device to use Network Level Authentication to connect: On



## Bluetooth & devices

#### Mobile devices
- Phone Link : Off (use something else like [KDE Connect](https://kdeconnect.kde.org/), [LocalSend](https://localsend.org/), etc.)

#### AutoPlay
- Use AutoPlay for all media and devices: Off

## Network & internet

#### Ethernet
- DNS server assignment > Edit >
  - Edit DNS settings: Manual
  - IPv4: On
    - Preferred DNS: enter IPv4 address of a provider from [this list](https://www.privacyguides.org/en/dns/#recommended-providers)

      Example: For Quad9, enter 9.9.9.9
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
    - Alternate DNS: enter alternate IPv4 address of the same provider as above or a different provider

      Example: For Quad9, enter 149.112.112.112
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
  - IPv6: On
    - Preferred DNS: enter IPv6 address of a provider from [this list](https://www.privacyguides.org/en/dns/#recommended-providers)

      Example: For Quad9, enter 2620:fe::fe
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
    - Alternate DNS: enter alternate IPv6 address of the same provider as above or a different provider

      Example: For Quad9, enter 2620:fe::9
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off

  Click `Save`

#### Wi-Fi
- Random hardware addresses: On
- Hardware properties > DNS server assignment > Edit
  - Edit DNS settings: Manual
  - IPv4: On
    - Preferred DNS: enter IPv4 address of a provider from [this list](https://www.privacyguides.org/en/dns/#recommended-providers)

      Example: For Quad9, enter 9.9.9.9
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
    - Alternate DNS: enter alternate IPv4 address of the same provider as above or a different provider

      Example: For Quad9, enter 149.112.112.112
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
  - IPv6: On
    - Preferred DNS: enter IPv6 address of a provider from [this list](https://www.privacyguides.org/en/dns/#recommended-providers)

      Example: For Quad9, enter 2620:fe::fe
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off
    - Alternate DNS: enter alternate IPv6 address of the same provider as above or a different provider

      Example: For Quad9, enter 2620:fe::9
    - DNS over HTTPS: On (automatic template)
    - Fallback to plaintext: Off

  Click `Save`



## Personalization

#### Lock screen
- Personalize your lock screen
  - select `Picture` or `Slideshow`
  - Get fun facts, tips, tricks and more on your lock screen: Off

#### Start
- Show recommendations for tips, shortcuts, new apps and more: Off

#### Device usage
- Turn everything off



## Apps

#### Installed apps
Uninstall anything you don't use like XBox, candy crush, some other preinstalled apps/games etc.
Be sure not to uninstall anything important. If you have doubts about any app, search the net.



## Accounts

#### Your info
**This section is applicable only if you've signed in with a Microsoft account**

Delete your account picture and set it to default as mentioned below:
- Choose a file > Browse files
- Go to `C:\Users\JohnDoe\AppData\Roaming\Microsoft\Windows\AccountPictures` and delete your picture. (Replace `JohnDoe` with your username)
- Go to `C:\ProgramData\Microsoft\User Account Pictures` and select `guest.png`.

> :information_source: **NOTE**: `AppData` is a hidden folder by default. To enable: in file explorer on top click `View` > Show > select `Hidden items`.

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

#### Recall & Snapshots
**This feature is available only on some devices**
- Save Snapshots: Off
- Delete Snapshots >
  - Delete all snapshots: Delete all

#### Speech
- Online speech recognition: Off

#### Inking & typing personalization
- Custom inking and typing dictionary: Off

#### Diagnostics & feedback
- Diagnostic data > Send optional diagnostic data: Off
- Improve inking & typing: Off
- Tailored experiences: Off
- Delete diagnostic data: Delete
- Feedback frequency: Never

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
- App diagnostics > App diagnostic access: Off



## Windows Update

#### Advanced options
- Delivery Optimization > Allow downloads from other PCs: Off


---
---


## Disable ads in file explorer
Open file explorer. Click 3 dots menu on top > Options >
  - Click `View` on top of the new popup >
    - Uncheck `Show sync provider notifications`
    - Click `Apply`
    - Also click "Apply to Folders" on top (if available)



## Disable telemetry service
Press `Win key + r` > type `services.msc` > press enter

- Double-click on `Connected User Experiences and Telemetry` >
  - Service Status: Stopped (Click on `Stop`, if service is running)
  - Startup Type: Disabled 
  - Click `OK`



## Block & uninstall Quick Assist
Reason: [Threat actors misusing Quick Assist in social engineering attacks leading to ransomware](https://www.microsoft.com/en-us/security/blog/2024/05/15/threat-actors-misusing-quick-assist-in-social-engineering-attacks-leading-to-ransomware/).

Press `Win key + r` > type `powershell` > press `ctrl + shift + enter` > Yes

- Type (or copy paste) the following in the powershell window & press enter:
  ```Powershell
  notepad C:\Windows\System32\drivers\etc\hosts
  ```
- In this hosts file add the following line at the bottom & save it:
  ```
  0.0.0.0	remoteassistance.support.services.microsoft.com
  ```
- To uninstall, type (or copy paste) the following in the powershell window & press enter:
  ```Powershell
  Get-AppxPackage -Name MicrosoftCorporationII.QuickAssist | Remove-AppxPackage -AllUsers
  ```



## Block all Microsoft telemetry
Press `Win key + r` > type `powershell` > press `ctrl + shift + enter` > Yes

- Type (or copy paste) the following in the powershell window & press enter:
  ```Powershell
  notepad C:\Windows\System32\drivers\etc\hosts
  ```
- Add everything from [this list](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/hosts/native.winoffice.txt) at the bottom of the hosts file & save it.

The list is updated regularly, so remember to check back often & replace old entries in the hosts file with the most recent ones.
Windows updates will function normally even with these additions.



## Disable trending searches & web search in search bar
<!--
Press `Win key + r` > type `regedit` > press enter > Yes

- Navigate to `Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Search`
- In the left navigation window, right click on `Search` > New > DWORD (32-bit) Value > name it `BingSearchEnabled`
- Double click it and make sure `Value data` is set to `0`
-->

Press `Win key + r` > type `powershell` > press `ctrl + shift + enter` > Yes

- Type (or copy paste) the following in the powershell window & press enter:
  ```Powershell
  New-ItemProperty -Path "HKCU:\Software\Microsoft\Windows\CurrentVersion\Search" -Name "BingSearchEnabled" -Value 0 -PropertyType DWord -Force
  ```

- Open Task Manager > Processes > select `Windows Explorer` > Right click > Restart



## Disable Copilot
<!-- 
Press `Win key + r` > type `regedit` > press enter > Yes

- Navigate to `Computer\HKEY_CURRENT_USER\Software\Policies\Microsoft\Windows`
- In the left navigation window, right click on `Windows` > New > Key > name it `WindowsCopilot`
- Right click on `WindowsCopilot` > New > DWORD (32-bit) Value > name it `TurnOffWindowsCopilot`
- Double click it and set `Value data` to `1` > OK
-->

Press `Win key + r` > type `powershell` > press `ctrl + shift + enter` > Yes

- Type (or copy paste) the following in the powershell window & press enter:
  ```Powershell
  New-Item -Path "HKCU:\Software\Policies\Microsoft\Windows" -Name "WindowsCopilot" -Force; New-ItemProperty -Path "HKCU:\Software\Policies\Microsoft\Windows\WindowsCopilot" -Name "TurnOffWindowsCopilot" -Value 1 -PropertyType DWord -Force
  ```

- Open Task Manager > Processes > select `Windows Explorer` > Right click > Restart


---
---


- Microsoft 365/Office settings are available [here](https://github.com/StellarSand/privacy-settings/blob/main/Privacy%20Settings/Microsoft-365.md).
- Microsoft Edge Desktop settings are available [here](https://github.com/StellarSand/privacy-settings/blob/main/Privacy%20Settings/Microsoft-Edge.md).


---
---


## Fresh install

#### Block preinstalled third-party bloatware
- In the installation media setup wizard, select `Time and currency format` as `English (World)`.
- Once the device restarts, an error (`Something went wrong`) will be displayed. Click on `Skip` & continue with the rest of the setup.
- After the whole setup completes & the device boots into Windows 11, go to Settings > Time & language > Language & region > Country or region: select your country/region

#### Bypass Microsoft account requirement
After the installation media setup wizard completes & the device begins to restart, disconnect your internet connection (even if you're unable to disconnect for any reason, keep following the process).
<br>After the device restarts, it'll reach the country or region selection screen.
- Press `Shift + F10`. On some devices you may require to press `Fn + Shift + F10`.
- In the command prompt, type the following & press enter:
  ```cmd
  oobe\bypassnro
  ```
  Your device will restart.
- If for some reason you were unable to disconnect from the internet earlier, press `Shift + F10` or `Fn + Shift + F10` again. In the command prompt, type the following & press enter:
  ```cmd
  ipconfig /release
  ```
- Select `I don't have internet` & continue with the local account creation.
- If you used `ipconfig /release` command previously, once the whole setup process is complete:
  - Press `Win key + r` > type `cmd` & press enter.
  - In the command prompt, type the following & press enter:
    ```cmd
    ipconfig /renew
    ```