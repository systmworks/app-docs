# Intune Enhancer: published package

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

The extension makes one kind of network request, in `src/core/graph.js`, and only to https://graph.microsoft.com.
See the [privacy policy](../privacy-policy.md).

Contact: systmworks@outlook.com
