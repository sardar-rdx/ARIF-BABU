# Running RDX BOT on Replit

- Runtime: Node.js 20 or newer.
- Start the bot with `npm start`. The Replit workflow sets `PORT=5000` for the pairing console.
- Open the app preview and sign in to the console with username `admin` and the password stored in the `DASHBOARD_PASSWORD` Replit Secret.
- In the console, enter your own WhatsApp number in international format (digits only, including the country code) and request a pairing code. In WhatsApp, open **Settings → Linked Devices → Link with phone number** and enter that code.
- Keep the `session/` directory private. It contains WhatsApp login credentials; do not share it or commit it.

This bot uses an unofficial WhatsApp Web client and may cause account restrictions. Use it only with an account you control, follow WhatsApp's terms, and do not use it for spam or bulk messaging.
