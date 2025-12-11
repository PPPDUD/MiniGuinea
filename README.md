# MiniGuinea
<img width="128" height="128" alt="17558778127483925235314353808994" src="https://github.com/user-attachments/assets/6cb72e00-cf3a-4d79-a7b6-14bc73c39ded" />

MiniGuinea is a simple Chromium extension that:
- Stops dozens of ad providers from serving their ads to your browser; including but not limited to Google Doubleclick, Amazon Advertising, and CoinZilla
- Defeats several different analytics providers, most notably Google Analytics, Cloudflare Insights, and the United States Digital Analytics Program
- Uses Manifest v3 (if you don't know what this means, don't worry about it)
- Avoids interfering with the user experience as much as possible
- Makes some websites load faster by blocking unwanted web requests
- Blocks some tracker parameters in URLs (since 0.8, currently experimental)

MiniGuinea is known to work in Chromium, Google Chrome, and Microsoft Edge. It should function properly in most other Chromium browsers too.

MiniGuinea does not officially support Firefox-based browsers (Firefox, Tor Browser, etc.) at the moment. Firefox support is not planned for the foreseeable future.
 
# Comparison to other ad blockers
## Tracker blocking ability
| Tracker     | Blocked by MiniGuinea? | Blocked by AdBlock? | Blocked by Ghostery? |
| ----------- | ----------- | ----------- | ----------- |
| Google Analytics      | Yes       | No        | Yes*        |
| Qualtrics   | Yes         | No        | Yes       |
| Digital Analytics Program   | Yes**        | No       | Yes        |
| Cloudflare Insights   | Yes        | No       | Yes        |
| Jetpack Analytics   | Yes       | No       | Yes        |
| Wikitide Analytics (based on Matomo)   | Yes    | No       | Yes        |****

## Ad blocking ability
| Ad provider     | Blocked by MiniGuinea? | Blocked by AdBlock? | Blocked by Ghostery? |
| ----------- | ----------- | ----------- | ----------- |
| DoubleClick      | Yes       | Yes (acceptable ads must be disabled before it will work)        | Yes*        |
| DoubleVerify   | Yes         | Yes        | Yes       |
| Amazon Adsystem   | Yes       | Yes       | Yes*        |********
| Outbrain   | Yes       | Hidden but not blocked       | Partially        |

## Special considerations
| Blocking software     | Permissions | Storage space | Software license | Primary source of revenue | Uses telemetry? |
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| MiniGuinea      | Block content on any page       | ~0.03MB      | MIT        | None (hobby project) | No |
| AdBlock   | Read and change all your data on all websites, display notifications         | 299MB        | GPLv3 | Acceptable Ads program | Yes |  
| Ghostery  | Read your browsing history, block content on any page       | 49.8MB       | GPLv3        | Donations | Yes |********

*Ghostery appears to be injecting its own script here. More information is needed.

**This tracker appears to be capable of evading MiniGuinea in some situations. Research is underway.

# Known issues
On MiniGuinea v0.1, there is a missing icon file which makes installation impossible. Starting with MiniGuinea v0.2, all of the icon files are in place.

In MiniGuinea versions predating v0.6, you cannot view your Google Analytics dashboard properly. A fix was made during early development, but somehow got dropped from the codebase before v0.1 was released. An improved fix is available in v0.6 and later.

A bug has been discovered in MiniGuinea versions v0.4 through v0.6, preventing parts of the New York Post website from loading properly. A fix has been developed and will become available in v0.7.
