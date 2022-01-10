# Android 10 Privacy Settings

Go to Settings

**The actual location of the settings might differ from device to device. The following are according to stock android.**



## Network & internet

#### Wi-Fi
- Tap gear icon associated with the Wi-Fi > Advanced > Privacy > Use randomized MAC
- Wi-Fi preferences > 
  - Turn on Wi-Fi automatically: Off
  - Notify for public networks: Off

#### Advanced
- Private DNS > Private DNS provider hostname: enter the appropriate tls_auth_name from [this list](https://privacyguides.org/providers/dns/) > Save



## Connected devices

#### Connection preferences
- Bluetooth: Off
- Printing > Default Print Service: Off
- Nearby Share >
  - Off
  - Device visibility: Hidden
- Android Auto: Off

NOTE: Enable the above settings only when needed. Remember to turn them off when no longer required.



## Apps & notifications

#### Notifications
- Sensitive notifications: Off

#### Permission manager
- Review each permission and disable accordingly (choose which apps can have access to camera, microphone, gps, contacts etc. If any app doesn't need something, turn it off.)



## Display

#### Advanced
- Screen timeout: Shortest duration that suits you
- Lock screen display > Lock screen: Show sensitive content only when unlocked



## Privacy

#### Permission manager
- Review each permission and disable accordingly (choose which apps can have access to camera, microphone, gps, contacts etc. If any app doesn't need something, turn it off.)

#### Show passwords
- Off

#### Lock Screen
- Show sensitive content only when unlocked

#### Autofill service from Google
- Off

#### Ads
- Reset advertising ID > OK
- Opt out of Ads Personalization: On > OK

#### Usage and diagnostics
- Off

NOTE: Additionally some OEMs might include few more settings for personalized ads & diagnostics.

Search in your phone settings for "User Experience Program", "Personalized ad recommendations", "Send diagnostic data" or something similar.



## Location
- Use location: Off (enable only when needed, like for navigation apps, and turn off when not required)

#### Wi-Fi and Bluetooth scanning
- Wi-Fi scanning: Off
- Bluetooth scanning: Off

#### Advanced
- Google Location Accuracy > Improve Location Accuracy: Off



## Security

#### Screen lock
- Password, PIN or Pattern. Don't set to None or Swipe.

After setting screen lock, tap on gear icon next to Screen lock.

- Make pattern visible: Off (only available if Screen lock is set to Pattern)
- Lock after screen timeout: Immediately
- Power button instantly locks: On

#### SIM card lock
- Lock SIM card: On > Enter default PIN > OK
- Change SIM PIN > Enter old and new SIM PIN > OK (Create a secure new SIM PIN)

NOTE 1: The default PIN code is usually 1234 or 0000. However, if these two don't work, you should look on SIM card's packaging or contact your SIM provider's customer support.

NOTE 2: If you enter the PIN code wrong 3 times, you'll be asked to enter a PUK (Personal Unlock Key) code. This code can be obtained from the carrier, after they verify you are the rightful owner of the SIM. DO NOT try to guess the PUK code. If you enter it wrong 3 times, the SIM will be permanently locked and you might have to get a new SIM from your carrier.

#### Encryption & credentials
- Encrypt phone: Encrypted

#### Trust agents
- Smart Lock (Google): Off



## Accessibility

#### Text-to-speech output

Tap on gear icon next to Preferred engine

- Anonymous usage reports: Off



## System

#### Advanced
- Multiple users > Add users from lock screen: Off



---
---



NOTE: Some other settings are same as [Google Account settings](https://github.com/the-weird-aquarian/privacy-settings/blob/main/Privacy%20Settings/Google-Account-Privacy-Settings.md)
