---
name: Baileys runtime requirement
description: Runtime compatibility constraint for the WhatsApp client dependency.
---

Use Node.js 20 or newer for this bot. A broad manifest range such as `>=18` can make Render select a much newer major than the project has been tested on; this project has been verified with Node 24.

**Why:** Baileys' actual minimum is newer than the old manifest declared, and Render selected Node 26 from the broad range while the app had been tested on Node 24. The provided logs do not prove Node 26 caused the crash, so keep the version pin as a compatibility safeguard, not as a confirmed root cause.

**How to apply:** use the tested Node 24 major for Render until a newer major is tested; check Baileys' engine requirement when changing its version.
