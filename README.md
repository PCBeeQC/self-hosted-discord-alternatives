# 💬 Self-Hosted Discord Alternatives

A comprehensive comparison of the best **self-hosted Discord alternatives**, open-source chat platforms, and private team communication tools. 

This list tries to capture and summarize the features that matter when trying to self-host a chat platform. From my experience, what makes or breaks a self-hosted chat platform is how easy it is to use for the average user. Is there mobile apps they can download? Do push notifications work? Can they send GIFs in the chat (looking at you Element on iOS)? 

This list tries to answer some of these questions.

## ℹ️ A note on bias

This list is created and maintained by the creator of Spokes (which is why I put Spokes at the top). Apart from that, I want the list to be as accurate as possible. If you know of a serious self-hosted alternative that isn't listed here, or if you spot an inaccuracy, please open a pull request or issue. I will do my best to fix it as quickly as possible.

## ⚖️ Comparison

| Name | Project Type | Free / Paid | Ease of Setup | Desktop | Android | iOS | Voice & Video | SSO | Push Notifs | Encryption | Target Scale | Monetization |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| <img src="https://github.com/PCBeeQC.png?size=48" width="24" height="24" alt="Spokes logo" /> **[Spokes](https://spokes.app/)** | Indie | Paid (2 Month Free Trial) | 🟢 | Web, PWA | ✅ | 🚧 | ✅ | ✅ | Encrypted | At-Rest | Small / Teams | Flat server fee |
| <img src="https://github.com/mattermost.png?size=48" width="24" height="24" alt="Mattermost logo" /> **[Mattermost](https://mattermost.com/)** | Enterprise SaaS | Freemium | 🟡 | App, Web | ✅ | ✅ | 🟡 (free 40m limit) | Paid | Relay | At-Rest | Enterprise (Paid) / Teams (Free) | Per user fee |
| <img src="https://github.com/RocketChat.png?size=48" width="24" height="24" alt="Rocket.Chat logo" /> **[Rocket.Chat](https://rocket.chat/)** | Enterprise SaaS | Freemium | 🟡 | App, Web | ✅ | ✅ | 🟡 | ✅ | Relay (10k limit) | E2E | Enterprise | Per user fee |
| <img src="https://github.com/element-hq.png?size=48" width="24" height="24" alt="Element logo" /> **[Matrix (Element)](https://element.io/)** | Protocol / Foundation | Free | 🔴 | App, Web | ✅ | ✅ | 🟡 | ✅ | Encrypted | E2E | Massive / Any | It does not |
| <img src="https://github.com/zulip.png?size=48" width="24" height="24" alt="Zulip logo" /> **[Zulip](https://zulip.com/)** | Open-Source | Free | 🔴 | App, Web | ✅ | ✅ | 🟡 | ✅ | Paid Relay | ❌ | Enterprise / Any | It does not |
| <img src="https://github.com/nextcloud.png?size=48" width="24" height="24" alt="Nextcloud logo" /> **[Nextcloud Talk](https://nextcloud.com/talk/)** | Open-Source | Free | 🟡 | App, Web | ✅ | ✅ | 🟡 | ✅ | Relay | E2E | Any | It does not |
| <img src="https://github.com/stoatchat.png?size=48" width="24" height="24" alt="Stoat logo" /> **[Stoat](https://stoat.chat/)** | Open-Source | Free | 🔴 | App, Web, PWA | 🚧 | 🚧 | 🟡 | ❌ | ❌ (Not for self-hosted servers) | ❌ | Communities | It does not |
| <img src="https://github.com/spacebarchat.png?size=48" width="24" height="24" alt="Spacebar logo" /> **[Spacebar](https://spacebar.chat/)** | Open-Source | Free | 🔴 | App, Web | 🚧 | 🚧 | 🚧 | ❌ | ❌ | ❌ | Communities | It does not |
| <img src="https://github.com/chattocorp.png?size=48" width="24" height="24" alt="Chatto logo" /> **[Chatto](https://chatto.run/)** | Open-Source | Free | 🟢 | Web | ❌ | ❌ | ✅ | ✅ | Web Push | At-Rest | Communities | It does not |
| <img src="https://github.com/fluxerapp.png?size=48" width="24" height="24" alt="Fluxer logo" /> **[Fluxer](https://fluxer.app/)** | Open-Source | Free | 🟡 | App, Web | 🚧 | 🚧 | 🟡 | ✅ | UnifiedPush / Web Push | ❌ | Communities | It does not |
| <img src="https://github.com/Sharkord.png?size=48" width="24" height="24" alt="Sharkord logo" /> **[Sharkord](https://github.com/Sharkord/sharkord)** | Open-Source | Free | 🟢 | Web | 🚧 | ❌ | ✅ | ❌ | ❌ | ❌ | Small / Teams | It does not |

### 📖 Evaluation Criteria (Legend)

To ensure this list remains objective and verifiable, we use the following criteria to evaluate each platform:

#### General & Business Model
* **Project Type:** 
  * **Enterprise SaaS:** A commercial product built primarily as a hosted SaaS offering, with self-hosting provided as an alternative deployment method. Often features heavily restricted "Freemium" models for self-hosters.
  * **Protocol / Foundation:** A standard or foundation-backed project (e.g., Matrix).
  * **Open-Source:** A community-driven project built first-and-foremost for self-hosting.
  * **Indie:** An independently developed commercial product.
* **Free / Paid:** 
  * **Free:** 100% free and open-source software with no paid tiers.
  * **Freemium:** Core software is free, but enterprise or advanced features require a paid license.
  * **Paid / Licensing:** Software requires a commercial license. *(e.g., Spokes offers a fully unlocked 2-month free trial. After the trial, the software remains free to use forever, but receiving future updates requires an active license).*
* **Monetization:** How the app developer makes money from self-hosters.
  * **It does not:** 100% community-driven or non-profit with no paid tiers.
  * **Flat server fee:** You pay a single flat price per server/instance, regardless of user count.
  * **Per user fee:** The cost scales with the number of users on your server.
* **Target Scale:** 
  * **Small / Teams:** Optimized for performance and simplicity for groups up to ~100 users.
  * **Communities:** Built to handle medium-to-large communities (~1,000+ users).
  * **Enterprise / Massive:** Highly scalable architecture designed for massive servers or enterprise deployments (10,000+ users).

#### Deployment & Access
* **Ease of Setup:**
  * 🟢 **Easy:** Single Docker container, minimal network configuration required.
  * 🟡 **Medium:** Multiple containers (e.g., separate database), requires inter-container network config.
  * 🔴 **Hard:** Multiple containers, advanced network configuration, complex scaling setup.
* **Desktop:** Accessible via a WebUI (any browser), a Progressive Web App (PWA), or a native Desktop App.
* **Android:** Available in the Google Play Store (✅), available as an APK download only (🚧), or none (❌).
* **iOS:** Available in the Apple App Store (✅), or none (❌).

#### Features
* **Voice & Video:** 
  * ✅ **Built-in:** Works out of the box with no extra software.
  * 🟡 **Requires Extra Config / Plugin:** Supported, but requires running additional services (like Jitsi or LiveKit) separately.
  * ❌ **Not Supported.**
* **SSO (Single Sign-On):** Supports using an external identity provider (OIDC, SAML, etc.) for user authentication.
* **Push Notifications:** 
  * **Web:** Uses standard web push (VAPID).
  * **Relay:** Uses a centralized relay server to push notifications to mobile devices.
  * **Paid Relay:** Uses a centralized relay server, but requires a paid subscription to utilize it.
  * **Encrypted:** Payloads are End-to-End Encrypted before going through the relay, protecting data from Apple/Google.
  * ❌ **Not Supported.**
* **Encryption:** 
  * **At-Rest:** Channel data is encrypted in the database to protect against server/backup compromise.
  * **E2E:** Messages are end-to-end encrypted on the client device and cannot be read by the server at all.
  * ❌ **Not Supported:** Standard plaintext database storage.

---

