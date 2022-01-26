# Firefox Mobile Privacy Settings

**Following settings also apply to Fennec (F-droid version of firefox), except the Data Collection section.**

Go to Settings.



## Search
- Default search engine: DuckDuckGo or add any other privacy respecting search engine.
- Autocomplete URLs: Off
- Show clipboard suggestions: Off
- Show voice search: Off
- Show search suggestions: Off



## Logins and Passwords
- Save logins and passwords: Never save
- Autofill in Firefox/Fennec: Off
- Autofill in other apps: Off

NOTE: Never save passwords in browsers. Use a password manager instead. Check out [recommendations, alternatives & reviews](https://github.com/the-weird-aquarian/privacy-settings#recommendations-alternatives--reviews).



## Credit cards
- Save and autofill cards: Off

NOTE: Never save payment info or credit card details in browsers. A password manager can be used to also save payment information or card details.



## Private browsing
- Allow screenshots in private browsing: Off



## Enhanced Tracking Protection
- Enhanced Tracking Protection: On
- Strict



## Data collection
**This section does not apply to Fennec**
- Usage and technical data: Off
- Marketing data: Off
- Studies: Off



## Add-ons
Check [recommended extensions](https://github.com/the-weird-aquarian/privacy-settings#recommended-extensions) to add



---
---



## Further Hardening

Firefox Beta and Fennec users can further harden firefox by changing about:config settings

- For further hardening of Firefox, check out [arkenfox user.js](https://github.com/arkenfox/user.js).

NOTE 1: To use user.js, place it in
- Firefox Beta: /data/data/org.mozilla.firefox_beta/files/mozilla/SomeAlphanumericText.default/
- Fennec: /data/data/org.mozilla.fennec_fdroid/files/mozilla/SomeAlphanumericText.default/

Check the permissions for pref.js already present in that path and give the same permissions to user.js

NOTE 2:
- Root access is required for placing user.js in above mentioned path and changing permissions. 
- Users without root access can just change each and every setting manually in about:config

