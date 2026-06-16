# Privacy Policy

- **App:** aLike Expense Manager
- **Developer:** Eight Elephants Group
- **Package:** com.eightelephantsgroup.expmanager
- **Effective date:** 2 June 2026
- **Contact:** eightelephantsgroup@gmail.com

## The short version

aLike is an **offline expense manager**. Your financial data lives on your phone. We don't run servers, we don't collect analytics, and we never see your transactions. The only network features are **optional** and explicitly turned on by you (Google Drive backup; downloading a larger voice-recognition model). Nothing leaves your phone unless you ask it to.

## What data we collect

**None on our servers.** We don't operate any backend that receives your data. All of the following stays on your device:

- Transactions, accounts, categories, budgets, recurring rules, tags
- App settings (theme, currency, notifications, lock PIN)
- Your voice when using voice entry (processed locally by Whisper, then discarded)

## What permissions we use, and why

- **Microphone (RECORD_AUDIO)** — used only while you hold the microphone button on the entry screen. Audio is processed entirely on-device by a bundled Whisper model. Audio bytes are **never recorded to a file** and **never transmitted anywhere**.
- **Internet (INTERNET)** — used only when (a) you turn on Google Drive backup, or (b) you choose to download a larger voice-recognition model. The app makes no other network calls.
- **Biometric (USE_BIOMETRIC)** — only if you turn on app lock with fingerprint/face. Authentication is handled by Android; we never see your biometric data.
- **Notifications (POST_NOTIFICATIONS)** — only if you turn on reminders for recurring transactions, budget alerts, or daily logging nudges.
- **Foreground service (FOREGROUND_SERVICE / FOREGROUND_SERVICE_DATA_SYNC)** — used only briefly while a voice-recognition model download is in progress, so it can continue and show a progress notification.
- **Boot completed** — a normal Android permission with no runtime prompt. After the phone reboots, Android wipes its alarm queue; this permission lets the app re-arm its two scheduled alarms (the optional daily summary notification at 23:59 and the recurring-rule daily catch-up at 00:01). It touches no user data and triggers no network activity.


## Optional Google Drive backup

If you connect Google Drive in Settings → Backup & restore:

- The app writes backup files into your **own Google Drive's AppData folder** — a private space that **only this app can read or write**.
- We never see what you back up. The data is between you and Google.
- The app requests only the `https://www.googleapis.com/auth/drive.appdata` permission — it cannot see any of your other Drive files.
- **How the data is protected:**
  - In transit: HTTPS to Google Drive.
  - At rest on Google's servers: encrypted by Google.
  - **The backup file itself is plain JSON.** If someone gains access to your Google account, they can read your backed-up transactions. We recommend a strong Google account password and two-factor authentication.
- To remove access at any time: Google Account → Security → Third-party apps with account access → aLike Expense Manager → Remove access. Google will then delete the AppData folder automatically.

## Optional voice-recognition model download

Voice entry needs a Whisper speech model. The default model (Whisper-tiny, ~99 MB) is delivered via Google Play's standard on-demand asset-pack mechanism the first time you turn on voice in Settings — the pack is fetched from Google Play's CDN over HTTPS. Once installed, voice runs entirely on-device.

If you want better recognition you can opt into larger models (Whisper-base, Whisper-small) from Settings → Voice input. Those download from the open-source sherpa-onnx project's GitHub releases over HTTPS only when you tap Download.

No telemetry is sent from the app for either path. Whisper transcription always happens locally — audio never leaves the device.

## Your data rights (GDPR, UK GDPR, India DPDP Act, and similar laws)

Modern data-protection laws — EU GDPR, UK GDPR, India's DPDP Act 2023, Brazil's LGPD, California's CCPA, and others — all give you a similar set of rights over your personal data: access it, correct it, delete it, take it elsewhere.

aLike Expense Manager is an unusual case because **there is no developer-side data**. We operate no servers; we collect no analytics; we never read, copy, or receive your transactions, accounts, budgets, or voice. Everything lives on your own device, and (only if you opt in) a backup file in your own Google Drive's app-private folder.

That means:

- **Access:** the data is already in your hand inside the app. The Reports and Transactions screens are your access surface; **Settings → Backup & restore** can produce an exportable JSON file you can save anywhere.
- **Correction:** edit any transaction, account, or budget directly in the app.
- **Deletion ("right to be forgotten"):** uninstalling the app removes every byte of local data from your device. If you turned on Drive backup, you can delete the backup folder from your Google account under *drive.google.com → ⚙ Settings → Manage apps*, or revoke the app's Drive access at *myaccount.google.com → Security → Third-party access*.
- **Portability:** the in-app export produces a structured JSON file you can carry anywhere.
- **Objection / restriction of processing:** doesn't apply — we don't process your data on our side at all.
- **Complaints:** EU users may complain to their national Data Protection Authority. UK users may complain to the ICO at *ico.org.uk/make-a-complaint*. Indian users may complain to the Data Protection Board of India once it is constituted under the DPDP Act.

We don't operate a Subject Access Request portal because there is no developer-side data to request. The same applies to deletion, portability, and so on. The only thing we hold about any individual user is whatever you choose to send us in an email — which is voluntary and never required to use the app.

If you have questions, write to **eightelephantsgroup@gmail.com**.

**This stance does not change based on the user's region.** We treat every user the same regardless of where they live.


## Pro upgrade (in-app purchase)

If you upgrade to Pro:

- The purchase is processed by Google Play. Google sends us a receipt confirming the purchase, but **we never see your payment card or billing details**.
- The Pro entitlement is stored on your device and validated against Google Play.

## Analytics, advertising, third-party SDKs

- **No analytics SDK**. We do not collect crash reports, usage stats, or any telemetry.
- **No advertising**. The app has no ads and no advertising IDs are accessed.
- **No tracking**. We do not share any data with third parties because we do not collect any data to share.

## Children's privacy

The app is not directed at children under 13. We do not knowingly collect data from anyone, including children.

## Changes to this policy

If we change this policy, we will update the "Effective date" at the top and update the in-app About screen to surface the new version. Material changes will be flagged in release notes.

## Contact

Questions or concerns: **eightelephantsgroup@gmail.com**
