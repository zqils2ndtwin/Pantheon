# 🏛️ Pantheon

## Embrace the Power of the Gods!

*A Minecraft plugin where ancient Greek myths collide with your world.*

Pantheon introduces a rich, lore-driven experience where players can discover, build, and commune with the mighty Olympians. Forge legendary artifacts, master divine abilities, encounter mythic creatures, and shape your destiny through interaction with the gods themselves.

---

### ✨ Features

*   **Divine Altars:** Discover and construct powerful altars to honor the Greek Pantheon.
*   **AI-Powered Deities:** Engage in dynamic, intelligent conversations with summoned gods using advanced AI.
*   **Permanent Blessings:** Earn stackable, permanent potion effects from the gods to empower your journey.
*   **Legendary Artifacts:** Wield unique custom items infused with divine power and special abilities.
*   **Mythic Creatures:** Encounter rare and challenging creatures, guardians of sacred components.
*   **Ancient Rituals:** Perform complex, multi-stage rituals to craft powerful cores and items.
*   **Dynamic World Events:** Experience natural phenomena tied to the gods' influence.
*   **Hermes, the Messenger:** A mysterious messenger appears periodically to offer guidance and wisdom.

---

### 📦 Installation

1.  **Download:** Grab the latest `Pantheon.jar` from the [releases page](YOUR_GITHUB_RELEASES_LINK_HERE).
2.  **Place:** Drop the `Pantheon.jar` file into your server's `plugins/` directory.
3.  **Restart/Reload:** Start or restart your server.
4.  **Configure:** Important! Edit the generated `plugins/Pantheon/gemini.yml` file and set your Gemini API Key. AI interactions will **not** work without it.
    *   *Tip:* For security, consider setting the `GEMINI_API_KEY` as an environment variable on your server; it will take precedence over the key in the file.
5.  **Enjoy:** Dive into the world of divine myths!

---

### ⚙️ Configuration

Pantheon uses several YAML files for extensive customization:

*   `config.yml`: The main configuration file, detailing all god altars, their structures, core items, and Hermes dialogue hints.
*   `gemini.yml`: Configures the AI integration, including your Gemini API Key and the AI model to use.
*   `trading.yml`: Defines the base structure and instructions for the AI's trading/blessing sessions.

**Important Security Note for `gemini.yml`:**
Your `gemini-api-key` is sensitive information. **Do not share this file publicly** or commit it to public repositories without first removing or redacting your API key. Using an environment variable (`GEMINI_API_KEY`) is the recommended and most secure method.

---

### 📖 Core Mechanics

#### 🏛️ The Divine Altars

At the heart of every god's power lies their altar. Each deity requires a unique structure, built from specific materials around a sacred **Altar Core**.

*   **Construction:**
    *   Locate the recipe for an Altar Core (often hinted at by Hermes, or found through special rituals).
    *   Craft the Altar Core item.
    *   Place the Altar Core in the world, ensuring the surrounding block structure matches the god's specific blueprint (revealed through exploration or ancient texts).
    *   The plugin will automatically detect a correctly built altar.

*   **Altar of Insight (Athena):** A special altar that allows you to attune an "Aegis Codex" into an "Attuned Aegis Codex," revealing deeper secrets.

#### 💬 Communing with Gods (AI Dialogue)

Once an altar is active, you can call upon the deity's manifestation.

*   **Summoning:** Hold a **Theophany Stone** and use `/pray [your prayer/message]` near an active altar.
    *   A unique divine manifestation will appear, representing the god.
*   **Conversation:** Continue your dialogue with the god using `/godwhisper [your message]` or `/gw [message]`.
    *   The gods are powered by advanced AI (Google Gemini), offering dynamic and context-aware responses.
*   **Trading & Blessings:** Gods may offer to trade powerful artifacts or bestow permanent blessings in exchange for **Nether Stars**.
    *   When prompted, a magical chest will appear for you to place your offering. Close the chest, then continue your conversation with `/gw` to finalize the trade.
*   **Dismissal:** To end your communion, use `/godleave` or `/gl` near the manifestation.

#### ✨ Divine Blessings

Receive the eternal favor of the gods! These are **permanent potion effects** granted by deities in exchange for offerings. Unlike regular potion effects, they persist through death and logout, providing a lasting boost to your abilities.

#### ⚔️ Artifacts of Olympus (Custom Items & Abilities)

Unearth and forge unique custom items, each with powerful NBT-based abilities.

