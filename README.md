# macOS Maskable PWA Test

Minimal installable PWA for testing Chromium issue 423939352.

The manifest supplies a full-bleed blue icon with `purpose: maskable`.
On macOS 26, the installed app's `app.icns` should retain the original
unmasked image while Finder and Dock apply the native system shape.

Live test: https://hjanuschka.github.io/pwa-mac-mask/
