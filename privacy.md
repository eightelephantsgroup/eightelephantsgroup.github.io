# Privacy Policy

**App:** aLike Expense Manager
**Developer:** Eight Elephants Group
**Package:** com.eightelephantsgroup.expmanager
**Effective date:** 2 June 2026
**Contact:** eightelephantsgroup@gmail.com

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

The app ships with a small voice-recognition model. If you choose to download a larger one for better accuracy:

- Models are downloaded from `github.com/k2-fsa/sherpa-onnx/releases`, an open-source project.
- Downloads happen only when you tap "Download" in Settings → Voice input.
- We do not send any telemetry with the download request.

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
