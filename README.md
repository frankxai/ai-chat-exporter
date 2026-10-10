# AI Chat Exporter

A Chrome extension that exports AI chat conversations (ChatGPT and Gemini) to Markdown and writes them directly to your Obsidian vault folder.

## Current Scope (v0.2.0)

- Platforms: `chatgpt.com`, `gemini.google.com`
- Export to Markdown with YAML frontmatter
- Direct write to selected Obsidian folder (File System Access API)
- Image download and local path replacement (`assets/` by default)
- Trigger methods: popup, floating button, keyboard shortcut, context menu
- Custom filename and subfolder templates
- **In-page message selection** - Choose specific messages to export
- **User message toggle** - Option to exclude your own messages from exports

## Development

```bash
npm install
npm run dev
npm test
npm run build
```

## First-time setup

1. Load extension in Chrome (`chrome://extensions` -> Developer mode -> Load unpacked).
2. Open extension Options page.
3. Click `Choose Obsidian folder` and authorize your vault.
4. Open a chat on `https://chatgpt.com` or `https://gemini.google.com` and export.

## Template variables

- `{platform}`
- `{title}`
- `{date}` (`YYYY-MM-DD`)
- `{time}` (`HHmmss`)
- `{datetime}` (`YYYY-MM-DD-HHmmss`)
- `{model}`

## License

CC BY-NC-SA 4.0 - See [LICENSE](LICENSE) for details.

This work is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. Non-commercial use only.

<!-- STARLIGHT:OPERATING:BEGIN v2 sha=9f8fecc91edc source=794db1e51a55a128816f7aa266eb0ac1dbd452c3 -->

## Agent operating guidance

Repository agents use the shared Starlight operating contract in `AGENTS.md` alongside local instructions.
The contract asks agents to establish a useful outcome, select relevant skills, complete authorized work,
verify current sources, refine the actual artifact, and report evidence and remaining gates.
It covers human agency, privacy, rights, resource stewardship and bounded proactivity.
Repository identity, brand, canon, build commands and release gates remain local.

[Pinned contract](https://github.com/frankxai/Starlight-Intelligence-System/blob/794db1e51a55a128816f7aa266eb0ac1dbd452c3/docs/architecture/agents-md/band-a.md)
· [Projection and verification](https://github.com/frankxai/Starlight-Intelligence-System/blob/794db1e51a55a128816f7aa266eb0ac1dbd452c3/docs/architecture/AGENTS-MD-CONTRACT.md)

These files supply operating guidance. They do not activate an agent, grant tool permissions,
schedule recurring work, certify compliance or prove a live capability.

<!-- STARLIGHT:OPERATING:END -->
