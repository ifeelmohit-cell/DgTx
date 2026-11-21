# DGTX PRO Android project

This project wraps the current DGTX PRO offline-first HTML sales tracker in a simple Android WebView app. LocalStorage remains on the device/browser app installation; uninstalling the app or clearing app data can remove locally stored records. Export backups from within the app regularly.

## Build an APK using GitHub Actions (no Android Studio required)
1. Sign in to GitHub and create a new empty repository named `DGTX-PRO`.
2. Upload the contents of this folder to the repository (the `.github` folder must be included).
3. Open the repository's **Actions** tab and select **Build DGTX PRO APK**.
4. Tap **Run workflow** (or wait for the first push build to finish).
5. Open the completed workflow run and download the artifact named **DGTX-PRO-Android-APK**.
6. Extract the ZIP on your Android phone and install `app-debug.apk`. Android may ask you to allow installation from that source.

This is a debug APK for personal testing, not a Play Store release. It is not signed with a private release key. Do not share client-sensitive data from an unsecured device. The app currently stores data locally and does not sync to cloud.

## Included free offline assistant
The AI Assistant tab is a local, rule-based helper (not a connected generative AI model). It includes sales-performance coaching based on records saved in the app, a basic VAT estimate, a basic Corporate Tax estimate, and short UAE tax knowledge notes. It works without an API key or subscription and does not upload sales/customer data. Tax outputs are estimates only; check current FTA/MoF rules and client-specific circumstances before giving advice or filing returns.


## Latest update
- Uses the supplied official DgTx logo as the Android launcher icon and in-app brand mark.
- Adds UAE tax estimators for VAT, Corporate Tax, Excise Tax, Customs/import VAT, and informational UAE personal income tax and withholding-tax panels.
- Adds a DGTX service quotation calculator and catalogue based on the DgTx overview document.
- Fees for non-VAT services are editable and start at AED 0 because no official fee schedule was supplied.
- Tax estimates are indicative only and require review by a qualified DGTX tax professional before filing.
