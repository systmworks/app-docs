<p align="center"><a href="https://buymeacoffee.com/systmworks"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="45" alt="Buy me a coffee"></a></p>

> I have spent many, many hours creating and testing this. If it helps you please consider buying me a Coffee :)

# AVD Enhancer: download

## Install from Browser Store

Install from your browser's store: a store install updates itself automatically when a new version is approved.
The version live in each store today:

| Microsoft Edge | Google Chrome | Mozilla Firefox |
|:---:|:---:|:---:|
| ![Microsoft Edge Add-ons: not yet available](https://img.shields.io/badge/MICROSOFT%20EDGE-PENDING%20REVIEW-DFB317?style=for-the-badge&labelColor=555555) | [![Install from the Chrome Web Store](https://img.shields.io/badge/GOOGLE%20CHROME-INSTALL%20AVD%20ENHANCER-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=555555)](https://chromewebstore.google.com/detail/avd-enhancer/pjfnicplgngkmhkhkenohahoapoimopg) | ![Firefox Add-ons: not yet available](https://img.shields.io/badge/MOZILLA%20FIREFOX-PENDING%20REVIEW-DFB317?style=for-the-badge&labelColor=555555) |
| ![Edge published version none](https://img.shields.io/badge/Published%20Version-none%20yet-lightgrey?style=flat-square) | ![Chrome published version 1.2.0](https://img.shields.io/badge/Published%20Version-1.2.0-2EA44F?style=flat-square) | ![Firefox published version none](https://img.shields.io/badge/Published%20Version-none%20yet-lightgrey?style=flat-square) |
| ![Edge pending review 1.2.0](https://img.shields.io/badge/Pending%20review-1.2.0-DFB317?style=flat-square) | ![Chrome pending review 1.11.0](https://img.shields.io/badge/Pending%20review-1.11.0-DFB317?style=flat-square) | ![Firefox pending review 1.2.0](https://img.shields.io/badge/Pending%20review-1.2.0-DFB317?style=flat-square) |

The Edge and Firefox listings are waiting for the stores' review. Their links are added here when they are approved.
Until then Edge can install from the Chrome Web Store too (Edge asks you to allow extensions from other stores).

## Published package (Chrome 1.2.0)

The exact files of the version that is live in the Chrome Web Store, so you can read them or compare them with
what is installed. Only the currently published version is kept here; it is replaced when a newer one is approved.

| Version | File | SHA-256 |
|---|---|---|
| 1.2.0 | [AVD-Enhancer-ChromeEdge-1.2.0.zip](AVD-Enhancer-ChromeEdge-1.2.0.zip) | `34010071bb57994962e0954b470f980df9eec4ecded273457ad7cff6a61da198` |

The code is plain, unminified JavaScript. To check the download: compare its SHA-256 with the one above
(PowerShell: `Get-FileHash AVD-Enhancer-ChromeEdge-1.2.0.zip`).

To compare it with what you have installed: unzip it, then diff it against the extension folder under
`chrome://extensions` (Developer mode, then the extension's ID, then the folder under
`%LocalAppData%\Google\Chrome\User Data\Default\Extensions\`). The store repackages the file, so the ZIP's own
hash can differ from the store's, but the files inside should match.

The extension makes one kind of network request, and only to Azure Resource Manager: https://management.azure.com.
See the [privacy policy](../privacy-policy.md).

## Firefox package

The Firefox build is on Mozilla's review queue, so there is no package here yet. It is added when Firefox Add-ons
approves it.

## Manual Install

A manual install does not update itself. To move to a newer version, download the new ZIP and load it the same way,
or remove it and install from the store instead, which keeps it up to date.

**Keeping your settings.** A store install keeps your settings (switches, column widths and stars) through every
update. Your browser deletes them when the extension is removed, so to update a manual install without losing them:

### Chrome/Edge

* Download the latest `.zip` file ([AVD-Enhancer-ChromeEdge-1.2.0.zip](AVD-Enhancer-ChromeEdge-1.2.0.zip), in the published package section above)
* Extract the contents of the `.zip` file.
* Open your browser and navigate to:
   * Microsoft Edge: `edge://extensions`
   * Google Chrome: `chrome://extensions`
* Enable "Developer mode" by toggling the switch
* Click on "Load unpacked" and select the extracted folder

To update it and keep your settings, extract the new `.zip` over the same folder (replace the files), then click the
extension's reload button on the extensions page. Removing the extension, or loading the new version from a different
folder, starts again with default settings.

Newer versions are listed in [What's new](../whats-new.md) before the stores approve them, so the store can be a
version or two behind.

## Pre-release / Experimental

Newer versions that are still in store review are posted here for Chrome and Edge, with `-experimental` in the file name so
they are not mistaken for the published package. They are installed by hand (see Manual Install above), and a manual install
does not update itself. Once a store approves the version, install from the store instead.

| Version | File | SHA-256 |
|---|---|---|
| 1.11.0 (pending review in Chrome) | [AVD-Enhancer-ChromeEdge-1.11.0-experimental.zip](AVD-Enhancer-ChromeEdge-1.11.0-experimental.zip) | `856e322a7bea3198239d15595db0a096e6866a7880646ce85894e24a0c9d2807` |

What is new since 1.2.0: six themes (Light Blue, Grey and Pink; Dark Blue, Green and Red), notices when Scan sessions or Check my access leave something out, keyboard and screen reader support in the sidebar, and a few fixes. See [What's new](../whats-new.md).

Contact: systmworks@outlook.com

---

**Sharing & responsibility** - Built for the community, shared with good intentions. Use at your own risk. The author accepts no responsibility for any outcomes resulting from the use of this software. Test in a safe environment first. If you find an issue or have a suggestion, contributions are welcome.
