# MacOS Sequoia Privacy Settings

Go to System Settings by any of the following methods:
- Apple Icon on top left > System Settings
- Spotlight Search for `System Settings` by pressing `command + space` on your keyboard.



## Apple Account

#### Sign-In & Security
- Two-Factor Authentication: On


#### iCloud
- Advanced Data Protection: On
  > <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
  >
  > Advanced Data Protection means you'll be handling your own encryption keys. If you lose this information Apple will not be able to recover your data!
- Access iCloud Data on the Web: Off
  > <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
  >
  > Keep tabs on what you're using iCloud for and make sure it's only enabled for applications you need.



## Wi-Fi

#### Network Settings
- Ask to join hotspots: Off
- Wifi Network `Details` >
  - Private Wi-Fi address: Rotating
    > <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
    >
    > `Rotating` will cycle through new MAC addresses periodically. `Fixed` will use a new, unique MAC address on that specific network.
  - Limit IP address tracking: On



## Bluetooth
- Bluetooth: Off



## Network
- Firewall > Firewall: On
  - Options >
    - Block all incoming connections: On
      > <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
      >
      > **EXTREME** and **may** break many programs unless you manually exclude them.
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



## Apple Intelligence & Siri
- Apple Intelligence: Off > Turn Off Apple Intelligence
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
  > <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
  >
  > Malware can still be hosted on the App Store & denying other sources may heavily restrict software you can run. Enable this feature only if you don't trust other sources for installing applications.
- Allow accessories to connect: Ask Every Time
- FileVault: On
- Lockdown Mode: On



## Spotlight
- Siri Suggestions: Off
- Improve Search: Off


---


## Disable AI photo analysis
Open `Photos` > Settings > General (on top) >
  - Enhanced Visual Search: Off



## Block all Apple telemetry
- Spotlight Search for `terminal` & open it.
- Type (or copy & paste) the following in the terminal window & press enter:
  ```zsh
  sudo nano /etc/hosts
  ```
- Type your password & press enter.
- Use the down arrow key on your keyboard to move the cursor to the bottom of the hosts file.
- Copy & paste everything from [this list](https://raw.githubusercontent.com/hagezi/dns-blocklists/refs/heads/main/hosts/native.apple.txt) at the bottom of the hosts file & save it.
  > <img src="../icons/ic_tip.svg" width="22" align="top"> **Tip**
  >
  > To save the file press `Ctrl + x`, type `y`, press enter.
- Type (or copy & paste) the following in the terminal window & press enter:
  ```zsh
  dscacheutil -flushcache
  ```

The list is updated regularly, so remember to check back often & replace old entries in the hosts file with the most recent ones.
macOS updates will function normally even with these additions.


---


Apple Account settings are available [here](https://github.com/StellarSand/privacy-settings/blob/main/Privacy%20Settings/Apple-Account.md).