# MacOS Sequoia Privacy Settings

Go to System Settings by any of the following methods:
- Apple Icon on top left > System Settings
- Spotlight Search for `System Settings` by pressing `command + space` on your keyboard.



## Apple Account

#### Sign-In & Security
- Two-Factor Authentication: On


#### iCloud
- Advanced Data Protection: On
- Access iCloud Data on the Web: Off

> :information_source: **IMPORTANT NOTE 1**: Advanced Data Protection means you'll be handling your own encryption keys. If you lose this information Apple will not be able to recover your data!
>
> :information_source: **NOTE 2**: Keep tabs on what you're using iCloud for and make sure it's only enabled for applications you need.



## Wi-Fi

#### Network Settings
- Ask to join hotsposts: Off
- Wifi Network `Details` > Private Wi-Fi address
  - `Fixed` or `Rotating` (`Fixed` will use a new, unique MAC address on that specific network. `Rotating` will cycle through new MAC addresses periodically.)



## Bluetooth
- Bluetooth: Off



## Network
- Firewall > Firewall: On
  - Options >
    - Block all incoming connections: On (**EXTREME** and **may** break many programs unless you manually exclude them.)
    - Enable stealth mode: On



## General

#### Software Update
- Automatic Updates >
  - Download new updates when available: On
  - Install macOS updates: On
  - Install application updates from the App Store: On
  - Install Security Responses and system files: On

#### AirDrop & Handoff
- Allow Handoff between this Mac and your iCloud devices: Off
- AirDrop: `No One` or `Contacts Only`
- AirPlay Receiver: Off
- Allow AirPlay for: Current User
- Require password: On

#### Login Items & Extensions
Generally keep tabs on programs and extensions in this menu and keep it as minimal as possible. 



## Siri
- Siri: Off
- Siri history: Delete Siri & Dictation History



## Notifications

#### Notification Center
- Show previews: `When Unlocked` or `Never`

## Focus
- Focus status: Off



## Privacy & Security

#### Location Services
- Location Services: Off

#### General Permissions (Calendars, Contacts, Files & Folders, Full Disk Access, HomeKit, Media & Apple Music, Passkeys Access, Photos, Reminders, etc.)
Generally keep tabs on all permissions and restrict as many as possible. The fewer permissions granted the better.

#### Analytics & Improvements
- Share Mac Analytics: Off
- Improve Siri & Dictation: Off
- Improve Assistive Voice Features: Off
- Share with app developers: Off
- Share iCloud Analytics: Off

#### Apple Advertising
- Personalized Ads: Off

#### Security
- Allow applications from: App Store
  > :information_source: **NOTE**: Malware can still be hosted on the App Store & denying other sources may heavily restrict software you can run. Enable this feature only if you don't trust other sources for installing applications.
- Allow accessories to connect: Ask Every Time
- FileVault: On
- Lockdown Mode: On



## Spotlight
- Siri Suggestions: Off
- Improve Search: Off


---
---


## Disable AI photo analysis
Open `Photos` > Settings > General (on top) >
  - Enhanced Visual Search: Off


---
---


Apple Account settings are available [here](https://github.com/StellarSand/privacy-settings/blob/main/Privacy%20Settings/Apple-Account.md).