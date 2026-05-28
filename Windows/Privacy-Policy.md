# Privacy Policy — PouchVerse (Windows)

**Effective Date: May 29, 2026**
**Applicable Product: PouchVerse (Windows)**
**Published by: EJIANDAN LIMITED (藝簡單有限公司)**

---

## 1. Overview

PouchVerse is a **local-only, peer-to-peer LAN file transfer tool** for Windows. It requires no account registration, collects no personal data, and never uploads any files or metadata to any server.

---

## 2. Information We Do Not Collect

We **never** collect, store, upload, or share:

- Your name, email address, or any personally identifiable information
- Your location, device advertising identifier, or tracking identifiers
- Any file names, file contents, or file metadata you transfer
- Your network usage behaviour or device information
- Any data used for advertising, analytics, or profiling

PouchVerse **does not include any third-party SDK, analytics service, advertising network, or cloud service**.

---

## 3. Data Processed Locally

The app stores the following data **only on your Windows PC**, never transmitted anywhere:

| Data | Location | Purpose |
|---|---|---|
| Preferences (language, receive toggle) | `%AppData%\PouchTransfer` | App configuration |
| Temporary transfer state | Memory only | Transfer progress display |

All data is removed when the app is uninstalled.

---

## 4. Network Activity

- **LAN only**: PouchVerse uses mDNS to discover peer devices on the same local network, and transfers files via a direct TCP connection (port 52013 or 52014).
- **No internet access**: No data is sent to any remote server at any time.
- **No relay**: Transfers are direct, peer-to-peer, and pass through no intermediate server.
- **Not encrypted**: LAN transfers are unencrypted. Avoid transferring sensitive files over untrusted public networks.

---

## 5. System Permissions

| Permission | Required | Purpose | Effect if Denied |
|---|---|---|---|
| **Windows Firewall** | No | Allow inbound LAN connections for file receiving | Receiving files will not work; sending is unaffected |

PouchVerse does **not** request internet access, contacts, calendar, camera, microphone, location, or any other permissions beyond local network communication.

---

## 6. Contact

If you have any questions about this Privacy Policy, please open an issue on our GitHub repository:
[https://github.com/ejiandan/PouchVerse-release/issues](https://github.com/ejiandan/PouchVerse-release/issues)

---

*This policy applies to PouchVerse for Windows only. See the [iOS Privacy Policy](../Legal/Privacy-Policy.md) for the iOS version of PouchVerse.*
