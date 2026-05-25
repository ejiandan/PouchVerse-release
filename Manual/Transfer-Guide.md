# LAN Transfer Guide

> **Language:** English | [简体中文](Transfer-Guide.zh-Hans.md) | [繁體中文](Transfer-Guide.zh-Hant.md) | [日本語](Transfer-Guide.ja.md) | [한국어](Transfer-Guide.ko.md) | [Español](Transfer-Guide.es.md)

PouchVerse supports high-speed **peer-to-peer LAN file transfer** across all platforms. No internet required, no relay server — files travel directly between your devices.

---

## Platform Support Matrix

| Sender → Receiver | iOS | macOS | Android | Windows |
|---|---|---|---|---|
| **iOS** | ✅ | ✅ | ✅ | ✅ |
| **macOS** | ✅ | ✅ | ✅ | ✅ |
| **Android** | ✅ | ✅ | ✅ | ✅ |
| **Windows** | ✅ | ✅ | ✅ | ✅ |

> macOS, Android, and Windows apps are **coming soon**.

---

## How It Works

PouchVerse uses **Bonjour (mDNS)** for automatic device discovery on the same local network, and a custom **TCP protocol (port 52013)** for direct peer-to-peer transfer. No registration, no pairing codes, no cloud relay.

For Apple devices (iPhone ↔ iPhone, iPhone ↔ Mac), direct **peer-to-peer Wi-Fi** is supported — no access point or internet required.

---

## iOS → iOS Transfer (Step by Step)

### On the Receiving Device
1. Open PouchVerse
2. Tap **☰** (sidebar) → enable **LAN Receive**
3. The device is now discoverable on the local network

### On the Sending Device
1. Long-press the file(s) you want to send
2. In the radial menu, tap **Transfer**
3. Available devices appear in the list — tap the target device
4. Transfer starts immediately; progress is shown on both devices

---

## Troubleshooting

**Device not showing up?**
- Ensure both devices are on the same Wi-Fi network (or use Apple peer-to-peer Wi-Fi)
- Check that **Local Network** permission is granted: Settings → Privacy & Security → Local Network → PouchVerse ✅
- Ensure LAN Receive is enabled on the receiving device

**Transfer is slow?**
- Wi-Fi 5 GHz band is recommended for best performance
- Avoid transferring large files over a congested 2.4 GHz network

**Transfer interrupted?**
- Keep both apps in the foreground during transfer
- iOS may background the app when the screen turns off — keep the screen on

---

## Privacy & Security

- All transfers are **peer-to-peer** with no relay server
- Transfers pass through **no third-party service**
- **Transfers are not encrypted** — avoid sending sensitive files over untrusted public Wi-Fi networks
- The receiving device must explicitly enable LAN Receive — passive discovery only

---

*Questions? See [FAQ](FAQ.md) or contact support@ejiandan.com*
