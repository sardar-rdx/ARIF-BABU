# Running RDX BOT on Replit

- Runtime: Node.js 24.x (Baileys requires Node.js 20 or newer).
- Install dependencies with `npm ci`, then run the `Start application` workflow to open the pairing page in Replit Preview on port 5000.
- The Replit workflow uses pairing-only mode, so the page opens without a dashboard login and the bot-control endpoints stay disabled.
- Do not share the preview link or pairing codes. Only pair a WhatsApp account you own.
- Keep the `session/` directory private. It contains WhatsApp login credentials; do not share it or commit it.
- For Render, use `npm start` as the service start command so persistent storage is prepared. The Render config enables `PAIRING_ONLY`; set `PAIRING_NUMBER` in the service environment to the account’s full international number (digits only) before requesting a pairing code. Without it, the page starts but pairing is refused.

This bot uses an unofficial WhatsApp Web client and may cause account restrictions. Use it only with an account you control, follow WhatsApp's terms, and do not use it for spam or bulk messaging.
