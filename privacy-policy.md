# Privacy Policy

**Last Updated:** September 2, 2026

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




* **Staff Activity & Management Data:**
* Message counts bucketed by time (daily, weekly, monthly, all-time) and moderation case counts to track weekly staff quota progress.


* Staff promotion/demotion history and Leave of Absence (LOA) records (durations, status, approval metadata).


* Internal staff review scores and feedback comments.




* **Message Content & Automod Triggers:**
* The Bot scans chat messages in real time to enforce rules (e.g., cross-trade detection, blacklisted phrases, invite links, spam, and command parsing).


* General messages are processed strictly in memory and are discarded immediately.


* Only messages that trigger an automod violation or moderation action are stored as log records or rendered proof images for staff review.




* **Server Configurations:**
* Custom command triggers/responses, logging channel assignments, whitelisted channels/roles, and anti-nuke parameters configured by server administrators.





---

### 2. How We Use the Information

We use the collected data solely to deliver the Bot's core services, including:

* Executing and logging moderation actions (warn, mute, jail, kick, ban).


* Enforcing anti-nuke safeguards (monitoring unauthorized mass role pings, rapid channel creation/deletion, or suspicious bot additions).


* Running the cross-trading automod filter to prevent scams and server rule violations.


* Calculating weekly staff activity metrics against configured server quotas.


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

The Bot interacts with the following external APIs solely to fetch publicly available in-game information:

* **Bloxy Values API:** Used to retrieve current in-game fruit stock rotations.


* **Supreme Values:** Used to provide publicly listed weapon and trading values.

No personal user data or Discord identifiers are ever shared with or transmitted to these third-party providers.

---

### 6. Contact Us

If you have questions about this Privacy Policy, wish to request data removal, or have security concerns, please contact the Bot developers:

* **Discord:** `[Your Discord Tag/Username or Support Server Link]`
* **Email:** `[Your Contact Email Address]`
