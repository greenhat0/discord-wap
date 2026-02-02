# Discord WAP (Fork)
Discord proxy client for old mobile browsers with Wireless Application Protocol 1.x or HTML support.

## Status
### Working
* Server, channel, and DM lists
  * Note: due to page size limitations, only the most recently used channels are shown (WML version)
* Message sending
* Replying with ping on or off
* Message history with pagination
* Settings (e.g. message load count)
* Message timestamps
* Attachments and profile pictures (HTML "modern" layout only)
* Emojis
  * Note: Only default Emojis are supported as of now. (HTML only)
### Not implemented
* Message editing and deleting
* Threads
* Message indicators (WIP)
* Reactions
## How to use
Hosted public instances are only for the [Original](https://github.com/gtrxAC/discord-wap) repository. You will have to [self-host](#Self-hosting).
> - A public instance is hosted at http://gtrxac.fi/wap or http://146.59.80.3/wap, but it is recommended to host your own instance if possible.

Using a secondary/alt account is recommended for safety, especially when using public instances hosted by unknown people. However, when using third-party clients, Discord has been known to sometimes restrict or temporarily disable newly created accounts. This may also affect accounts that don't have two-factor authentication or a verified phone number. If your alt account is likely to get restricted, it may be worth using your main account instead.

Additionally, the servers list may fail to load on older devices if the account is a member of too many servers.

You will need:
* A Discord account
* A way to get that account's token, e.g. a web browser with support for developer tools (most PC browsers, or Kiwi Browser on Android)
* A phone that supports xHTML/HTML or WAP 1.x/WML 1.1 or higher
> - A data transfer technology that is available in your region (usually GPRS) | Not related unless you port forward

## Self-hosting
1. Install [Node.js](https://nodejs.org).
2. Clone this repository.
3. Copy `.env.example` to `.env`.
4. Edit the variables inside the `.env` file as you see fit.
4. Open a terminal in the folder of the cloned repository.
5. Run `npm i` and `node .`

Steps:
* Get your account's token using, for example, [this guide](https://github.com/NotNexuss/Get-Discord-Token).
> - Configure your phone's internet access point settings. In particular, set the APN (access point name) to your carrier's APN, and set the WAP gateway's IP address to one of the IPs listed [here](https://nbpfan.bs0dd.net/index.php?lang=eng&page=wap%2Fmain). Guides for certain phone brands are provided [here](https://lpcwiki.miraheze.org/wiki/GPRS_configuration). | Not related unless you port forward
* Find your IPv4 Address and paste the Instance's address into your Phone's browser, for example http://127.0.0.1:1337/wap | (http://IP:PORT/wap) |
* When the page loads, enter your account's token and select `Log in`.
* For quick access in the future, you should add the main menu (Servers/DMs/Settings selection) to your bookmarks. This bookmark will contain your account's token.


## Additional credits
[iamcal](https://github.com/iamcal) for [emoji-data](https://github.com/iamcal/emoji-data)

[gtrxAC](https://github.com/gtrxAC) for [Discord WAP](https://github.com/gtrxAC/discord-wap)
