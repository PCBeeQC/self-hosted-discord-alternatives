# 💬 Self-Hosted Discord Alternatives

A comparison of the best **self-hosted Discord alternatives**, open-source chat platforms, and private team communication tools. 

When evaluating a self-hosted replacement for Discord, most comparisons only look at desktop text channel screenshots. In real-world deployments, what makes or breaks a self-hosted chat server for friends, gaming communities, families, and small teams comes down to four practical requirements:
1. **Ease of Hosting & Maintenance:** Does it run in a **single Docker container**, or does it require orchestrating 5–10 separate containers (PostgreSQL/MongoDB, Redis, Coturn TURN, and a standalone WebRTC media server)?
2. **Voice & Video Channels:** Are persistent, drop-in voice rooms, video calls, and screen sharing **built directly into the server** out of the box, or do they require stitching together external Jitsi/LiveKit bridges?
3. **Official Mobile Apps:** Can non-technical users download polished, official apps directly from the **Apple App Store (iOS)** and **Google Play Store (Android)** without sideloading APKs or joining expired TestFlight betas?
4. **Working Push Notifications:** Do mobile push notifications work reliably when phones are locked, and can users send media and GIFs effortlessly?

This list tries to answer some of these questions. If you know of a serious self-hosted alternative that isn't listed here, or if you spot an inaccuracy, please open a pull request or issue. I will do my best to fix it as quickly as possible.

## ⚖️ Comparison