*   **Pallas' Edge (Athena):** A golden sword with a chance to disarm opponents and mark foes for increased damage.
*   **Craftsman's Compass (Athena):** A mystical compass that guides you to structures, cycles targets, and briefly reveals nearby ores.
*   **Poseidon's Trident:** A trident imbued with oceanic power, slowing foes on hit and summoning a damaging water vortex.
*   **Scales of the Deep (Poseidon):** A helmet granting permanent water breathing and a powerful swimming boost.
*   **Soulreaper (Hades):** A netherite sword that harvests souls from fallen foes, healing the wielder and fueling a laser that pulls and withers enemies.
*   **Helm of Darkness (Hades):** A shadowy helmet that grants wither immunity, spectral particles, and temporary invisibility on kill.
*   **Ares' War Axe:** An axe that causes foes to bleed and allows a "Berserker Charge" for speed and resistance.
*   **Berserker's Cuirass (Ares):** Armor that grants strength and resistance at low health, and a burst of speed on kill.
*   **Queen's Diadem (Hera):** A regal helmet granting passive speed and a chance to summon a "Peacock's Glare" to attack assailants when you're damaged.
*   **The Crossroads Staff (Hecate):** A staff allowing you to launch debilitating hex bolts and warp short distances.
*   **Whisper-Step Boots (Hecate):** Boots providing wither rose immunity, magic damage reduction, strength with magic items, and enhanced speed at night or in swamps.
*   **Lifegiver's Verdant Hoe (Demeter):** A hoe that instantly harvests and replants mature crops, and can cause abundant growth in an area.
*   **Verdant Heartstone (Demeter):** A powerful block that accelerates crop/sapling growth and passively heals nearby passive mobs.
*   **Adamantine Girdle (Hephaestus):** Leggings that reduce durability loss on all armor and provide fire resistance.
*   **Forgemaster's Pickaxe (Hephaestus):** A pickaxe with auto-smelt and silk touch modes, and a "Forgemaster's Maw" (pocket inventory) to store mined items.

#### 👹 Mythic Creatures

The world now holds unique creatures tied to the gods:

*   **Abyssal Guardian (Poseidon):** A formidable drowned variant found in deep oceans, guarded by potent enchantments. Defeat it for an "Ocean Depths Gem."
*   **Athena's Owl:** Rare, naturally spawning chickens in specific biomes. They are sources of "Owl Feather Quills."
*   **Night Wraith (Hecate):** A rare, empowered Phantom variant that emerges at night. Dropping "Spectral Dust" upon defeat.
*   **Stygian Guardian (Hades):** Powerful Wither Skeletons that defend the Stygian Fissures.

#### 🧪 Rituals & Crafting

Beyond standard crafting, Pantheon introduces complex rituals:

*   **Hecate's Moonlit Catalyst Ritual:** A multi-stage brewing process on a brewing stand, requiring specific ingredients added at the right time and environment (swamp, night), culminating in the "Moonlit Catalyst Potion." Consumption under the correct conditions yields the Altar Core.
*   **Hephaestus' Forge Heart Ritual:** Involves placing an "Unfired Core Mold," firing it with lava, rhythmically shaping molten netherite with a hammer, and then quenching it with water.
*   **Lectern Unlocks:** Place certain custom books on a lectern (like the "Aegis Codex" or "Attuned Aegis Codex") to reveal hidden recipes for core items and components.
*   **Component Crafting:** Discover and combine unique components like "Crown Jewel Shards," "Golden Thread," "Compressed Netherite Ingots," and the "Theophany Stone."

#### 🌍 World Events

The gods' influence manifests directly in your world:

*   **Stygian Fissures (Hades):** Rare, dangerous obsidian structures found deep underground in Deep Dark biomes. Activate them to face waves of Stygian Guardians and claim the "Stygian Core."
*   **Verdant Heartstones (Demeter):** Place this item to create an aura that accelerates crop growth and heals passive mobs.
*   **Hermes, the Messenger:** Periodically, a mystical Ocelot representing Hermes will appear. Interact with him to receive guidance on the gods, their altars, and how to obtain their core items. He can also direct you to the plugin's wiki!

---

### 🎮 Commands

For a full list of commands and their detailed usage, please visit the [Commands Wiki Page](YOUR_GITHUB_WIKI_LINK_HERE/Commands).

*   `/pantheon` or `/pt`: Main plugin command for admins and debugging (reload, give items, build altars, summon entities).
*   `/pray [prayer/message]` or `/p [prayer/message]`: Initiate communion with a nearby god.
*   `/godwhisper [message]` or `/gw [message]`: Continue your conversation with a god.
*   `/godleave` or `/gl`: Dismiss a divine manifestation.

---

### 🔐 Wiki Access

To access the full Pantheon wiki and discover all secrets, use `/pt getpass` in-game. This will reveal the current password for the wiki.

---

### 🛡️ Permissions

For a detailed breakdown of all plugin permissions, please visit the [Permissions Wiki Page](YOUR_GITHUB_WIKI_LINK_HERE/Permissions).

---

### 🤝 Contributing & Support

We welcome contributions and feedback!

*   **Feature Requests:** Have an idea for a new god, item, or mechanic? Open a discussion or a feature request on GitHub.
*   **Code Contributions:** Feel free to fork the repository and submit pull requests.

Need help? Join our [Discord Server](YOUR_DISCORD_SERVER_LINK_HERE)!

---

### ✨ Credits

*   **Developer:** Zqil
*   **Built on:** [PaperMC](https://papermc.io/)
*   **AI Integration:** [Google Gemini API](https://ai.google.dev/models/gemini)
*   **Libraries:** Kyori Adventure, Gson

---

### 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Dive into the world of Pantheon today and carve your legend among the gods!
