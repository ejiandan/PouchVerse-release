# PouchVerse — iOS Changelog

---

## v1.0.1

**Status:** Submitted to App Store · TestFlight Public Beta Approved  
**TestFlight:** <https://testflight.apple.com/join/8t2n7tmd>

### Bug Fixes

#### File Transfer

- Fixed an issue where a failed transfer item could automatically restart after cancelling and retrying when transferring files from Mac to iPhone.
- Improved state handling logic after transfer interruption for better stability and interaction consistency.

#### Video Preview

- Fixed an issue where the document switch button and lock button overlapped in landscape mode.
- Adjusted lock button layout to improve the landscape operation experience.

### Improvements

#### Video Preview Help Tip

- Added a help button (**?**) on the playback interface.
- Tap the help button to view seek operation instructions; tap again to dismiss.
- Supports multi-language localization.

#### Seek Zone Description

| Zone | Behavior |
|---|---|
| Top zone | Precise positioning (smaller step) |
| Bottom zone | Fast positioning (larger step) |

---

## v1.0

**Status:** Live on App Store
**App Store:** <https://apps.apple.com/app/id6766184837>  
**TestFlight:** <https://testflight.apple.com/join/8t2n7tmd>

### Initial Release

#### File Unification

- Import files from any app, system file picker, or LAN transfer into one unified, indexed library.

#### Physical Deduplication

- SHA-256 fingerprinting identifies identical content regardless of filename, preventing duplicate storage. Saves significant space on 128 GB / 256 GB devices.

#### 6D Flexible Organization

- Organize with virtual folders, tags, color importance (5 levels), usage labels, and time dimensions.
- One file can belong to multiple virtual folders and tags simultaneously — no physical duplication.

#### Instant Offline Search

- Full-text search across filenames, document body, and image OCR text; supports Chinese pinyin / initials.
- On-demand audio transcription — entirely on-device, no internet required.

#### All-Format Preview

- 80+ file formats: video, audio, images, PDF, Office documents, code, archives, ISO, and more.
- One-tap preview without leaving the app.

#### Pro Media Player

- Custom dual-zone video seek controls: top zone for precise positioning, bottom zone for fast seeking.
- Audio player with rich artwork display and lyrics support.

#### Cross-Platform LAN Transfer

- Bonjour peer discovery + custom TCP direct transfer; no relay server, no account required.
- Apple devices can transfer directly without Wi-Fi.

#### Biometric Private Space

- Face ID / Touch ID protected in-app private folder; auto-locks on every background entry.
- 100% local storage — private content never uploaded to any server.

#### Multi-Language Support

- Simplified Chinese, Traditional Chinese, English, Japanese, Korean, Spanish.
