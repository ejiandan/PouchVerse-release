# PouchVerse Privacy Policy

**Effective Date: May 29, 2026**
**Applicable Product: PouchVerse (Android)**
**Published by: Beijing EJIANDAN Network Technology Co., Ltd.**

---

## 1. Overview

We are committed to a **local-first / offline-capable** product philosophy. PouchVerse is a local file aggregation and management tool that requires no account registration, collects no personal data, and never uploads any of your files or metadata to any server. This policy transparently explains what the app does and does not do on your Android device, and how you remain in control.

---

## 2. Information We Do **Not** Collect

We **never** collect, store, upload, or share any of the following:

- Your name, phone number, email address, ID number, or any other personally identifiable information
- Your location, device unique identifiers (IMEI / Android ID / advertising ID AAID), or any tracking identifiers
- Any file content or file names you import, view, organise, or transfer
- Your search queries, browsing history, or in-app usage behaviour
- Your contacts, calendar, photo library metadata, or health data
- Any data used for tracking, profiling, marketing, or advertising

PouchVerse **does not include any third-party SDK, analytics service, advertising network, or push notification service**.

---

## 3. Data Processed On-Device

To provide core functionality, the following data is stored **exclusively within the app's private directory** (inaccessible to other apps) and never leaves your device:

| Data | Location | Purpose |
|---|---|---|
| Imported file content | `files/store/` | File management and preview |
| File metadata (name, size, type, date, colour tag, usage tag, etc.) | `databases/pouchverse.db` | List display, filtering, and sorting |
| Full-text search index (FTS5) | `databases/pouchverse.db` | Keyword search |
| Thumbnails | `files/thumbs/` | List previews |
| Content hash (SHA-256) | `databases/pouchverse.db` | Duplicate detection |
| Preferences | `SharedPreferences` | Video seek step, language settings, etc. |

Uninstalling PouchVerse **permanently deletes** all of the above data.

---

## 4. System Permissions

- **Storage / Document Picker**: Import files via the system document picker.
- **Media** (if used): Import photos or videos from the gallery / media library.
- **Nearby Devices / Local Network**: Discover devices and transfer files over LAN.
- **Microphone**: The app does not actively request recording permission; audio text extraction uses on-device offline recognition and audio never leaves the device.
- **Biometrics / Device Credentials**: Unlock the in-app "Private Files" section.

PouchVerse does **not** request internet access (including cellular data), push notifications, camera, location, contacts, calendar, or motion permissions. (Note: the Android `INTERNET` permission is used solely by the LAN feature for local Wi-Fi socket communication and never interacts with any remote server.)

---

## 5. Network Activity

- **No internet connectivity**: PouchVerse does not send or receive any data to or from any remote server.
- **LAN Transfer**: Only when you actively use the "LAN Transfer" feature does PouchVerse use mDNS / NSD to discover peer devices on the same local network and transfer files you select via a custom TCP protocol (port 52013), directly peer-to-peer.
  - LAN transfers pass through **no relay server**; sender and receiver connect directly peer-to-peer.
  - Transfers are not encrypted; please avoid transferring sensitive files over untrusted public Wi-Fi networks.

---

## 6. Private Files

The "Private Files" feature uses the Android system BiometricPrompt (fingerprint / face / device PIN / pattern / password) to provide a **secondary in-app access control layer** for hidden private folders. Please note:

- Private files are **not encrypted on disk**; their privacy boundary relies on membership flags, in-memory unlock state, and UI concealment.
- The app **immediately re-locks** when it is backgrounded or closed; re-authentication is required on next access.
- On rooted devices, or devices that have been physically accessed by someone who knows the device credentials, files may be accessible.

---

## 7. Children's Privacy

PouchVerse is a general-purpose application and is not directed at children. If a minor under the age of 14 uses this app, it should be under the supervision of a parent or guardian who manages device permissions and imported content.

---

## 8. Third-Party Open-Source Components

PouchVerse statically links the following open-source libraries. **No data is transmitted through any of them.**

- FFmpeg (LGPL 2.1+): Local video / audio decoding
- unrar (UnRAR Licence, extract-only): RAR archive extraction
- zlib (zlib Licence): DEFLATE decompression
- SQLite3 (Public Domain): Local database
- AndroidX / Jetpack Compose (Apache 2.0): UI framework

Full licence texts are available in-app under **Sidebar → Licences**.

---

## 9. Data Export and Deletion

- **Export**: Long-press a file row → Share, or share the file directly to the system file manager / another app.
- **Delete**: Swipe left on any file row to delete it, or uninstall the app from system settings to permanently remove all local data.
- Because all data resides entirely on your device, **we are unable and will never attempt** to remotely recover data you have deleted.

---

## 10. Changes to This Policy

If this policy is materially updated, the new version will be announced via the **About PouchVerse → Privacy Policy** page within the app. Continued use of the app after any change constitutes acceptance of the updated policy.

---

## 11. Contact Us

If you have any questions, comments, or complaints regarding this Privacy Policy, please contact us at:

- Company: Beijing EJIANDAN Network Technology Co., Ltd.
- Email: support@ejiandan.com
