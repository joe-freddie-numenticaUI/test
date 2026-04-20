# FAQ AI Bot — Strapi Plugin

An AI-powered FAQ chatbot plugin for Strapi. Drop it into any Strapi project and get an intelligent FAQ assistant in your admin panel.

> ⚠️ **Note:** To test the chatbot API, you can use the [nui-strapi-chatbot-react](https://www.npmjs.com/package/nui-strapi-chatbot-react) package as a simple frontend UI.

[![Node.js >= 18](https://img.shields.io/badge/Node.js-%3E%3D%2018-green.svg)](https://nodejs.org/)
[![npm version](https://img.shields.io/npm/v/nui-strapi-chatbot-plugin)](https://www.npmjs.com/package/nui-strapi-chatbot-plugin)
![Strapi v5](https://img.shields.io/badge/Strapi-%5E5.0.0-blueviolet)

---

## 📦 Installation

```bash
# npm
npm install nui-strapi-chatbot-plugin@latest

# yarn
yarn add nui-strapi-chatbot-plugin@latest

# pnpm
pnpm add nui-strapi-chatbot-plugin@latest
```

---

## 🚀 Build & Start

```bash
npm run build
npm run develop
```

---

## 💡 Usage

1. Start your Strapi app.
2. Open the admin panel and navigate to **FAQ AI Bot** in the sidebar.
3. Set up your [OpenAI API key](https://platform.openai.com/settings/organization/api-keys). Make sure **`gpt-4o-mini`** and **`text-embedding-3-small`** models are available on your account.
4. Add your frontend base domain (used to resolve card assets from its public folder).
5. Add a contact link so the AI can provide it to users on request.
6. Save the configuration.
7. Add your FAQ entries in the **Chatbot-FAQ** collection.
8. The chatbot is ready to use — test it directly from the admin panel.

---

## 🔄 Updating

```bash
npm install nui-strapi-chatbot-plugin@latest

# Then rebuild and restart
npm run build && npm run develop
```

---

## 🔒 Security

- **Admin endpoints** (`/collections`, `/usage`, `/validate-key`) require Strapi admin authentication and are not publicly accessible.
- **Your OpenAI API key** is stored in the Strapi plugin store and is never returned to the browser in plaintext.
- **The `/ask` endpoint** is public (required by the frontend chatbot widget). In production, apply rate limiting at your reverse-proxy or CDN to prevent billing abuse.

---

## ⚠️ Troubleshooting

- Make sure the base domain is set correctly before testing.
- Only add FAQ entries to the **Chatbot-FAQ** collection after providing a valid API key.
- If you see a version mismatch during install, run:

  ```bash
  npm install --legacy-peer-deps
  ```

---

## 📚 Links

- [Strapi Docs](https://docs.strapi.io)
- [Developer Setup](./DEVELOPERS_README.md)
