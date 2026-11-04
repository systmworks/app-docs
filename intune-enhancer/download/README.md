# Intune Enhancer: download

Install from your browser's store: a store install updates itself automatically when a new version is approved.
The version live in each store today:

| Microsoft Edge | Google Chrome | Mozilla Firefox |
|:---:|:---:|:---:|
| [![Install from Microsoft Edge Add-ons](https://img.shields.io/badge/MICROSOFT%20EDGE-INSTALL%20INTUNE%20ENHANCER-0078D7?style=for-the-badge&labelColor=555555)](https://microsoftedge.microsoft.com/addons/detail/intune-enhancer/hcmhldmcpgieiaeobdbppcgfckahdeci) | [![Install from the Chrome Web Store](https://img.shields.io/badge/GOOGLE%20CHROME-INSTALL%20INTUNE%20ENHANCER-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=555555)](https://chromewebstore.google.com/detail/intune-enhancer/geifmacoimaenjdednhfiegamkjkgjjm) | ![Firefox Add-ons: coming soon](https://img.shields.io/badge/MOZILLA%20FIREFOX-COMING%20SOON-FF7139?style=for-the-badge&logo=firefoxbrowser&logoColor=white&labelColor=555555) |
| ![Edge published version 1.27.0](https://img.shields.io/badge/Published%20Version-1.27.0-0078D7?style=flat-square) | ![Chrome published version 1.87.0](https://img.shields.io/badge/Published%20Version-1.87.0-4285F4?style=flat-square) | ![Firefox published version none](https://img.shields.io/badge/Published%20Version-none-lightgrey?style=flat-square) |
| ![Edge pending review 1.86.0](https://img.shields.io/badge/Pending%20review-1.86.0-DFB317?style=flat-square) | ![Chrome pending review none](https://img.shields.io/badge/Pending%20review-none-lightgrey?style=flat-square) | ![Firefox pending review 1.84.0](https://img.shields.io/badge/Pending%20review-1.84.0-DFB317?style=flat-square) |

**Manual Install**

A manual install does not update itself. To move to a newer version, download the new ZIP and load it the same way,
or remove it and install from the store instead, which keeps it up to date.

Chrome/Edge

* Download the latest `.zip` file ([Intune-Enhancer-1.87.0.zip](Intune-Enhancer-1.87.0.zip), in the published package section below)
* Extract the contents of the `.zip` file.
* Open your browser and navigate to:
   * Microsoft Edge: `edge://extensions`
   * Google Chrome: `chrome://extensions`
* Enable "Developer mode" by toggling the switch
* Click on "Load unpacked" and select the extracted folder

Firefox

* Install it from Firefox Add-ons once the review is done (Firefox only installs signed add-ons, so there is no
  manual install from a ZIP).

Newer versions are listed in [What's new](../whats-new.md) before the stores approve them, so the store can be a
version or two behind.

## Published package (Chrome 1.87.0)

The exact files of the version that is live in the Chrome Web Store, so you can read them or compare them with
what is installed. Only the currently published version is kept here; it is replaced when a newer one is approved.

| Version | File | SHA-256 |
|---|---|---|
| 1.87.0 | [Intune-Enhancer-1.87.0.zip](Intune-Enhancer-1.87.0.zip) | `4783d8195cddaed3fce27b2b58e6a6a884eae0ba3bb2fd05571c0eb1b7df5cee` |

The code is plain, unminified JavaScript. To check the download: compare its SHA-256 with the one above
(PowerShell: `Get-FileHash Intune-Enhancer-1.87.0.zip`).

To compare it with what you have installed: unzip it, then diff it against the extension folder under
`chrome://extensions` (Developer mode, then the extension's ID, then the folder under
`%LocalAppData%\Google\Chrome\User Data\Default\Extensions\`). The store repackages the file, so the ZIP's own
hash can differ from the store's, but the files inside should match.

The extension makes one kind of network request, in `src/core/graph.js`, and only to Microsoft Graph:

* https://graph.microsoft.com (all versions)
* https://graph.microsoft.us (v1.92+)
* https://dod-graph.microsoft.us (v1.92+)

The two US Government addresses are used only if you allow a US Government cloud in Settings, and then only the one for the cloud you are signed in to. See the [privacy policy](../privacy-policy.md).

Contact: systmworks@outlook.com
