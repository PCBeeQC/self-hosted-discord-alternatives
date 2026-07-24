# 💬 Self-Hosted Discord Alternatives

A comprehensive comparison of the best **self-hosted Discord alternatives**, open-source chat platforms, and private team communication tools. 

This list tries to capture and summarize the features that matter when trying to self-host a chat platform. From my experience, what makes or breaks a self-hosted chat platform is how easy it is to use for the average user. Are there mobile apps they can download? Do push notifications work? Can they send GIFs in the chat (looking at you, Element on iOS)?

This list tries to answer some of these questions.

## ℹ️ A note on bias

This list is created and maintained by the creator of Spokes (which is why I put Spokes at the top). Apart from that, I want the list to be as accurate as possible. If you know of a serious self-hosted alternative that isn't listed here, or if you spot an inaccuracy, please open a pull request or issue. I will do my best to fix it as quickly as possible.

## ⚖️ Comparison

| Name | Project Type | Free / Paid | Ease of Setup | Desktop | Android | iOS | Voice & Video | SSO | Push Notifs | Encryption | Target Scale | Monetization |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| <img src="https://github.com/PCBeeQC.png?size=48" width="24" height="24" alt="Spokes logo" /> **[Spokes](https://spokes.sh/)** | Indie | Paid (2 Months Free Trial) | 🟢 | Web, PWA | ✅ | 🚧 | ✅ | ✅ | Encrypted | At-Rest | Small / Teams | Flat server fee |
| <img src="https://github.com/mattermost.png?size=48" width="24" height="24" alt="Mattermost logo" /> **[Mattermost](https://mattermost.com/)** | Enterprise SaaS | Freemium | 🟡 | App, Web | ✅ | ✅ | 🟡 (free 40m limit) | Paid | Relay | At-Rest | Enterprise (Paid) / Teams (Free) | Per user fee ($10/mo) |
| <img src="https://github.com/RocketChat.png?size=48" width="24" height="24" alt="Rocket.Chat logo" /> **[Rocket.Chat](https://rocket.chat/)** | Enterprise SaaS | Freemium | 🟡 | App, Web | ✅ | ✅ | 🟡 | ✅ | Relay (10k limit) | E2E | Enterprise | Per user fee ($7/mo) |
| <img src="https://github.com/element-hq.png?size=48" width="24" height="24" alt="Element logo" /> **[Matrix (Element)](https://matrix.org/)** | Protocol / Foundation | Free | 🔴 | App, Web | ✅ | ✅ | 🟡 | ✅ | Encrypted | E2E | Massive / Any | Free to use |
| <img src="https://github.com/zulip.png?size=48" width="24" height="24" alt="Zulip logo" /> **[Zulip](https://zulip.com/)** | Open-Source | Free | 🔴 | App, Web | ✅ | ✅ | 🟡 | ✅ | Paid Relay | ❌ | Enterprise / Any | Per user fee (Support/Relay) |
| <img src="https://github.com/nextcloud.png?size=48" width="24" height="24" alt="Nextcloud logo" /> **[Nextcloud Talk](https://nextcloud.com/talk/)** | Open-Source | Free | 🟡 | App, Web | ✅ | ✅ | 🟡 | ✅ | Relay | E2E | Any | Free to use |
| <img src="https://github.com/stoatchat.png?size=48" width="24" height="24" alt="Stoat logo" /> **[Stoat](https://stoat.chat/)** | Open-Source | Free | 🔴 | App, Web, PWA | 🚧 | 🚧 | 🟡 | ❌ | ❌ (Not for self-hosted servers) | ❌ | Communities | Discord nitro model |
| <img src="https://github.com/spacebarchat.png?size=48" width="24" height="24" alt="Spacebar logo" /> **[Spacebar](https://spacebar.chat/)** | Open-Source | Free | 🔴 | App, Web | 🚧 | 🚧 | 🚧 | ❌ | ❌ | ❌ | Communities | Free to use |
| <img src="https://github.com/chattocorp.png?size=48" width="24" height="24" alt="Chatto logo" /> **[Chatto](https://chatto.run/)** | Open-Source | Free | 🟢 | Web | ❌ | ❌ | ✅ | ✅ | Web Push | At-Rest | Communities | Cloud hosting |
| <img src="https://github.com/fluxerapp.png?size=48" width="24" height="24" alt="Fluxer logo" /> **[Fluxer](https://fluxer.app/)** | Open-Source | Free | 🟡 | App, Web | 🚧 | 🚧 | 🟡 | ✅ | UnifiedPush / Web Push | ❌ | Communities | Discord nitro model |
| <img src="https://github.com/Sharkord.png?size=48" width="24" height="24" alt="Sharkord logo" /> **[Sharkord](https://github.com/Sharkord/sharkord)** | Open-Source | Free | 🟢 | Web | 🚧 | ❌ | ✅ | ❌ | ❌ | ❌ | Small / Teams | Free to use |

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
  * **Free to use:** 100% community-driven or non-profit with no paid tiers.
  * **Discord nitro model:** Core server is free; premium features sold directly to users (B2C).
  * **Cloud hosting:** Self-hosted is free; they make money selling managed cloud hosting.
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

### 💭 My personal insights on choosing the right platform

If you're feeling overwhelmed by the list, here are some personal perspectives from my own journey of trying to move away from Discord and Slack. I haven't tried or daily-driven every single platform on this list, but I have tried a few, and here are my conclusions.

I have two separate use cases for a self-hosted chat platform: personal and work. Let's start with personal.

#### Friends and family use case
My friend group has been using Discord since 2015. We use it to chat, coordinate events, share pictures, etc. It has always worked great. The only issue is that everyone in my friend group, myself included, recently started having kids, and we want to preserve our children's privacy as much as possible. Discord simply isn't the right place for that.

I don't need the Discord replacement to be a Discord clone, but I do have some requirements.

**As the sysadmin:**
- It must support SSO. I don't want to manage individual accounts for every single service we self-host.
- I want the simplest possible install. The simpler the installation, the less chance that some part of the setup breaks in the future.

**For the users:** (I want to reduce friction as much as possible. Not everyone cares about tech; they just want a good experience.)
- Must have working iOS and Android apps.
- Must have reliable notifications.
- Group channels and private messages.
- Good built-in GIF support.
- Picture and video sharing.

Around a year and a half ago, we went through all the options, tried a bunch, and decided that Matrix/Element was the best fit for us. It works well, but it's not really comparable to the Discord server experience. I don't exactly know how to describe it, but the apps feel "clunky". We recently switched to Spokes (mostly because I'm the creator of Spokes).

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
