# Firefox Mobile Privacy Settings

**Following settings also apply to Fennec (F-droid version of firefox), except the Data Collection section.**

Go to Settings.



## General

#### Search
- Default search engine: DuckDuckGo or add any other privacy respecting search engine like Qwant, Swisscows etc.
- Autocomplete URLs: Off
- Show clipboard suggestion: Off
- Show voice search: Off
- Show search suggestions: Off

#### Logins and Passwords
- Save logins and passwords: Never save
- Autofill: Off

NOTE: Never save passwords in browsers. Use a password manager instead. Check out [Additional Resources](https://github.com/the-weird-aquarian/privacy-settings#additional-resources) for more info.

#### Credit cards
- Save and autofill cards: Off

NOTE: Never save payment info or credit card details in browsers. A password manager can be used to also save payment information or card details.



## Privacy and security

#### Private browsing
- Open links in a private tab: On
- Allow screenshots in private browsing: Off

#### Enhanced Tracking Protection
- Toggle on
- Strict

#### Data collection
**This section does not apply to Fennec**
- Usage and technical data: Off
- Marketing data: Off
- Studies: Off



---
---



## Further Hardening

Firefox Beta and Fennec users can further harden firefox by changing about:config settings

- For further hardening of Firefox, check out [Privacy Guides](https://www.privacyguides.org/browsers/#about_config) and [arkenfox user.js](https://github.com/arkenfox/user.js)

NOTE: To use user.js, place it in
- Firefox Beta: /data/data/org.mozilla.firefox_beta/files/mozilla/SomeAlphanumericText.default/
- Fennec: /data/data/org.mozilla.fennec_fdroid/files/mozilla/SomeAlphanumericText.default/

Check the permissions for pref.js and give the same to user.js

**Requires root access for the above steps**

Alternatively just change each and every setting manually in about:config

