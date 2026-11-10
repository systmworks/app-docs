# Intune Enhancer: download

## Install from Browser Store

Install from your browser's store: a store install updates itself automatically when a new version is approved.
The version live in each store today:

| Microsoft Edge | Google Chrome | Mozilla Firefox |
|:---:|:---:|:---:|
| [![Install from Microsoft Edge Add-ons](https://img.shields.io/badge/MICROSOFT%20EDGE-INSTALL%20INTUNE%20ENHANCER-0078D7?style=for-the-badge&labelColor=555555)](https://microsoftedge.microsoft.com/addons/detail/intune-enhancer/hcmhldmcpgieiaeobdbppcgfckahdeci) | [![Install from the Chrome Web Store](https://img.shields.io/badge/GOOGLE%20CHROME-INSTALL%20INTUNE%20ENHANCER-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=555555)](https://chromewebstore.google.com/detail/intune-enhancer/geifmacoimaenjdednhfiegamkjkgjjm) | [![Install from Firefox Add-ons](https://img.shields.io/badge/MOZILLA%20FIREFOX-INSTALL%20INTUNE%20ENHANCER-FF7139?style=for-the-badge&logo=firefoxbrowser&logoColor=white&labelColor=555555)](https://addons.mozilla.org/firefox/addon/intune-enhancer/) |
| ![Edge published version 1.86.0](https://img.shields.io/badge/Published%20Version-1.86.0-2EA44F?style=flat-square) | ![Chrome published version 2.89.0](https://img.shields.io/badge/Published%20Version-2.89.0-2EA44F?style=flat-square) | ![Firefox published version 2.89.0](https://img.shields.io/badge/Published%20Version-2.89.0-2EA44F?style=flat-square) |
| ![Edge pending review 2.89.0](https://img.shields.io/badge/Pending%20review-2.89.0-DFB317?style=flat-square) | ![Chrome pending review none](https://img.shields.io/badge/Pending%20review-none-lightgrey?style=flat-square) | ![Firefox pending review none](https://img.shields.io/badge/Pending%20review-none-lightgrey?style=flat-square) |

## Published package (Chrome 2.89.0)

The exact files of the version that is live in the Chrome Web Store, so you can read them or compare them with
what is installed. Only the currently published version is kept here; it is replaced when a newer one is approved.

| Version | File | SHA-256 |
|---|---|---|
| 2.89.0 | [Intune-Enhancer-ChromeEdge-2.89.0.zip](Intune-Enhancer-ChromeEdge-2.89.0.zip) | `e10d088fff71e581c0f5723db0c3ae5ab1a82a47ca90f2c3e5ebf42ac3aff86c` |

The code is plain, unminified JavaScript. To check the download: compare its SHA-256 with the one above
(PowerShell: `Get-FileHash Intune-Enhancer-ChromeEdge-2.89.0.zip`).

To compare it with what you have installed: unzip it, then diff it against the extension folder under
`chrome://extensions` (Developer mode, then the extension's ID, then the folder under
`%LocalAppData%\Google\Chrome\User Data\Default\Extensions\`). The store repackages the file, so the ZIP's own
hash can differ from the store's, but the files inside should match.

## Firefox package (2.89.0)

The Firefox build of the version that is live on Firefox Add-ons: the same files as Chrome and Edge, with a
Firefox manifest.

| Version | File | SHA-256 |
|---|---|---|
| 2.89.0 | [Intune-Enhancer-Firefox-2.89.0.zip](Intune-Enhancer-Firefox-2.89.0.zip) | `036a2051324ca384a23e120c6a44a6e281e5b24d85a05ea7d5b1036f8894e8b9` |

The extension makes one kind of network request, in `src/core/graph.js`, and only to Microsoft Graph:

* https://graph.microsoft.com (all versions)
* https://graph.microsoft.us (v1.92+)
* https://dod-graph.microsoft.us (v1.92+)

The two US Government addresses are used only if you allow a US Government cloud in Settings, and then only the one for the cloud you are signed in to. See the [privacy policy](../privacy-policy.md).

## Manual Install

A manual install does not update itself. To move to a newer version, download the new ZIP and load it the same way,
or remove it and install from the store instead, which keeps it up to date.

**Keeping your settings.** A store install keeps your settings (switches, column widths and stars) through every
update. Your browser deletes them when the extension is removed, so to update a manual install without losing them:

### Chrome/Edge

* Download the latest `.zip` file ([Intune-Enhancer-ChromeEdge-2.89.0.zip](Intune-Enhancer-ChromeEdge-2.89.0.zip), in the published package section above)
* Extract the contents of the `.zip` file.
* Open your browser and navigate to:
   * Microsoft Edge: `edge://extensions`
   * Google Chrome: `chrome://extensions`
* Enable "Developer mode" by toggling the switch
* Click on "Load unpacked" and select the extracted folder

To update it and keep your settings, extract the new `.zip` over the same folder (replace the files), then click the
extension's reload button on the extensions page. Removing the extension, or loading the new version from a different
folder, starts again with default settings.

### Firefox

Intune Enhancer is on [Firefox Add-ons](https://addons.mozilla.org/firefox/addon/intune-enhancer/), and installing
from there is the easiest way. To load it by hand for a test instead:

* Download the Firefox `.zip` file ([Intune-Enhancer-Firefox-2.89.0.zip](Intune-Enhancer-Firefox-2.89.0.zip), the
  published version, in the Firefox package section above)
* Extract the contents of the `.zip` file.
* Open Firefox and navigate to `about:debugging#/runtime/this-firefox`
* Click "Load Temporary Add-on" and select the `manifest.json` file in the extracted folder

Firefox removes a temporary add-on when it closes, so you load it again after each restart (and it never updates
itself). Your settings are kept when you load it again.

Newer versions are listed in [What's new](../whats-new.md) before the stores approve them, so the store can be a
version or two behind.

## Pre-release / Experimental (2.89.0)

**This version is still undergoing testing.** It has the newest features and fixes listed in
[What's new](../whats-new.md), but the Chrome and Edge stores have not approved it yet, so use the store version if you want the
tested one. (Firefox already has this version: see the Firefox package above.) Install it by hand with the steps above
(Load unpacked). A manual install does not update itself.

| Browser | File | SHA-256 |
|---|---|---|
| Chrome / Edge | [Intune-Enhancer-ChromeEdge-2.89.0-experimental.zip](Intune-Enhancer-ChromeEdge-2.89.0-experimental.zip) | `8f073021db5399615b9a8e3890c85eb6ad33bf0a3b198bd6874e4d5a857ade20` |

If you already have a store version installed, remove it before loading this one (two copies would both run). Removing
it deletes its settings, so you set them again here.

Contact: systmworks@outlook.com
