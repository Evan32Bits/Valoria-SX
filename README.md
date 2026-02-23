# 🌌 VALORIA SX — *WIP*

`I'm currently working on it; a stable public release will be available soon.`

**Valoria SX** is a modular, lightweight framework built to enhance FiveM servers with a clean UI, optimized systems, and a modern gameplay experience.  
Each component is designed to be **standalone** or easily integrated with others, allowing server owners to pick only what they need and avoid unnecessary complexity.

This pack includes essentials such as a responsive HUD, a polished loadscreen, a dynamic pause menu, an intuitive inventory system, and simple job mechanics.  
Valoria SX prioritizes **performance**, **visual consistency**, and **ease of use**, making it suitable for both beginners and advanced developers seeking a solid foundation.

---

## 📋 Features — `v0.3`

### ⏳ Loadscreen — `sx-loadscreen` *(Standalone)*
Fully customizable loadscreen with reactive cursor, custom colors, background options, animations, and configuration hooks.

### 🌐 HUD — `sx-hud` *(Dependencies: sx-player, sx-characters)*
Up to six configurable status bars (health, armor, hunger, thirst, stamina, oxygen) plus money display (cash, bank, illegal). Clean, responsive layout designed for clarity and performance.

### 🔔 Notifications — `sx-notify` *(Standalone)*
Customizable, responsive notification system with simple export hooks for other scripts.

### 📱 Phone — `sx-phone` *(Optional dependency: sx-inventory)*
Work in progress — core structure in place, features to be added in upcoming releases.

### 🚶 Player System — `sx-player` *(Dependencies: sx-notify, MySQL DB, oxmysql)*
Core player data management: health, armor, hunger, thirst, and money (cash, bank, illegal). Persistent storage and exportable events/APIs.

### ⏯️ Pause Menu — `sx-menu` *(Standalone classic mode; full features require sx-player)*
Modern pause menu to replace or extend the original GTA V pause menu with configurable entries and quick actions.

### 📦 Inventory — `sx-inventories` *(Dependencies: sx-notify, sx-player, oxmysql, MySQL DB)*
Fully functional inventory: use, drop, give items, and simple item creation. Designed for performance and easy integration.

### 🏪 Shops — `sx-shops` *(Dependencies: sx-inventories, sx-player, sx-notify)*
Shop templates and configuration system. Works out of the box with sx-inventories and can be adapted to other inventory systems.

### 👩‍🌾 Simple Jobs — `sx-easyjobs` *(Dependencies: sx-notify, sx-player)*
Lightweight delivery jobs system, configurable and easy to deploy for quick server content.

---

## 🖼️ Screenshots
Coming soon — screenshots and demo GIFs will be added to the repository and the project page.

---

## 🚀 Quick Start

1. **Requirements**
   - FiveM server
   - MySQL database (for modules that require persistence)
   - `oxmysql` (recommended) or compatible MySQL connector

2. **Installation**
   - Clone the repository into your server resources folder.
   - Add each module you want to `server.cfg`.
   - Configure database credentials and module settings in the provided config files.

3. **Basic Configuration**
   - Edit `config.lua` (or equivalent) for each module to set dependencies, UI options, and database settings.
   - Start the server and verify logs for any missing dependencies.

4. **Notes**
   - Modules are designed to be independent; only enable the ones you need.
   - Example configs and integration snippets are included in each module folder.

---

## 🗺️ Roadmap — Detailed

### ❇️ Current Version — **v0.3**
**Legend:** ✅ Done | ♒ In progress | ❌ To do

- **Loadscreen** — ✅ Complete  
- **HUD** — Health ✅; Armor ✅; Hunger ✅; Thirst ✅; Stamina ✅; Money (cash/bank/illegal) ✅; Oxygen ❌; Responsive UI ✅  
- **Notifications** — Send ✅; Responsive ♒; Exports ✅  
- **Phone** — All ❌ (WIP)  
- **Pause Menu** — Open Settings ✅; Open Shop ✅; Quit Server ✅; Open Map ❌  
- **Inventory** — Use items ✅; Drop items ✅; Give items ❌  
- **Documentation** — French: 90% ; English: 40%

---

### 🗓️ Next Release — **v0.4**
**Priorities**
- Performance optimizations (profiling, DB call reduction, client/server caching)  
- UI/UX polish (animations, transitions, accessibility improvements)  
- Critical bug fixes (dropped items disappearing on zone unload)  
- New internal features (kept private until release)

**Delivery plan**
- Internal beta for rapid iteration and fixes  
- Public beta for community testing and feedback

---

### 🎯 Milestone — **v1.0**
- Full character creator (appearance, presets, save/load)  
- Stable public API (events, exports, hooks for third-party integration)  
- Load testing and stabilization for a public release  
- Packaging and migration guides (examples for ESX/QBCore)

---

### 💡 Backlog / Community Ideas
- Simple quest system (deliveries, daily objectives)  
- Multi-inventory support (backpack, trunk, safe)  
- Optional integrations for popular frameworks (ESX, QBCore)  
- Admin permission system and role management

---

### 📅 Example Timeline
- **v0.4 — Internal Beta:** 4–6 weeks after current stabilization  
- **v0.5 — Public Beta:** 8–12 weeks after v0.4 depending on feedback  
- **v1.0 — Stable Release:** Timeline depends on testing and community feedback

---

## 🧭 Usage & Integration Tips

- Prefer enabling only the modules you need to reduce resource usage.
- Use the provided export hooks to connect third-party scripts without modifying core files.
- For performance-sensitive servers, enable server-side caching and minimize frequent DB writes.
- Follow the example integration snippets in each module to connect with ESX/QBCore or custom frameworks.

---

## 🛠️ Contributing

- Bug reports and feature requests: open an issue with reproduction steps and logs.
- Pull requests: follow the repository coding style, include tests or manual verification steps, and target the `develop` branch.
- Community contributions are welcome, but major changes should be discussed via an issue first.

---

## 🔗 Links
- **Discord:** https://discord.gg/g9HNXUxmht (Valoria SX section)  
- **YouTube:** https://youtube.com/@Evan32Bits (mainly French; some English tutorials)  
- **Twitch:** https://twitch.tv/evan32bits (streams, UTC+1)  
- **GitHub:** https://github.com/Evan32Bits (project owner)

---

## 🏛️ License & Usage

All code in this repository is **proprietary** and owned exclusively by the project author.  
You **may modify and adapt** the code for use on your own server, but you **may not redistribute, resell, or share** the original or modified code with third parties without explicit permission.

Contact via Discord for licensing questions or commercial arrangements.
