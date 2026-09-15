# LaserDx — Capacitor iOS starter

This is a ready-to-go project shell for your `laserdx_v4_42_responsive.html` app.

- `www/index.html` — your app, copied in as-is (nothing was changed).
- `package.json` — Capacitor 8 dependencies.
- `capacitor.config.json` — points `webDir` at `www/`, with `contentInset: automatic`
  set on iOS so your fixed header sits below the status bar/notch instead of behind it.

## Use it

1. Unzip this folder wherever you want your project to live.
2. Open a terminal in that folder.
3. Run:
   ```
   npm install
   npx cap add ios
   npx cap sync ios
   npx cap open ios
   ```
4. Before you `npx cap add ios`, open `capacitor.config.json` and replace
   `"com.yourcompany.laserdx"` with your real reverse-DNS bundle ID
   (e.g. `com.acmederm.laserdx`) — this has to match what you register in
   App Store Connect, and it's much more annoying to change later.

Full step-by-step (Xcode signing, archive, App Store Connect upload, and the
App Store pitfalls specific to this build) is in the chat where this came from.
