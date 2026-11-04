# Intune Enhancer: download

Install from your browser's store. The version live in each store today:

| Browser | Store | Version live |
|---|---|---|
| Google Chrome | [Chrome Web Store](https://chromewebstore.google.com/detail/intune-enhancer/geifmacoimaenjdednhfiegamkjkgjjm) | 1.76.0 |
| Microsoft Edge | [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/intune-enhancer/hcmhldmcpgieiaeobdbppcgfckahdeci) | 1.27.0 |

Newer versions are listed in [What's new](../whats-new.md) before the stores approve them, so the store can be a
version or two behind.

## Published package (Chrome 1.76.0)

The exact files of the version that is live in the Chrome Web Store, so you can read them or compare them with
what is installed. Only the currently published version is kept here; it is replaced when a newer one is approved.

| Version | File | SHA-256 |
|---|---|---|
| 1.76.0 | [Intune-Enhancer-1.76.0.zip](Intune-Enhancer-1.76.0.zip) | `9ec48b42f8289de69ee85fb8fc89c178a29df92cf23ba9830ed6c3f681330605` |

The code is plain, unminified JavaScript. To check the download: compare its SHA-256 with the one above
(PowerShell: `Get-FileHash Intune-Enhancer-1.76.0.zip`).

To compare it with what you have installed: unzip it, then diff it against the extension folder under
`chrome://extensions` (Developer mode, then the extension's ID, then the folder under
`%LocalAppData%\Google\Chrome\User Data\Default\Extensions\`). The store repackages the file, so the ZIP's own
hash can differ from the store's, but the files inside should match.

The extension makes one kind of network request, in `src/core/graph.js`, and in the 1.76.0 package above only to https://graph.microsoft.com. From 1.92.0 it can also use https://graph.microsoft.us or https://dod-graph.microsoft.us, but only if you allow a US Government cloud in its Settings, and then only the one for the cloud you are signed in to.
See the [privacy policy](../privacy-policy.md).

Contact: systmworks@outlook.com
