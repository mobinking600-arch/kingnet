# KingNet — Real WireGuard Android Client

This project uses the official embeddable WireGuard Android tunnel library:

`com.wireguard.android:tunnel:1.0.20260102`

The official WireGuard Android project documents this library as the embeddable tunnel
library and its `GoBackend` uses the non-root userspace WireGuard implementation. The
backend creates the Android `VpnService` tunnel and configures routes, DNS, MTU and
WireGuard peers.

## Important
This version contains the REAL WireGuard backend integration and VPN permission flow.
The UI is intentionally kept small while the backend is wired for real tunnel
activation.

A production-ready build should still add:
- persistent profile storage
- `.conf` file picker/import
- QR scanner
- profile editor
- live statistics
- notification/foreground-service polish
- release signing

## Build
Open in Android Studio, sync Gradle, then Build > Build APK(s).

No test `.conf` is included. You need a valid WireGuard profile from your own server.

## Legal/licensing
The embedded WireGuard tunnel library is licensed by the WireGuard project under
Apache-2.0. Keep its license/notice requirements when distributing the app.
\n## KingNet branding\nThe main screen includes the visible `Powered by KingNet` brand mark.\n
## Launcher icon
The supplied KingNet logo image is used as the app launcher icon.\n