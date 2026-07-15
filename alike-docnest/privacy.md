---
title: Privacy Policy — aLike DocNest
---

# Privacy Policy — aLike DocNest

**Last updated: 15 July 2026**

aLike DocNest ("the app") is a private, offline-first family document manager published by
**Eight Elephants Group** ("we", "us"). This policy explains what the app does and does not do with
your information. It is written to match how the app actually behaves.

## The short version

- **No account, no sign-up.** You don't create an account or give us an email to use the app.
- **Your data stays on your device.** Documents, photos, family details and categories are stored
  locally and **encrypted at rest** on your device.
- **We don't collect, see, sell, or share your data.** No analytics, no advertising, no tracking.
  Nothing you add to the app is sent to us.
- **Backups are optional and go to *your own* Google Drive** — not to us.
- **Text recognition, document scanning, and voice search all run on your device.**

## What the app stores, and where

Everything you create in the app — document files, scanned PDFs, member photos, document details
(titles, numbers, dates, notes, tags), family member profiles, and categories — is stored **only on
your device**, in the app's private storage. Files and the database are **encrypted at rest** using
your device's hardware-backed keystore.

We do **not** operate servers that receive your documents, and we have no ability to access your data.

## Permissions the app uses

- **Notifications** (optional): to remind you when a document is due for renewal. Reminders are
  generated on your device. You can decline this; you simply won't get reminders.
- **Microphone** (optional, for voice search): used only while you actively use voice search to speak
  a search query. Speech is processed **on your device**; audio is not recorded, stored, or sent
  anywhere.
- **Foreground service while downloading the voice model** (only when you choose to download a
  voice-search model): the app shows a progress notification and keeps the download running if you
  switch apps. It is used solely for that download and stops when the download finishes.

The app does **not** request storage or camera permissions. Choosing a document uses the system file
picker, choosing a photo uses the Android photo picker, and scanning uses Google Play Services'
on-device document scanner — each grants access only to the specific item you pick.

## Document scanning and text recognition

Scanning uses the **Google Play Services ML Kit document scanner**, and text recognition (OCR) uses
**ML Kit on-device text recognition**. Both run **locally on your device**; your document images and
recognized text are not uploaded to us or to a third party for these features. Google's handling of
its on-device libraries is governed by Google's own terms.

## Voice search

Voice search lets you find your documents by speaking instead of typing. Speech recognition runs
**entirely on your device** using an offline model (Whisper via sherpa-onnx). Your voice is processed
locally; the audio is **never recorded, stored, or sent** to us or any third party.

The speech-recognition **model files** are downloaded over the internet the first time you use voice
search (and you can optionally download larger, more accurate models). Only the model files are
downloaded **to** your device — no document data, audio, or personal information is sent as part of
this. The default model is delivered through **Google Play**; Google's handling of that delivery is
governed by Google's own terms.

## Optional Google Drive backup

If — and only if — you choose to set up backup, the app:

1. Asks you to connect a Google account using Google's standard account picker and consent screen.
2. Creates an **encrypted backup bundle** on your device and uploads it to a **private app-data folder
   in your own Google Drive**. That folder is only accessible to this app on your account; other apps
   and people cannot see it, and **we cannot see it**.
3. Lets you restore that backup to a device.

We never receive your backup. It lives in your Google Drive under your control. Your use of Google
Drive is also subject to [Google's Privacy Policy](https://policies.google.com/privacy). You can
delete backups from within the app or from your Google Drive at any time. The app's access is limited
to the Drive **app-data** scope (this app's private folder); it cannot read the rest of your Drive.

## App lock

You may optionally set a PIN and/or biometric lock. The PIN is stored **only on your device** as a
salted hash; it never leaves the device and we never see it.

## Children

The app is a general-purpose tool for organizing family documents and is **not directed at children**,
and we do not knowingly collect any personal information from children.

## Your control and data deletion

- You can edit or delete any document, member, or category in the app at any time.
- **Uninstalling the app removes all of its local data** from your device.
- If you set up Drive backup, you can delete the backups in-app or from your Google Drive.

## Changes to this policy

If we change this policy we will update the "Last updated" date above and, for material changes, note
it in the app.

## Contact

Questions about this policy: **eightelephantsgroup@gmail.com**.
