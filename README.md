# 💬 Self-Hosted Discord Alternatives

A practical comparison of **self-hosted Discord alternatives**, open-source chat platforms, and private group communication tools.

This comparison focuses strictly on the **self-hosted version** of each platform (some projects offer different features or push notification behavior on their hosted cloud plans).

Every self-hosted chat platform makes trade-offs. Depending on your group, you may prioritize an open-source license, full end-to-end encryption and federation, Discord bot compatibility, a lightweight Docker setup, built-in voice and video, or official iOS and Android apps with working push notifications. The table below compares each option across those areas, along with how each project is licensed and funded.

> **Disclosure:** I am the developer of [Spokes](https://spokes.sh/). My goal here is to keep an accurate, up-to-date list of serious self-hosted Discord alternatives. If a project is missing or any detail is outdated, please open an issue or pull request and I will update it quickly.

## ⚖️ Comparison (Alphabetical)

| Name | License | Project Type | Ease of Setup | Desktop | Android | iOS | Voice & Video | SSO | Self-Hosted Push Notifs | Encryption | Target Scale | Monetization |
| :--- | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :--- | :---: | :---: | :--- |
| <img src="https://github.com/chattocorp.png?size=48" width="24" height="24" alt="Chatto logo" /> **[Chatto](https://chatto.run/)** | Open-Source | Open-Source | 🟡 | Web, PWA | ❌ | ❌ | 🟡 | ✅ | Web Push | At-Rest | Communities | Cloud hosting |
| <img src="https://github.com/fluxerapp.png?size=48" width="24" height="24" alt="Fluxer logo" /> **[Fluxer](https://fluxer.app/)** | Open-Source (AGPLv3) | Open-Source | 🟡 | App, Web, PWA | ✅ | 🚧 | 🟡 | ✅ | Encrypted Relay / UnifiedPush / Web Push | ❌ | Communities | Supporter pass ($199) |
| <img src="https://github.com/element-hq.png?size=48" width="24" height="24" alt="Element logo" /> **[Matrix (Element)](https://matrix.org/)** | Open-Source (AGPLv3 / Apache 2.0) | Protocol / Foundation | 🔴 | App, Web, PWA | ✅ | ✅ | 🟡 | ✅ | Free Relay / UnifiedPush (Encrypted) | E2E | Massive / Any | Free to use |
| <img src="https://github.com/mattermost.png?size=48" width="24" height="24" alt="Mattermost logo" /> **[Mattermost](https://mattermost.com/)** | Open-Core (MIT / Commercial) | Enterprise SaaS | 🟡 | App, Web, PWA | ✅ | ✅ | 🟡 (free 1:1 & 40m limit) | Paid | Relay (10k/mo free cap) | ❌ | Enterprise (Paid) / Teams (Free) | Per user fee ($10/mo) |
| <img src="https://github.com/nextcloud.png?size=48" width="24" height="24" alt="Nextcloud logo" /> **[Nextcloud Talk](https://nextcloud.com/talk/)** | Open-Source (AGPLv3) | Open-Source | 🟡 | App, Web | ✅ | ✅ | 🟡 | ✅ | Free Relay / Encrypted | ❌ | Any | Free to use |
| <img src="https://github.com/RocketChat.png?size=48" width="24" height="24" alt="Rocket.Chat logo" /> **[Rocket.Chat](https://rocket.chat/)** | Open-Core (MIT / Commercial) | Enterprise SaaS | 🟡 | App, Web, PWA | ✅ | ✅ | 🟡 | ✅ | Relay (10k/mo free cap) | E2E (opt.) | Enterprise (Paid) / Small (Free) | Per user fee ($7+/mo) |
| <img src="https://github.com/Sharkord.png?size=48" width="24" height="24" alt="Sharkord logo" /> **[Sharkord](https://github.com/Sharkord/sharkord)** | Open-Source (MIT) | Open-Source | 🟢 | Web | ❌ | ❌ | ✅ | ✅ | ❌ | ❌ | Small / Teams | Free to use |
| <img src="https://github.com/spacebarchat.png?size=48" width="24" height="24" alt="Spacebar logo" /> **[Spacebar](https://spacebar.chat/)** | Open-Source (AGPLv3) | Open-Source | 🔴 | App, Web | 🚧 | ❌ | 🟡 | ❌ | ❌ | ❌ | Communities | Free to use |
| <img src="https://spokes.sh/logo.png" width="24" height="24" alt="Spokes logo" /> **[Spokes](https://spokes.sh/)** | Source-Available (BSL 1.1 -> Apache 2.0) | Indie | 🟢 | App, Web, PWA | ✅ | ✅ | ✅ | ✅ | Encrypted Native Relay (2-mo trial; $45/yr flat/server) + Free Web Push | At-Rest (Vaults) | Small / Teams | Free server; optional $45/yr flat push pass |
| <img src="https://github.com/stoatchat.png?size=48" width="24" height="24" alt="Stoat logo" /> **[Stoat](https://stoat.chat/)** | Open-Source (AGPLv3) | Open-Source | 🔴 | App, Web, PWA | 🚧 | 🚧 | 🟡 | ❌ | Web Push only when self-hosted | ❌ | Communities | Free to use |
| <img src="https://github.com/zulip.png?size=48" width="24" height="24" alt="Zulip logo" /> **[Zulip](https://zulip.com/)** | Open-Source (Apache 2.0) | Open-Source | 🔴 | App, Web | ✅ | ✅ | 🟡 | ✅ | Encrypted Relay (Free ≤10 users; $3.50/user/mo above) | ❌ | Enterprise / Any | Per user fee ($3.50/mo Relay) |

### 📖 Evaluation Criteria (Legend)

To keep this list objective and verifiable, each platform is evaluated using these criteria:

#### General & Business Model
* **License:**
  * **Open-Source:** Released under an OSI-approved license (such as AGPLv3, Apache 2.0, or MIT).
  * **Open-Core:** Core server is open-source, while commercial or enterprise features are under a separate paid license.
  * **Source-Available:** Full source code is public on GitHub, with a time-limited commercial restriction (for example, BSL 1.1 converting automatically to Apache 2.0 after four years).
* **Project Type:**
  * **Enterprise SaaS:** A commercial product built primarily as a hosted SaaS offering, with self-hosting provided as an alternative deployment method. Often features restricted free tiers for self-hosters.
  * **Protocol / Foundation:** A standard or foundation-backed project (e.g., Matrix).
  * **Open-Source:** A community-driven project built primarily for open-source deployment.
  * **Indie:** An independently developed self-hosted product.
* **Monetization:** How the developer funds ongoing development and hosted infrastructure (such as mobile push relays):
  * **Free to use:** Community-driven or non-profit with no paid tiers.
  * **Supporter pass / Donations:** Self-hosted is free with all features; funded by optional supporter passes (e.g., Operator Pass) or donations.
  * **Cloud hosting:** Self-hosted is free; revenue comes from managed cloud hosting.
  * **Flat server pass:** A single flat price per server/instance covering unlimited users, with no per-user fees.
  * **Per user fee:** Cost scales with the number of users on your server.
* **Target Scale:**
  * **Small / Teams:** Optimized for simplicity and low maintenance for private groups up to ~100 users.
  * **Communities:** Built to handle medium-to-large communities (~1,000+ users).
  * **Enterprise / Massive:** Multi-service architecture designed for massive servers or enterprise deployments (10,000+ users).

#### Deployment & Access
* **Ease of Setup:**
  * 🟢 **Easy:** Single Docker container, no external database required, minimal network configuration.
  * 🟡 **Medium:** Multi-container Compose stack (separate database, cache, or media services).
  * 🔴 **Hard:** Complex multi-service stack (6 to 8+ containers) with advanced reverse-proxy or media routing config.
* **Desktop:** Accessible via a WebUI (any browser), a Progressive Web App (PWA), or a native Desktop App.
* **Android:** Live production app in the Google Play Store (✅), beta or APK-only (🚧), or none (❌).
* **iOS:** Live production app in the Apple App Store (✅), TestFlight beta only (🚧), or none (❌).

#### Features
* **Voice & Video:**
  * ✅ **Built-in:** Persistent drop-in voice and video channels work out of the box inside the same container/binary.
  * 🟡 **Requires Extra Config / Separate Service:** Supported, but requires deploying and configuring separate services (such as LiveKit, Jitsi, TURN, or an HPB) or has free-tier call limits.
  * ❌ **Not Supported.**
* **SSO (Single Sign-On):** Supports using an external identity provider (OIDC, SAML, etc.) for user authentication.
* **Self-Hosted Push Notifications:**
  * **Web Push:** Uses standard browser Web Push (VAPID).
  * **UnifiedPush:** Uses the open UnifiedPush standard on Android.
  * **Relay:** Uses a hosted relay server to deliver APNs/FCM push notifications to official App Store and Google Play apps.
  * **Encrypted:** Notification payloads are end-to-end encrypted by your server before transiting the relay, so Apple, Google, and the relay cannot read them.
  * ❌ **Not Supported.**
* **Encryption:**
  * **At-Rest (Vaults):** Sensitive channels and data can be encrypted on disk to protect against backup or database leaks.
  * **E2E:** Messages are end-to-end encrypted on client devices and cannot be read by the server.
  * ❌ **Not Supported:** Standard plaintext database storage (with TLS in transit).

---

### 🔍 Platform Summaries (Alphabetical)

* **[Chatto](https://chatto.run/):** Open-source community chat with Web and PWA support, Web Push notifications, and SSO. Requires extra setup for voice/video and does not currently have native iOS or Android store apps.
* **[Fluxer](https://fluxer.app/):** AGPLv3 open-source Discord clone supporting OIDC SSO, Android (Google Play / GitHub APK), and iOS (TestFlight beta) with UnifiedPush and an opt-in encrypted push relay. Self-hosting runs a 7-container Compose stack (PostgreSQL, Valkey, NATS, Meilisearch, SeaweedFS, LiveKit, Caddy) automated via its `rexctl` installer, and is funded by donations and an optional supporter pass ($199) that does not restrict self-hosted features.
* **[Matrix (Element)](https://matrix.org/):** Decentralized, federated open-source protocol with end-to-end encryption and official iOS (App Store) and Android (Google Play) apps with free push notifications. Self-hosting a homeserver with working group voice and video channels requires a multi-container stack (Synapse or Conduit, PostgreSQL, TURN, and Element Call / LiveKit or Jitsi), and the interface feels like a room list rather than a unified Discord server.
* **[Mattermost](https://mattermost.com/):** Slack-style workplace chat. Deploys via Docker Compose with PostgreSQL. Official iOS and Android apps are available, though the free Entry tier limits push notifications (10k/month), group calls (1:1 and 40-minute limit), searchable history (10k messages), and OIDC SSO unless on a per-user paid plan ($10/user/mo).
* **[Nextcloud Talk](https://nextcloud.com/talk/):** Communication module for Nextcloud with official iOS and Android apps and working push notifications. Group voice and video calls beyond a few users require deploying and configuring a separate High-Performance Backend (HPB) and TURN server.
* **[Rocket.Chat](https://rocket.chat/):** Enterprise Slack-style workspace. Deploys via Docker Compose with MongoDB. Official iOS and Android apps are available; voice/video requires extra Jitsi/Pexip setup, and free self-hosted servers have a 10k/month push notification cap ($7+/user/mo for paid tiers).
* **[Sharkord](https://github.com/Sharkord/sharkord):** Lightweight MIT-licensed Discord alternative that runs in a single Docker container or binary with built-in WebRTC voice, video, screen sharing, and SSO. Accessible via web browser only, with no official App Store or Google Play mobile apps and no mobile push notifications.
* **[Spacebar](https://spacebar.chat/):** AGPLv3 open-source project aiming for Discord API compatibility so existing Discord bots and clients can connect. Requires a multi-container setup, voice/video requires extra setup, and mobile clients are still early (no iOS App Store app or working self-hosted mobile push notifications).
* **[Spokes](https://spokes.sh/):** Source-available ([GitHub](https://github.com/PCBeeQC/Spokes_Server), BSL 1.1) self-hosted Discord alternative built for private friend groups, gaming squads, families, and small teams. Deploys as a single Docker container (`ghcr.io/pcbeeqc/spokes:latest`) with no external database, embedded LiveKit drop-in voice/video/screen sharing, built-in Casdoor OIDC SSO, shared photo albums, and a group calendar. Ships official native apps on both the Apple App Store and Google Play Store plus desktop clients and Web/PWA, with free Web Push forever, a 2-month free trial of encrypted native mobile push, and an optional flat $45/yr per-server pass (unlimited users). Trade-offs: source-available, no cross-server federation or protocol-level room E2EE, and native mobile push requires the flat server pass after the 2-month trial.
* **[Stoat](https://stoat.chat/):** AGPLv3 open-source Discord clone built primarily for the `stoat.chat` cloud. Self-hosting requires an 8+ container stack (Rust API, Web, MongoDB, Redis/Valkey, RabbitMQ, MinIO, and LiveKit, which replaced its legacy Vortex voice backend). Android is in beta, iOS is on TestFlight, and self-hosted instances only support Web Push out of the box because native mobile push keys are tied to the official cloud.
* **[Zulip](https://zulip.com/):** Apache 2.0 open-source chat organized around topic-threaded streams. Deploys as a multi-container Docker stack (PostgreSQL, Redis, RabbitMQ) with official iOS and Android apps. Calls rely on external Jitsi/Zoom links rather than persistent voice rooms, and mobile push notifications require a paid plan ($3.50/user/mo) above 10 users (or approval for its non-commercial Community plan).

---

### 💭 Further Reading

- **[Self-Hosted Discord & Slack Alternatives Compared (spokes.sh/compare)](https://spokes.sh/compare/)**: Interactive criteria selector and side-by-side breakdown across 18 self-hosted requirements.
- **[What you actually need in a self-hosted Discord alternative (DEV Community)](https://dev.to/matsmd/what-you-actually-need-in-a-self-hosted-discord-alternative-matrix-vs-mattermost-vs-spokes-5fmj)**: Practical write-up on running self-hosted chat for real-life friend groups and small teams.
