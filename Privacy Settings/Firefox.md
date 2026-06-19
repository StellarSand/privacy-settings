# <img src="../icons/firefox.svg" width="42" align="top"> Firefox Desktop Privacy Settings

Go to Settings.



## Home and startup

#### Firefox Home
- Stories: Off
- Support Firefox : Off



## Search

#### Default search engine
- `DuckDuckGo` or add any other privacy respecting search engine.

#### Search engine suggestions
- Show search suggestions: Off

#### Address Bar
- Suggest search engines to use: Off



## Privacy and security

#### Enhanced Tracking Protection
- Advanced settings >
  - Strict

#### Additional protections
- Tell websites not to sell or share my data: Enable only for jurisdictions mentioned in the note below
  > <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
  >
  > [Global Privacy Control (GPC)](https://globalprivacycontrol.org/) operates as a “Do Not Sell” mechanism in some US states such as California, Colorado and Connecticut. It may also be used to indicate an opt-out of targeted advertising or general request to limit the sale or sharing of your personal data in those jurisdictions, as well as in jurisdictions such as the EU, UK, Nevada, Utah and Virginia.
  > <br>If you don't reside in these jurisdictions, disable this, as it **may** be used for potential browser fingerprinting purposes.

#### DNS over HTTPS
- Advanced settings >
  - Custom
    - Always warn me if secure DNS isn’t available: On
    - Choose provider: `NextDNS`/`Cloudflare` or select `Custom` and provide URL for other secure DNS from [this list](https://www.privacyguides.org/en/dns/#recommended-providers).
  
      Example: For Quad9, enter https://dns.quad9.net/dns-query

#### Connection and software security
- Advanced settings >
  - HTTPS-Only Mode: Enable HTTPS-Only Mode in all windows
  - Deceptive content and dangerous software protection: Enable everything



## Passwords and autofill

#### Passwords
- Ask to save passwords: Off

> <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
>
> Never save passwords in browsers. Use a password manager instead. Check out [recommendations, alternatives & reviews](https://github.com/StellarSand/privacy-settings#recommendations-alternatives--reviews).

#### Payment methods
- Save and autofill payment info: Off

> <img src="../icons/ic_note.svg" width="22" align="top"> **Note**
>
> Never save payment info in browsers. A password manager can be used to also save payment information.

#### Addresses and more
- Save and autofill addresses: Off



## Downloads

#### Save files to
- Always ask you where to save files: On



## Tabs and browsing

#### Recommendations
- Recommend extensions as you browse: Off
- Recommend features as you browse: Off



## AI Controls
- Block AI enhancements: On



## Permissions and data

#### Permissions
- Block pop-ups and third-party redirects: On
- Show warning when websites try to install extensions: On

#### Firefox data collection and use
- Disable everything


---


## Further Hardening
- For further hardening of Firefox, check out [arkenfox user.js](https://github.com/arkenfox/user.js).