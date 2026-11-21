# Granite for Claude, Cursor and other AI apps

Granite is a document vault. Drop in a bill, a tax form, an insurance policy or an ID, and Granite reads it, files it under the right type, pulls out the details that matter (dates, amounts, policy numbers) and keeps it findable.

This repo connects your Granite vault to AI apps, so you can work with your documents in conversation:

- **Find things.** "What's the deductible on my car insurance?" "When does my passport expire?"
- **Add things.** "Save this as a note in Granite." "Add this PDF to my vault."
- **Tidy up.** Rename a document, fix a detail Granite got wrong, move it into a collection, mark a bill as paid, or delete a duplicate. Your AI app asks you before it deletes anything.
- **Ask across everything.** "How much did I pay contractors in 2024?" uses Granite's own answers, with the documents they came from. (Paid plan.)

You need a Granite account. Free accounts can search, read and add up to 25 documents. You choose what each app may do on Granite's permission screen, and you can see and disconnect apps any time in Granite under Settings, Connected apps.

## Claude

In Claude Code:

```
/plugin install granite --marketplace Ordinary-Systems/granite-connectors
```

Then run `/mcp` and sign in to Granite.

In Claude on the web, desktop or mobile: add Granite from the connector directory, or go to Settings, Connectors, add a custom connector, and paste `https://api.granite.co/mcp`.

The plugin includes the Granite connector and a skill that teaches Claude how to find, file and update documents well.

## Cursor

[Add Granite to Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=granite&config=eyJ1cmwiOiJodHRwczovL2FwaS5ncmFuaXRlLmNvL21jcCJ9), then sign in to Granite when Cursor asks.

## VS Code

[Add Granite to VS Code](https://vscode.dev/redirect?url=vscode%3Amcp%2Finstall%3F%257B%2522name%2522%253A%2522granite%2522%252C%2522type%2522%253A%2522http%2522%252C%2522url%2522%253A%2522https%253A%252F%252Fapi.granite.co%252Fmcp%2522%257D), then sign in to Granite when VS Code asks.

## ChatGPT, Grok and others

Any app that supports remote MCP connectors can use Granite. Add a custom connector with the URL `https://api.granite.co/mcp` and sign in. In ChatGPT the connection is read-only and shows selected details from supported document types. Setup steps for each app: https://granite.co/docs/mcp.

## Privacy

An AI app only reaches your vault after you connect it, and only for what you ask. See the [Granite privacy policy](https://granite.co/privacy).

## Help

Docs: https://granite.co/docs/mcp. Questions: hello@granite.co.
