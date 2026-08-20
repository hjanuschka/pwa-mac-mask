# macOS Maskable PWA Test

Minimal installable PWA for testing Chromium issue 423939352.

The manifest supplies a full-bleed blue icon with `purpose: maskable`.
On macOS 26, the installed app's `app.icns` should retain the original
unmasked image while Finder and Dock apply the native system shape.

Live test: https://www.januschka.com/pwa-mac-mask/

The page includes reference PNGs for the expected `app.icns` contents:

- macOS 25 and earlier: Chrome-masked icon, captured with Canary 154 on
  macOS 15.6.
- macOS 26: original full-bleed icon; Finder and Dock apply the system shape.

The macOS 26 reference represents the file contents, not Finder's rendered
appearance.