| Name | Project Type | Free / Paid | Ease of Setup | Desktop | Android | iOS | Voice & Video | SSO | Push Notifs | Encryption | Target Scale | Monetization |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| <img src="https://spokes.sh/logo.png" width="24" height="24" alt="Spokes logo" /> **[Spokes](https://spokes.sh/)** | Indie | Freemium | 🟢 | App, Web, PWA | ✅ | ✅ | ✅ | ✅ | Web Push / Paid Relay / Encrypted | At-Rest | Small / Teams | Flat server pass ($45/yr) |
| <img src="https://github.com/mattermost.png?size=48" width="24" height="24" alt="Mattermost logo" /> **[Mattermost](https://mattermost.com/)** | Enterprise SaaS | Freemium | 🟡 | App, Web, PWA | ✅ | ✅ | 🟡 (free 1:1 & 40m limit) | Paid | Paid Relay (Free 10k/Test limit) | ❌ | Enterprise (Paid) / Teams (Free) | Per user fee ($10/mo) |
| <img src="https://github.com/RocketChat.png?size=48" width="24" height="24" alt="Rocket.Chat logo" /> **[Rocket.Chat](https://rocket.chat/)** | Enterprise SaaS | Freemium | 🟡 | App, Web, PWA | ✅ | ✅ | 🟡 | Paid | Relay (10k limit) | E2E | Enterprise (Paid) / Small (Free) | Per user fee ($8+/mo) |
| <img src="https://github.com/element-hq.png?size=48" width="24" height="24" alt="Element logo" /> **[Matrix (Element)](https://matrix.org/)** | Protocol / Foundation | Free | 🔴 | App, Web, PWA | ✅ | ✅ | 🟡 | ✅ | Relay / Encrypted | E2E | Massive / Any | Free to use |
| <img src="https://github.com/zulip.png?size=48" width="24" height="24" alt="Zulip logo" /> **[Zulip](https://zulip.com/)** | Open-Source | Freemium | 🟡 | App, Web | ✅ | ✅ | 🟡 | ✅ | Paid Relay / Encrypted (Free ≤10 users) | ❌ | Enterprise / Any | Per user fee ($3.50/mo Relay) |
| <img src="https://github.com/nextcloud.png?size=48" width="24" height="24" alt="Nextcloud logo" /> **[Nextcloud Talk](https://nextcloud.com/talk/)** | Open-Source | Free | 🟡 | App, Web | ✅ | ✅ | 🟡 | ✅ | Relay / Encrypted | ❌ | Any | Free to use |
| <img src="https://github.com/stoatchat.png?size=48" width="24" height="24" alt="Stoat logo" /> **[Stoat](https://stoat.chat/)** | Open-Source | Free | 🔴 | App, Web, PWA | ✅ | 🚧 | 🟡 | ❌ | Web Push | ❌ | Communities | Free to use |
| <img src="https://github.com/spacebarchat.png?size=48" width="24" height="24" alt="Spacebar logo" /> **[Spacebar](https://spacebar.chat/)** | Open-Source | Free | 🔴 | App, Web | 🚧 | ❌ | 🟡 | ❌ | ❌ | ❌ | Communities | Free to use |
| <img src="https://github.com/chattocorp.png?size=48" width="24" height="24" alt="Chatto logo" /> **[Chatto](https://chatto.run/)** | Open-Source | Free | 🟡 | Web, PWA | ❌ | ❌ | 🟡 | ✅ | Web Push | At-Rest | Communities | Cloud hosting |
| <img src="https://github.com/fluxerapp.png?size=48" width="24" height="24" alt="Fluxer logo" /> **[Fluxer](https://fluxer.app/)** | Open-Source | Free | 🟡 | App, Web, PWA | ✅ | 🚧 | 🟡 | ✅ | Relay / Encrypted / UnifiedPush / Web Push | ❌ | Communities | Supporter pass ($199) |
| <img src="https://github.com/Sharkord.png?size=48" width="24" height="24" alt="Sharkord logo" /> **[Sharkord](https://github.com/Sharkord/sharkord)** | Open-Source | Free | 🟢 | Web | ❌ | ❌ | ✅ | ✅ | ❌ | ❌ | Small / Teams | Free to use |

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
  * **Freemium:** Core software is free to self-host, but advanced/hosted services (such as push notification relays) or enterprise features require a paid license.
  * **Paid / Licensing:** Software requires a mandatory commercial license.
* **Monetization:** How the app developer makes money from self-hosters.
  * **Free to use:** 100% community-driven or non-profit with no paid tiers.
  * **Supporter pass / Donations:** Self-hosted is 100% free with all features; funded by optional supporter passes (e.g., Operator Pass) or donations.
  * **Cloud hosting:** Self-hosted is free; they make money selling managed cloud hosting.
  * **Flat server pass:** You pay a single flat price per server/instance, regardless of user count.
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
* **iOS:** Available in the Apple App Store (✅), available on TestFlight (🚧), or none (❌).

#### Features
* **Voice & Video:** 
  * ✅ **Built-in:** Works out of the box with no extra software.
  * 🟡 **Requires Extra Config / Plugin:** Supported, but requires running additional services (like Jitsi or LiveKit) separately.
  * ❌ **Not Supported.**
* **SSO (Single Sign-On):** Supports using an external identity provider (OIDC, SAML, etc.) for user authentication.
* **Push Notifications:** 
  * **Web Push:** Uses standard web push (VAPID).
  * **UnifiedPush:** Uses the open UnifiedPush standard on Android.
  * **Relay:** Uses a centralized relay server to push notifications to mobile devices.
  * **Paid Relay:** Uses a centralized relay server, but requires a paid subscription to utilize it.
  * **Encrypted:** Payloads are End-to-End Encrypted before going through the relay, protecting data from Apple/Google.
  * ❌ **Not Supported.**
* **Encryption:** 
  * **At-Rest:** Channel data is encrypted in the database to protect against server/backup compromise.
  * **E2E:** Messages are end-to-end encrypted on the client device and cannot be read by the server at all.
  * ❌ **Not Supported:** Standard plaintext database storage.

---

### 🔍 Platform Summaries

* **[Spokes](https://spokes.sh/):** Built for small groups, families, and teams. Deploys as a single Docker container with no external database required. Includes built-in Discord-style voice and video channels, SSO, and official iOS (App Store) and Android (Google Play) apps with encrypted push notifications (free Web Push; 2-month free trial of native mobile push, then $45/yr flat per-server pass).
* **[Mattermost](https://mattermost.com/):** Slack-style workplace chat. Deploys via Docker Compose with PostgreSQL. Official iOS and Android apps are available, though the free tier limits push notifications (10k/month), group calls (1:1 and 40-minute limit), and SSO unless on a per-user paid plan ($10/user/mo).
* **[Rocket.Chat](https://rocket.chat/):** Enterprise Slack-style workspace. Deploys via Docker Compose with MongoDB. Official iOS and Android apps are available; voice/video requires extra Jitsi/LiveKit setup, and free self-hosted servers have a 10k/month push notification cap ($8+/user/mo for paid tiers).
* **[Matrix (Element)](https://matrix.org/):** Decentralized, federated protocol with end-to-end encryption and official iOS and Android apps (with free push notifications). Self-hosting a homeserver with working voice and video channels requires a multi-container stack (Synapse, PostgreSQL, TURN, and a separate LiveKit or Jitsi service).
* **[Zulip](https://zulip.com/):** Open-source chat organized around topic-threaded streams. Deploys as a multi-container Docker stack with official iOS and Android apps. Calls rely on external Jitsi/Zoom integrations rather than persistent voice rooms, and mobile push notifications require a paid plan ($3.50/user/mo) above 10 users.
* **[Nextcloud Talk](https://nextcloud.com/talk/):** Communication module for Nextcloud with official iOS and Android apps and working push notifications. Group voice and video calls beyond a few users require deploying and configuring a separate High-Performance Backend (HPB) and TURN server.
* **[Stoat](https://stoat.chat/) (formerly Revolt):** Open-source Discord clone. Self-hosting requires a multi-container stack (MongoDB, Redis, RabbitMQ, MinIO, Vortex). Android is available, iOS is on TestFlight, and self-hosted instances only support Web Push out of the box (native mobile push keys are tied to the official hosted instance).
* **[Spacebar](https://spacebar.chat/):** Open-source project aiming for Discord API compatibility. Requires a multi-container setup, mobile clients are still in early development (no iOS App Store app or working self-hosted mobile push notifications), and voice/video requires extra setup.
* **[Chatto](https://chatto.run/):** Open-source community chat with Web and PWA support, Web Push notifications, and SSO. Requires extra setup for voice/video and does not currently have native iOS or Android store apps.
* **[Fluxer](https://fluxer.app/):** Open-source Discord clone supporting SSO, Android, and iOS (TestFlight) with UnifiedPush and encrypted push relay support. Deploys as a multi-container stack, requires extra configuration for self-hosted voice and video, and is funded by an optional one-time Operator Pass ($199) that does not restrict self-hosted features.
* **[Sharkord](https://github.com/Sharkord/sharkord):** Lightweight open-source Discord alternative that runs in a single container with built-in voice and video channels. Accessible via web browser only, with no native iOS or Android mobile apps and no push notifications.

---

### 💭 My personal insights on choosing the right platform

If you're feeling overwhelmed by the list, here are some personal perspectives from my own journey of trying to move away from Discord and Slack. I haven't tried or daily-driven every single platform on this list, but I have tried a few, and here are my conclusions.

I have two separate use cases for a self-hosted chat platform: personal and work. Let's start with personal.

#### Friends and family use case
My friend group has been using Discord since 2015. We use it to chat, coordinate events, share pictures, etc. It has always worked great. The only issue is that everyone in my friend group, myself included, recently started having kids, and we want to preserve our children's privacy as much as possible. Discord simply isn't the right place for that.

I don't need the Discord replacement to be a Discord clone, but I do have some requirements.

**As the sysadmin:**
- It must support SSO. I don't want to manage individual accounts for every single service we self-host.
- I want the simplest possible install. The simpler the installation, the less chance that some part of the setup breaks in the future.

**For the users:** (The goal is to reduce friction as much as possible. Not everyone cares about tech. They just want a good experience.)
- Must have working iOS and Android apps.
- Must have reliable notifications.
- Group channels and private messages.
- Good built-in GIF support.
- Picture and video sharing.

(The requirements above are my own. You need to figure out your own requirements.)

Around a year and a half ago, we went through all the options, tried a bunch, and decided that Matrix/Element was the best fit for us. It works well, but it's not really comparable to the Discord server experience. I don't exactly know how to describe it, but the apps feel "clunky". I eventually ended up building Spokes to get the exact setup we wanted, and we have been using it since.

#### Small business use case
I work at a small 10-employee business where, among other roles, I manage IT. Around 3 years ago, we started needing a chat platform.

We didn't have any hard-to-meet requirements:
- A locally self-hosted solution. To avoid per-user fees and to have blazing-fast upload and download speeds for quick file sharing.
- Good support for channels, channel categories, permissions, etc.
- SSO support.
- A good desktop client.

We settled on Mattermost and have been really happy with it for the most part. However, the Mattermost team recently started removing features from the free tier, so your mileage may vary.

#### In conclusion
A chat platform is only useful if people use it. Think about your group and use case: what features are required for adoption, and what features are nice to have?
