<p align="center"><a href="https://buymeacoffee.com/systmworks"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="45" alt="Buy me a coffee"></a></p>

> I have spent many, many hours creating and testing this. If it helps you please consider buying me a Coffee :)

# Intune Enhancer: download

## Install from Browser Store

Install from your browser's store: a store install updates itself automatically when a new version is approved.
The version live in each store today:

| Microsoft Edge | Google Chrome | Mozilla Firefox |
|:---:|:---:|:---:|
| [![Install from Microsoft Edge Add-ons](https://img.shields.io/badge/MICROSOFT%20EDGE-INSTALL%20INTUNE%20ENHANCER-0078D7?style=for-the-badge&labelColor=555555)](https://microsoftedge.microsoft.com/addons/detail/intune-enhancer/hcmhldmcpgieiaeobdbppcgfckahdeci) | [![Install from the Chrome Web Store](https://img.shields.io/badge/GOOGLE%20CHROME-INSTALL%20INTUNE%20ENHANCER-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=555555)](https://chromewebstore.google.com/detail/intune-enhancer/geifmacoimaenjdednhfiegamkjkgjjm) | [![Install from Firefox Add-ons](https://img.shields.io/badge/MOZILLA%20FIREFOX-INSTALL%20INTUNE%20ENHANCER-FF7139?style=for-the-badge&logo=firefoxbrowser&logoColor=white&labelColor=555555)](https://addons.mozilla.org/firefox/addon/intune-enhancer/) |
| ![Edge published version 2.89.0](https://img.shields.io/badge/Published%20Version-2.89.0-2EA44F?style=flat-square) | ![Chrome published version 2.117.0](https://img.shields.io/badge/Published%20Version-2.117.0-2EA44F?style=flat-square) | ![Firefox published version 2.117.0](https://img.shields.io/badge/Published%20Version-2.117.0-2EA44F?style=flat-square) |
| ![Edge pending review none](https://img.shields.io/badge/Pending%20review-none-lightgrey?style=flat-square) | ![Chrome pending review none](https://img.shields.io/badge/Pending%20review-none-lightgrey?style=flat-square) | ![Firefox pending review none](https://img.shields.io/badge/Pending%20review-none-lightgrey?style=flat-square) |

## Published package (Chrome 2.117.0)

The exact files of the version that is live in the Chrome Web Store, so you can read them or compare them with
what is installed. Only the currently published version is kept here; it is replaced when a newer one is approved.

| Version | File | SHA-256 |
|---|---|---|
| 2.117.0 | [Intune-Enhancer-ChromeEdge-2.117.0.zip](Intune-Enhancer-ChromeEdge-2.117.0.zip) | `2625b9d478e6579350c24c42f57fa2d4ae6735ffe33e0a253013280667889bf4` |

The code is plain, unminified JavaScript. To check the download: compare its SHA-256 with the one above
(PowerShell: `Get-FileHash Intune-Enhancer-ChromeEdge-2.117.0.zip`).

To compare it with what you have installed: unzip it, then diff it against the extension folder under
`chrome://extensions` (Developer mode, then the extension's ID, then the folder under
`%LocalAppData%\Google\Chrome\User Data\Default\Extensions\`). The store repackages the file, so the ZIP's own
hash can differ from the store's, but the files inside should match.

## Firefox package (2.117.0)

The Firefox build of the version that is live on Firefox Add-ons: the same files as Chrome and Edge, with a
Firefox manifest.

| Version | File | SHA-256 |
|---|---|---|
| 2.117.0 | [Intune-Enhancer-Firefox-2.117.0.zip](Intune-Enhancer-Firefox-2.117.0.zip) | `44a04932f6cdb8758a48bc0429ca21ab1964e4bf8dd6273584271c0aa09d1401` |

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

* Download the latest `.zip` file ([Intune-Enhancer-ChromeEdge-2.117.0.zip](Intune-Enhancer-ChromeEdge-2.117.0.zip), in the published package section above)
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

* Download the Firefox `.zip` file ([Intune-Enhancer-Firefox-2.117.0.zip](Intune-Enhancer-Firefox-2.117.0.zip), the
  published version, in the Firefox package section above)
* Extract the contents of the `.zip` file.
* Open Firefox and navigate to `about:debugging#/runtime/this-firefox`
* Click "Load Temporary Add-on" and select the `manifest.json` file in the extracted folder

Firefox removes a temporary add-on when it closes, so you load it again after each restart (and it never updates
itself). Your settings are kept when you load it again.

Newer versions are listed in [What's new](../whats-new.md) before the stores approve them, so the store can be a
version or two behind.

## Pre-release / Experimental (2.117.0)

**This version is still undergoing testing.** It has the newest features and fixes listed in
[What's new](../whats-new.md), but the Edge store has not approved it yet, so use the store version if you want the tested
one. (Chrome and Firefox already have this version: see the published packages above.) Install it by hand with the steps above
(Load unpacked). A manual install does not update itself.

The file is the Chrome and Edge ZIP in the published package section above ([Intune-Enhancer-ChromeEdge-2.117.0.zip](Intune-Enhancer-ChromeEdge-2.117.0.zip)).

If you already have a store version installed, remove it before loading this one (two copies would both run). Removing
it deletes its settings, so you set them again here.

Contact: systmworks@outlook.com

---

**Sharing & responsibility** - Built for the community, shared with good intentions. Use at your own risk. The author accepts no responsibility for any outcomes resulting from the use of this software. Test in a safe environment first. If you find an issue or have a suggestion, contributions are welcome.
