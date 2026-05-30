# Frequently Asked Questions (FAQ)

> **Language:** English | [简体中文](FAQ.zh-Hans.md)

---

## General

**Q: Does PouchVerse require an internet connection?**  
A: No. All core features — importing, searching, previewing, organising — work completely offline. The only exception is the optional LAN Transfer feature, which uses your local network (not the internet) to connect devices directly.

**Q: Do I need to create an account?**  
A: No account is required. PouchVerse has no login, no sign-up, and no cloud service.

**Q: What happens to my data if I uninstall the app?**  
A: All data (files, database, thumbnails, indexes) is stored in the app's on-device sandbox. Uninstalling permanently deletes everything. **Please back up important files before uninstalling.**

**Q: Is there a subscription fee?**  
A: PouchVerse is a **one-time purchase** — no subscription, no ads, no in-app purchases.

---

## Import & Files

**Q: What file formats are supported?**  
A: PouchVerse supports 80+ formats including images (JPG, PNG, HEIC, RAW...), video (MP4, MOV, MKV, AVI, RMVB...), audio (MP3, FLAC, AAC, WAV, MIDI...), documents (PDF, DOCX, XLSX, PPTX, Pages, Numbers, Keynote...), code (Swift, Python, JS, TS, 50+ languages), archives (ZIP, RAR, 7Z, TAR...), and more.

**Q: I imported the same file twice. Why is there only one copy?**  
A: PouchVerse uses **SHA-256 content hashing** to detect identical files. If you import a file with the same content as an existing one (regardless of filename), it is silently deduplicated — no storage is wasted.

**Q: Can I import files from third-party apps like WeChat?**  
A: Yes. In any app, find the file, tap **Share → Copy to PouchVerse**. If the app supports the iOS share sheet, PouchVerse will appear as a destination. You can also use the **PouchVerse Share Extension** which installs alongside the main app.

---

## Search

**Q: Why doesn't OCR search work immediately after import?**  
A: OCR indexing runs in the background after import. It may take a few seconds to a minute depending on the number of files and device performance. Once done, text within images is fully searchable.

**Q: Can I search inside ZIP / RAR archives?**  
A: You can browse the internal directory of archives and preview files inside them. Full-text search within archived files is not supported in v1.0.

**Q: How do I search for Chinese files by Pinyin?**  
A: Just type the Pinyin or initials in the search bar. For example, type `ndbg` or `niandubao` to find files named `年度报告`. This works automatically — no setup required.

---

## LAN Transfer

**Q: Do both devices need PouchVerse installed?**  
A: Yes, for iOS transfers both devices need PouchVerse. **PouchVerse Transfer** (macOS / Windows companion app for LAN file transfer) and the Android version will be available soon and will interoperate with the iOS version.

**Q: The other device isn't showing up in the transfer list. What should I do?**  
A: 1. Ensure both devices are on the same Wi-Fi network. 2. Grant **Local Network** permission (Settings → Privacy & Security → Local Network → PouchVerse). 3. Make sure the receiving device has **LAN Receive** enabled in the sidebar.

**Q: Is the transfer encrypted?**  
A: No. LAN Transfer is peer-to-peer but **not encrypted**. Avoid transferring sensitive files over untrusted public Wi-Fi networks.

---

## Private Files

**Q: Are private files encrypted on disk?**  
A: No. The Private Files feature provides **in-app access control** (Face ID / Touch ID / passcode) but does not encrypt files on the filesystem. On a jailbroken device or if someone has physical access to your device and knows your passcode, files may be accessible. For maximum security, use iOS's full-device encryption (enabled by default when you set a device passcode).

**Q: I forgot my passcode. Can I recover access to private files?**  
A: If you forget your device passcode and can no longer authenticate, there is no recovery path — the private section remains locked. Since all data is local, EJIANDAN has no access to your files.

---

## Privacy & Data

**Q: Does PouchVerse send any data to servers?**  
A: No. See our [Privacy Policy](../Legal/Privacy-Policy.md) for full details. In summary: no data is collected, no files are uploaded, and no analytics SDKs are included.

**Q: Does audio transcription send audio to the cloud?**  
A: No. Speech-to-text uses Apple's Speech framework with `requiresOnDeviceRecognition = true` enforced — audio is never sent to any server.

---

## Feedback & Support

**Q: How do I report a bug or request a feature?**  
A: [Open an issue](https://github.com/ejiandan/PouchVerse-release/issues) on GitHub, or email support@ejiandan.com.

---

*Can't find your answer? Email us: support@ejiandan.com*
