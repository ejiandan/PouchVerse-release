# PouchVerse Privacy Policy

**Effective Date: April 26, 2026**
**Applicable Product: PouchVerse (iOS)**
**Published by: EJIANDAN LIMITED (藝簡單有限公司)**

---

## 1. Overview

We are committed to a **local-first / offline-capable** product philosophy. PouchVerse is a personal file management tool that requires no account registration, collects no personal data, and never uploads any of your files or metadata to any server. This policy transparently explains what the app does and does not do on your iOS device, and how you remain in control.

---

## 2. Information We Do **Not** Collect

We **never** collect, store, upload, or share any of the following:

- Your name, phone number, email address, or any other personally identifiable information
- Your location, device advertising identifier (IDFA / IDFV), or any tracking identifiers
- Any file content or file names you import, view, organise, or transfer
- Your search queries, browsing history, or in-app usage behaviour
- Your contacts, calendar, photo library metadata, or health data
- Any data used for tracking, profiling, marketing, or advertising

PouchVerse **does not include any third-party SDK, analytics service, advertising network, or push notification service**.

---

## 3. Data Processed On-Device

To provide core functionality, the following data is stored **exclusively within the app's on-device sandbox** and never leaves your device:

| Data | Location | Purpose |
|---|---|---|
| Imported file content | `Documents/store/` | File management and preview |
| File metadata (name, size, type, date, colour tag, usage tag, etc.) | `Documents/pouchverse.db` | List display, filtering, and sorting |
| Full-text search index (FTS5) | `Documents/pouchverse.db` | Keyword search |
| Pinyin / initials index, image OCR text and scene tags, audio transcription text | `Documents/pouchverse.db` (within the FTS index) | Enhanced local search; all generation is performed offline on-device |
| Thumbnails | `Documents/thumbs/` | List previews |
| Content hash (SHA-256) | `Documents/pouchverse.db` | Duplicate detection |
| Preferences | `UserDefaults` | Video seek step, LAN transfer toggle, language settings, etc. |

Uninstalling PouchVerse **permanently deletes** all of the above data.

---

## 4. System Permissions

| Permission | Required | Purpose | Effect if Denied |
|---|---|---|---|
| **Files / Document Picker** | No (on demand) | Import files via the iOS Files app or document picker | Only affects that import source |
| **Photo Library** (if used) | No | Import photos or videos from your photo library | Only affects photo library imports |
| **Local Network** | No | Discover nearby devices and transfer files over LAN | Only affects the LAN Transfer feature |
| **Speech Recognition** | No | On-demand transcription — only invoked when you explicitly tap the "Extract Text" button on the audio preview screen; device-only recognition is enforced (`requiresOnDeviceRecognition = true`); audio never leaves the device; not triggered on import | Only affects the audio text extraction feature |
| **Face ID / Touch ID / Passcode** | No | Unlock the "Private Files" section within the app | Only affects access to Private Files |

PouchVerse does **not** request internet access, push notifications, microphone (the Speech framework is used without microphone input), camera, location, contacts, calendar, or motion permissions.

---

## 5. Network Activity

- **No internet connectivity**: PouchVerse does not send or receive any data to or from any remote server.
- **On-device offline intelligence**: Pinyin indexing, image OCR and scene classification, and audio speech-to-text all use Apple's **Vision** and **Speech** system frameworks and are processed entirely on-device without any network connection; speech recognition enforces `requiresOnDeviceRecognition = true`.
- **LAN Transfer**: Only when you actively use the "LAN Transfer" feature does PouchVerse use Bonjour (mDNS) to discover peer devices on the same local network and transfer files you select via a custom TCP protocol (port 52013), directly peer-to-peer.
  - LAN transfers pass through **no relay server**.
  - Transfers are not encrypted; please avoid transferring sensitive files over untrusted public Wi-Fi networks.

---

## 6. Private Files

The "Private Files" feature uses iOS Local Authentication (Face ID / Touch ID / device passcode) to provide a **secondary in-app access control layer** for a dedicated private folder. Please note:

- Private files are **not encrypted on disk**; their privacy boundary relies on membership flags, in-memory unlock state, and UI concealment.
- The app **immediately re-locks** when it is backgrounded or closed; re-authentication is required on next access.
- On jailbroken devices, or devices that have been physically accessed by someone who knows the device passcode, files may be accessible outside of the app.

---

## 7. Children's Privacy

PouchVerse is a general-purpose application and is not directed at children under the age of 13 (or the applicable age in your jurisdiction). If a child under 13 uses this app, it should be under the supervision of a parent or guardian who manages device permissions and imported content.

---

## 8. Third-Party Open-Source Components

PouchVerse statically links the following open-source libraries. **No data is transmitted through any of them.**

| Library | Licence | Use |
|---|---|---|
| FFmpeg | LGPL 2.1+ | Local video / audio decoding |
| unrar | UnRAR Licence (extract-only) | RAR archive extraction |
| zlib | zlib Licence | DEFLATE decompression |
| SQLite3 | Public Domain | Local database |
| FreePats General MIDI soundfont | CC0 1.0 Universal | MIDI playback |

Full licence texts are available in-app under **Sidebar → Licences**.

---

## 9. Data Export and Deletion

- **Export**: Long-press a file in the list → Share, or share the file directly to the Files app or any other app.
- **Delete**: Swipe left on any file in the list to delete it, or uninstall PouchVerse from iOS Settings to permanently remove all local data.
- Because all data resides entirely on your device, **we are unable and will never attempt** to remotely recover data you have deleted.

---

## 10. Changes to This Policy

If this policy is materially updated, the new version will be announced via the **About PouchVerse → Privacy Policy** page within the app. Continued use of the app after any change constitutes acceptance of the updated policy.

---

## 11. Contact Us

If you have any questions, comments, or complaints regarding this Privacy Policy, please contact us at:

- Company: EJIANDAN LIMITED (藝簡單有限公司)
- Email: support@ejiandan.com

---

© EJIANDAN LIMITED (藝簡單有限公司). All rights reserved.
