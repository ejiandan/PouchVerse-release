# Privacy Policy — Pouch Transfer (macOS)

**Effective Date: May 27, 2026**
**Applicable Product: Pouch Transfer (macOS)**
**Published by: EJIANDAN LIMITED (藝簡單有限公司)**

---

## 1. Overview

Pouch Transfer is a **local-only, peer-to-peer LAN file transfer tool** for macOS. It requires no account registration, collects no personal data, and never uploads any files or metadata to any server.

---

## 2. Information We Do Not Collect

We **never** collect, store, upload, or share:

- Your name, email address, or any personally identifiable information
- Your location, device advertising identifier, or tracking identifiers
- Any file names, file contents, or file metadata you transfer
- Your network usage behaviour or device information
- Any data used for advertising, analytics, or profiling

Pouch Transfer **does not include any third-party SDK, analytics service, advertising network, or cloud service**.

---

## 3. Data Processed Locally

The app stores the following data **only on your Mac**, never transmitted anywhere:

| Data | Location | Purpose |
|---|---|---|
| Preferences (language, receive toggle) | `UserDefaults` | App configuration |
| Temporary transfer state | Memory only | Transfer progress display |

All data is removed when the app is uninstalled.

---

## 4. Network Activity

- **LAN only**: Pouch Transfer uses Bonjour (mDNS) to discover peer devices on the same local network, and transfers files via a direct TCP connection (port 52013 or 52014).
- **No internet access**: No data is sent to any remote server at any time.
- **No relay**: Transfers are direct, peer-to-peer, and pass through no intermediate server.
- **Not encrypted**: LAN transfers are unencrypted. Avoid transferring sensitive files over untrusted public networks.

---

## 5. System Permissions

| Permission | Required | Purpose | Effect if Denied |
|---|---|---|---|
| **Local Network** | No | Discover peer devices via mDNS | Only affects device discovery |
| **Downloads folder** | No | Save received files | Received files will not be saved |

Pouch Transfer does **not** request internet access, contacts, calendar, camera, microphone, location, or any other permissions.

---

## 6. Contact

If you have any questions about this Privacy Policy, please open an issue on our GitHub repository:
[https://github.com/ejiandan/PouchVerse-release/issues](https://github.com/ejiandan/PouchVerse-release/issues)

---

*This policy applies to Pouch Transfer for macOS only. See the [iOS Privacy Policy](../Legal/Privacy-Policy.md) for the iOS version of PouchVerse.*
