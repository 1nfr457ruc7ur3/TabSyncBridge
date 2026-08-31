# TabSyncBridge

<p align="center">
  <img src="https://indexridge.github.io/TabSyncBridge/tabsyncbridge-app-icon-1024.png" width="128" alt="TabSyncBridge Icon">
</p>

<h3 align="center">Sync Safari & Chrome Tabs Together — No iCloud or Google Account</h3>

<p align="center">
  Private local-network tab sync and remote tab control for your own iPhone, Safari, Chromium-family browsers, and linked desktop setup.
</p>

<p align="center">
  <a href="https://apps.apple.com/us/app/tabsyncbridge/id6766262129">
    <img src="https://img.shields.io/badge/Download_on_the-App_Store-000000?style=for-the-badge&logo=apple" alt="Download on the App Store">
  </a>
  <a href="https://chromewebstore.google.com/detail/tabsyncbridge/fbhngbfbapkkhcdpijagknchlcmcfmgl">
    <img src="https://img.shields.io/badge/Available_in the-Chrome_Web_Store-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Available in the Chrome Web Store">
  </a>
</p>

---

## 🚫 Stop sending your tabs through the cloud

Are you tired of signing into Google Sync on your Mac just to see your Chrome tabs on your iPhone? Do you want to use Safari on iOS and Edge on Windows without jumping through hoops?

**TabSyncBridge** is the definitive private alternative to iCloud Tabs and Chrome Sync. It syncs your tabs locally over your own Wi-Fi. 

- **No Cloud Accounts:** No signing into third-party sync servers.
- **Cross-Browser:** Sync between Safari (iOS) and Chrome, Edge, Brave, Opera, Chromium (Desktop).
- **Privacy-First:** Your tab titles, URLs, and device identifiers never leave your network.
- **Remote Control:** Close a forgotten desktop tab straight from your iPhone.

## 🛠️ Architecture: How it works without the cloud

Unlike standard sync services that route your data through external databases, TabSyncBridge operates exclusively on your local network (LAN) using standard web protocols.

1. **Discovery:** The iOS app and desktop bridge discover each other over your private Wi-Fi network using zero-configuration networking (Bonjour/mDNS).
2. **Direct Peer-to-Peer:** Once paired, a direct local WebSocket connection is established on port `53317`.
3. **Payload Exchange:** Tab snapshots (URL, Title, Origin) are exchanged directly between devices.
4. **Native Messaging Bridge:** On desktop, a lightweight native host script securely relays the WebSocket data into your isolated Chromium extension without needing a local web server running in the background.

This architecture ensures that **your data is physically incapable of being tracked or scraped** by external servers.

## 🚀 Quick Install (Free 3-Month Trial)

1. [Download TabSyncBridge on the App Store](https://apps.apple.com/us/app/tabsyncbridge/id6766262129)
2. [Add the Chromium companion from the Chrome Web Store](https://chromewebstore.google.com/detail/tabsyncbridge/fbhngbfbapkkhcdpijagknchlcmcfmgl)
3. Follow the [Desktop bridge setup instructions](https://indexridge.github.io/TabSyncBridge/desktop-bridge-setup) to link your devices over Wi-Fi.

## 📖 Learn More

- [Marketing page](https://indexridge.github.io/TabSyncBridge/marketing)
- [Sync tabs without a cloud account](https://indexridge.github.io/TabSyncBridge/sync-tabs-without-cloud)
- [Why browser tab sync usually uses cloud accounts](https://indexridge.github.io/TabSyncBridge/why-browser-tab-sync-uses-cloud)
- [Safari and Chromium tab sync](https://indexridge.github.io/TabSyncBridge/safari-chrome-tab-sync)
- [Close remote tabs](https://indexridge.github.io/TabSyncBridge/close-remote-tabs)
- [Privacy Policy](https://indexridge.github.io/TabSyncBridge/privacy) | [Terms of Use](https://indexridge.github.io/TabSyncBridge/terms) | [Support](https://indexridge.github.io/TabSyncBridge/support)

*TabSyncBridge is £2.99 per month after a 3-month free trial. Purchases, renewals, cancellations, refunds, and restore purchases are handled by Apple through the App Store.*
