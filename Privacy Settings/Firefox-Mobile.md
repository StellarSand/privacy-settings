# Firefox Mobile Privacy Settings

**Following settings also apply to Fennec, except the Data collection section.**

Go to Settings.



## Search

#### Search engines
- Default search engine: DuckDuckGo or add any other privacy respecting search engine.

#### Suggestions from search engine
- Show search suggestions: Off

#### Address bar preferences
- Show clipboard suggestions: Off
- Autocomplete URLs: Off



## Homepage
- Sponsored shortcuts: Off
- Thought-provoking stories: Off (Does not apply to Fennec)



## Passwords
- Save passwords: Never save
- Autofill in Firefox/Fennec: Off
- Autofill in other apps: Off

> :information_source: **NOTE**: Never save passwords in browsers. Use a password manager instead. Check out [recommendations, alternatives & reviews](https://github.com/StellarSand/privacy-settings#recommendations-alternatives--reviews).


## Autofill
- Save and autofill addresses: Off
- Save and autofill cards: Off

> :information_source: **NOTE**: Never save payment info or credit card details in browsers. A password manager can be used to also save payment information or card details.



## Private browsing
- Allow screenshots in private browsing: Off



## HTTPS-Only Mode
- On
- Enable in all tabs



## Enhanced Tracking Protection
- On
- Strict
- Tell websites not to share & sell data: Enable only for jurisdictions mentioned in the note below
  > :information_source: **NOTE**: [Global Privacy Control (GPC)](https://globalprivacycontrol.org/) operates as a “Do Not Sell” mechanism in some US states such as California, Colorado and Connecticut. It may also be used to indicate an opt-out of targeted advertising or general request to limit the sale or sharing of your personal data in those jurisdictions, as well as in jurisdictions such as the EU, UK, Nevada, Utah and Virginia.
  > <br>If you don't reside in these jurisdictions, disable this, as it **may** be used for potential browser fingerprinting purposes.



## Site permissions
- Cross-site cookies: Blocked



## Data collection
**This section does not apply to Fennec**
- Usage and technical data: Off
- Studies: Off



## Extensions
Check [recommended extensions](https://github.com/StellarSand/privacy-settings#recommended-extensions) to add


---
---


## Further Hardening

- For further hardening of Firefox Beta and Fennec, check out [arkenfox user.js](https://github.com/arkenfox/user.js).

> :information_source: **NOTE 1**: To use user.js, place it in
> - Firefox Beta: `/data/data/org.mozilla.firefox_beta/files/mozilla/<profile name>.default/`
> - Fennec: `/data/data/org.mozilla.fennec_fdroid/files/mozilla/<profile name>.default/`
>
> Check the permissions for pref.js already present in that path and give the same permissions to user.js
>
> :information_source: **NOTE 2**:
> - Root access is required for placing user.js in above mentioned path and changing permissions. 
> - Users without root access can change each and every setting manually in about:config
