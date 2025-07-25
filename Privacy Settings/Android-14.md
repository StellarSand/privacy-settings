# Android 14 Privacy Settings

Go to Settings

**The actual location of the settings might differ from device to device. The following are according to stock android.**



## Network & internet

#### Internet
- Network preferences >
  - Turn on Wi-Fi automatically: Off
  - Notify for public networks: Off

#### Private DNS
- Private DNS > Private DNS provider hostname: enter the hostname of DNS provider from [this list](https://www.privacyguides.org/en/dns/#recommended-providers) > Save

  Example: For Quad9, enter dns.quad9.net



## Connected devices

#### Connection preferences
- Bluetooth: Off
- Printing > Default Print Service: Off
- Nearby Share > Device visibility: Off
- Android Auto: Off

> <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
>
> Enable the above settings only when required. Remember to turn them off when no longer required.



## Notifications

#### Notification history
- Use notification history: Off

#### Sensitive notifications
- Off



## Display

#### Lock screen
- Privacy: Show sensitive content only when unlocked

#### Screen timeout
- Shortest duration that suits you



## Accessibility

#### Text-to-speech output

Tap on gear icon next to `Preferred engine`

- Anonymous usage reports: Off



## Security & privacy

#### Device unlock > Screen lock
- Password, PIN or Pattern. Don't set to `None` or `Swipe`.

After setting screen lock, tap on gear icon.

- Make pattern visible: Off (only available if Screen lock is set to `Pattern`)
- Enhanced PIN privacy: On (only available if Screen lock is set to `PIN`)
- Lock after screen timeout: Immediately
- Power button instantly locks: On

#### Privacy
- Permission manager > 
    - Review each permission and disable accordingly (choose which apps can have access to camera, microphone, gps, contacts etc. If any app doesn't need something, turn it off.)
- Ads >
    - Reset advertising ID > OK
    - Opt out of Ads Personalization: On > OK
- Show passwords: Off

#### More security & privacy
- Notifications on lock screen: Show sensitive content only when unlocked
- Personalize using app data: Off
- Android System Intelligence > 
    - Customize the experience using your Google Account data: Off
    - Clear data > select `All time` > Clear data
- Autofill service from Google >
    - Use Autofill with Google: Off
- Usage & diagnostics: Off
  > <img src="../icons/ic_tip.svg" width="22" align="top"> **Tip**
  >
  > Additionally some OEMs include few more settings for personalized ads & diagnostics.
  <br>Search in your phone settings for `User Experience Program`, `Personalized ad recommendations`, `Send diagnostic data` or something similar.
- SIM card lock >
  - Lock SIM card: On > Enter default PIN > OK
  - Change SIM PIN > Enter old and new SIM PIN > OK (Create a secure new SIM PIN)
  > <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
  >
  > - The default PIN code is usually `1234` or `0000`. However, if these two don't work, you should look on SIM card's packaging or contact your SIM provider's customer support.
  > - If you enter the PIN code wrong 3 times, you'll be asked to enter a PUK (Personal Unlock Key) code. This code can be obtained from the carrier, after they verify you are the rightful owner of the SIM. DO NOT try to guess the PUK code. If you enter it wrong 3 times, the SIM will be permanently locked and you might have to get a new SIM from your carrier.
- Encryption & credentials >
  - Encrypt phone: Encrypted
- Trust agents >
  - Extend Unlock: Off



## Location
- Use location: Off (enable only when needed, like for navigation apps, and turn off when not required)

#### Location Services
- Google Location Accuracy > Improve Location Accuracy: Off
- Wi-Fi scanning: Off
- Bluetooth scanning: Off



## Google

#### Personalize using shared data
- Device Contacts: Off

#### Settings for Google apps
- Search, Assistant & Voice >
  - General >
    - Autocomplete settings > Autocomplete with trending searches: Off
    - Discover: Off
  - Privacy & Security >
    - Search customization: Off



## System

#### Multiple users
-  Add users from lock screen: Off



## Wi-Fi MAC Randomization
Go to `About phone` > tap `Build Number` 7 times. This will unlock Developer options.
<br> Now go to `System` > Developer options > Wi-fi non persistent MAC randomization: On


---


- Some other settings are same as [Google Account settings](https://github.com/StellarSand/privacy-settings/blob/main/Privacy%20Settings/Google-Account.md).
- Gboard settings are available [here](https://github.com/StellarSand/privacy-settings/blob/main/Privacy%20Settings/Gboard.md).