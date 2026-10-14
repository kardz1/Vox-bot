# Privacy Policy

**Last Updated:** October 14, 2026

This Privacy Policy explains how our Discord bot ("the Bot", "we", "us", or "our") collects, uses, stores, and protects information when added to your Discord server or used by your server members. By using the Bot, you agree to the collection and use of information in accordance with this policy.

---

### 1. Information We Collect

To function properly, provide moderation tools, enforce security, and run utility features, the Bot processes and stores the following types of data:

* **Discord Identifiers:**
  * User IDs and usernames/tags.
  * Server (Guild) IDs.
  * Channel IDs and Role IDs.

* **Moderation Records:**
  * Infraction logs, warnings, mutes, kicks, bans, and temporary jail records.
  * Moderation case IDs, moderator tags/IDs, target tags/IDs, timestamps, and moderator-provided reasons.
  * Stored role snapshots for jailed or quarantined members to enable proper restoration upon release.
  * Persistent role assignments, jail/ban request records, and ban appeal records.

* **Staff Activity & Management Data:**
  * Message counts bucketed by time (daily, weekly, monthly, all-time) and moderation case counts to track weekly staff quota progress.
  * Staff promotion/demotion history and Leave of Absence (LOA) records (durations, status, approval metadata).
  * Internal staff review scores and feedback comments.
  * Staff infraction records and their approval requests.

* **Community Features Data:**
  * Vouch and scam-vouch reports (reporter and target IDs, comments, and cooldown timestamps).
  * Staff application submissions and related cooldowns.
  * Help desk tickets (asker ID, question text, claim status, and the helper who handled it).
  * AFK status (reason and time set), and a temporary list of who pinged an AFK user (author tag, timestamp, and message link) which is shown to the user when they return.

* **Message Content, Logging & Automod Triggers:**
  * The Bot scans chat messages in real time to enforce rules (e.g., cross-trade detection, blacklisted phrases, invite links, spam, and command parsing).
  * General messages are processed strictly in memory and are discarded immediately.
  * Only messages that trigger an automod violation or moderation action are stored as log records or rendered proof images for staff review. Proof images may include the sender's avatar, which is fetched from Discord's CDN.
  * If a server administrator enables the optional logger modules (message, profile, role, voice, member, and channel logs), the Bot posts events such as message edits and deletions (including message content), username/avatar/nickname changes, role changes, voice activity, joins/leaves/bans, and channel changes to the log channels chosen by that server. These log entries live in the server's Discord channels and are governed by that server's own access settings.
  * Images or image links that a user submits to an image tool (such as background removal) are downloaded and processed temporarily to produce the result, and are not retained afterwards.

* **Server Configurations:**
  * Custom command triggers/responses, logging channel assignments, whitelisted channels/roles, and anti-nuke parameters configured by server administrators.
  * Other administrator-chosen settings such as sticky messages, join roles, quota settings, help desk and application forms, invite-cleanup settings, advertisement settings, and Blox Fruits stock alert channels.

---

### 2. How We Use the Information

We use the collected data solely to deliver the Bot's core services, including:

* Executing and logging moderation actions (warn, mute, jail, kick, ban).
* Enforcing anti-nuke safeguards (monitoring unauthorized mass role pings, rapid channel creation/deletion, or suspicious bot additions).
* Running the cross-trading automod filter to prevent scams and server rule violations.
* Calculating weekly staff activity metrics against configured server quotas.
* Running staff management tools such as applications, LOA, promotions, and staff feedback.
* Running community tools such as vouches, help desk tickets, AFK status, and server event logging.
* Responding to prefix commands, slash commands, and user queries (such as item value lookups or Blox Fruits stock alerts).

We do **not** sell, rent, monetize, or use any collected data or message content to train machine learning or AI models.

---

### 3. Data Storage and Security

* **Encryption at Rest:** All persistent application data (moderation history, user statistics, configurations) is stored locally in an encrypted database file (`bot_data.db`) using industry-standard AES-128-CBC encryption and HMAC-SHA256 authentication via Fernet.

* **Access Control:** Decryption keys are maintained exclusively in restricted server environment variables and are never exposed to public repositories or unauthorized personnel.

* **Data Transmission:** All interactions between the Bot and Discord are encrypted in transit via Discord's secure WebSocket and HTTPS APIs.

---

### 4. Data Retention and Deletion

* **Retention Period:** Moderation records, infraction logs, and server settings are retained for as long as the Bot remains in the server or until an authorized administrator clears them. Message quota progress counters are reset periodically according to server policy.

* **Right to Deletion:**
  * Server owners may request the complete deletion of their server's stored data by removing the Bot from their server and contacting us directly.
  * Individual users may request the removal of their personal moderation logs, activity statistics, or vouches from our database.

---

### 5. Third-Party Services

The Bot interacts with the following external services solely to fetch publicly available in-game information:

* **Supreme Values** (supremevalues.com): Used to provide publicly listed weapon and trading values.
* **MM2 Values** (mm2values.com): Used to provide publicly listed Murder Mystery 2 item values.
* **Cosmic Values** (bloxfruitsvalues.com): Used to provide publicly listed Blox Fruits values.

The Bot also loads public image assets (such as emoji and flag images from Twemoji via jsDelivr and FlagCDN) and may use Cloudflare's public DNS-over-HTTPS service to look up the address of the websites listed above if the host's own DNS fails. These requests contain only the public website or asset being requested.

No personal user data or Discord identifiers are ever shared with or transmitted to these third-party providers.

---

### 6. Contact Us

If you have questions about this Privacy Policy, wish to request data removal, or have security concerns, please contact the Bot developers:

* **Discord:** kard.z (1455245036860997840)
* **Email:** kardiorubix@gmail.com
