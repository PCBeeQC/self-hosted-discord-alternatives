# 💬 Self-Hosted Discord Alternatives

A comparison of self-hosted alternatives to communication platforms like Discord.

The goal of this list is to include all self-hosted alternatives, not only the open source projects. 

## ℹ️ A note on bias

This list is created and maintained by the creator of Spokes (which is why I put Spokes at the top). Apart from that, I want the list to be as accurate as possible. If you know of a serious self-hosted alternative that isn't listed here, or if you spot an inaccuracy, please open a pull request or issue. I will do my best to fix it as quickly as possible.

## ⚖️ Comparison

| Name | Free / Paid | Ease of Setup | Desktop | Android | iOS | Voice & Video | SSO | Push Notifs | Encryption | Target Scale |
| :--- | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **[Spokes](https://spokes.app/)** | Paid / Licensing | 🟢 | App, Web | ✅ | 🚧 | ✅ | ✅ | Encrypted | At-Rest | Small / Teams |
| **[Mattermost](https://mattermost.com/)** | Freemium | 🟡 | App, Web | ✅ | ✅ | ✅ | Paid | Paid Relay | At-Rest | Enterprise |
| **[Rocket.Chat](https://rocket.chat/)** | Freemium | 🟡 | App, Web | ✅ | ✅ | ✅ | ✅ | Relay | E2E | Enterprise |
| **[Matrix (Element)](https://element.io/)** | Free | 🔴 | App, Web | ✅ | ✅ | 🟡 | ✅ | Relay | E2E | Massive / Any |
| **[Zulip](https://zulip.com/)** | Freemium | 🟡 | App, Web | ✅ | ✅ | 🟡 | ✅ | Paid Relay | ❌ | Enterprise / Any |
| **[Nextcloud Talk](https://nextcloud.com/talk/)** | Free | 🟡 | Web | ✅ | ✅ | ✅ | ✅ | Relay | E2E | Any |
| **[Stoat](https://stoat.chat/)** | Free | 🔴 | App, Web, PWA | 🚧 | 🚧 | 🟡 | ❌ | ❌ | ❌ | Communities |
| **[Spacebar](https://spacebar.chat/)** | Free | 🔴 | App, Web | 🚧 | 🚧 | 🚧 | ❌ | ❌ | ❌ | Communities |
| **[Chatto](https://chatto.run/)** | Free | 🟢 | Web | ❌ | ❌ | ✅ | ✅ | ❌ | At-Rest | Communities |
| **[Fluxer](https://fluxer.app/)** | Free | 🟡 | App, Web | 🚧 | 🚧 | 🟡 | ✅ | ❌ | ❌ | Communities |

### 📖 Evaluation Criteria (Legend)

To ensure this list remains objective and verifiable, we use the following criteria to evaluate each platform:

#### General & Business Model
* **Free / Paid:** 
  * **Free:** 100% free and open-source software with no paid tiers.
  * **Freemium:** Core software is free, but enterprise or advanced features require a paid license.
  * **Paid / Licensing:** Software requires a license. (e.g., Spokes: The software is free to use forever, but receiving updates requires an active license).
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
* **Push Notifs:** 
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

