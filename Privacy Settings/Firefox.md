# Firefox Privacy Settings

Go to Settings.



## General

#### Files and Applications
- Downloads >
  - Always ask you where to save files: On

#### Browsing
- Recommend extensions as you browse: Off
- Recommend features as you browse: Off



## Home

#### Firefox Home Content
- Shortcuts > Sponsored shortcuts: Off
- Recommended stories: Off



## Search

#### Default Search Engine
- `DuckDuckGo` or add any other privacy respecting search engine.

#### Search Suggestions
- Show search suggestions: Off



## Privacy & Security

#### Enhanced Tracking Protection
- Strict

#### Website Privacy Preferences
- Tell websites not to sell or share my data: Enable only for jurisdictions mentioned in the note below
  > :information_source: **NOTE**: [Global Privacy Control (GPC)](https://globalprivacycontrol.org/) operates as a “Do Not Sell” mechanism in some US states such as California, Colorado and Connecticut. It may also be used to indicate an opt-out of targeted advertising or general request to limit the sale or sharing of your personal data in those jurisdictions, as well as in jurisdictions such as the EU, UK, Nevada, Utah and Virginia.
  > <br>If you don't reside in these jurisdictions, disable this, as it **may** be used for potential browser fingerprinting purposes.
- Send websites a “Do Not Track” request: Off

#### Passwords
- Ask to save passwords: Off

> :information_source: **NOTE**: Never save passwords in browsers. Use a password manager instead. Check out [recommendations, alternatives & reviews](https://github.com/StellarSand/privacy-settings#recommendations-alternatives--reviews).

#### Permissions
- Warn you when websites try to install add-ons: On

#### Firefox Data Collection and Use
- Turn off everything

#### Website Advertising Preferences
- Allow websites to perform privacy-preserving ad measurement: Off

#### Security
- Deceptive Content and Dangerous Software Protection >
  - Enable everything
- Certificates >
  - Query OCSP responder servers to confirm the current validity of certificates: On

#### HTTPS-Only Mode
- Enable HTTPS-Only Mode in all windows

#### DNS over HTTPS
- Enable secure DNS using >
  - Max Protection
  - Choose provider: `NextDNS`/`Cloudflare` or select `Custom` and provide URL for other secure DNS from [this list](https://www.privacyguides.org/en/dns/#recommended-providers).
  
    Example: For Quad9, enter https://dns.quad9.net/dns-query

---
---

## Further Hardening
- For further hardening of Firefox, check out [arkenfox user.js](https://github.com/arkenfox/user.js).