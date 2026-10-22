---
name: Baileys runtime requirement
description: Runtime compatibility constraint for the WhatsApp client dependency.
---

Use Node.js 20 or newer for this bot. The current Baileys release has an install-time guard that rejects Node 18, despite the root package manifest allowing Node 18.

**Why:** the package manifest's declared engine range does not reflect Baileys' actual minimum runtime.

**How to apply:** keep the configured Node.js runtime at 20 or newer and check Baileys' runtime guard when changing its version.
