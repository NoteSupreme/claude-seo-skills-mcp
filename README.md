# Claude SEO Skills MCP

A free, read-only MCP server that serves two open-source SEO skill packs to Claude and any other AI agent: site audits, local SEO and Google Maps, schema, competitor and /vs/ pages, Reddit, AI search citations, copywriting and more. Your AI finds the right skill, reads its instructions, and follows them. No install, no files to copy.

Hosted on [NoteSupreme](https://notesupreme.com/?ref=github).

## The two packs

### Claude SEO — by [AgriciDaniel](https://github.com/AgriciDaniel)
Source: **[github.com/AgriciDaniel/claude-seo](https://github.com/AgriciDaniel/claude-seo)** · MIT License

Full-site audits, single-page analysis, technical SEO, schema, content quality and E-E-A-T, backlinks, images, sitemaps, programmatic SEO, competitor pages, Google APIs, **local SEO and Google Maps** (geo-grid rank tracking, GBP audits, reviews). The FLOW prompts come from [github.com/AgriciDaniel/flow](https://github.com/AgriciDaniel/flow) under CC BY 4.0.

### Illyism SEO Skills — by [Ilias Ism](https://github.com/Illyism)
Source: **[github.com/Illyism/seo-skills](https://github.com/Illyism/seo-skills)** · MIT License · catalog at [il.ly/skills](https://il.ly/skills)

Output-first SaaS SEO: /vs/ and alternatives pages, Reddit threads that rank on Google, directory submissions, AI search (GEO) citations, de-slopping content, title rewrites, blog refreshes, YouTube SEO, customer research and copywriting. No local SEO.

> A few Illyism skills use the author's paid tools (LinkDR, AI SEO Tracker, Scribiz, Awesome Tools). They're tagged `uses-paid-service`, and the MCP tells your AI to check with you before relying on them.

This MCP hosts the skill instruction files only. Scripts and installers live in the original repos. All credit for the skills goes to their authors; please star their repos.

## Try asking

- "Using the Claude SEO skills MCP, run a local SEO audit for my plumbing business site."
- "Find the skill for writing /vs/ competitor pages and follow it for my product vs. Notion."
- "Which skill helps me get cited in ChatGPT and Perplexity answers?"

## Connect it

It's a remote MCP server (Streamable HTTP). No install, no API key, no sign-up: the link below includes its access token.

```
https://notesupreme.com/p/claude-seo-skills?token=nsp_9_aGgxEI87BKDjSVUU8Zfg
```

**Claude (claude.ai / Desktop):** Settings → Connectors → Add custom connector → paste the URL.

**Claude Code:**
```bash
claude mcp add --transport http claude-seo-skills "https://notesupreme.com/p/claude-seo-skills?token=nsp_9_aGgxEI87BKDjSVUU8Zfg"
```

**Cursor / VS Code / Windsurf** (`mcp.json` or the app's MCP settings):
```json
{
  "mcpServers": {
    "claude-seo-skills": { "url": "https://notesupreme.com/p/claude-seo-skills?token=nsp_9_aGgxEI87BKDjSVUU8Zfg" }
  }
}
```

**ChatGPT and any other MCP app:** add a remote MCP server / custom connector and paste the same URL.

Opened in a browser, the link explains how to connect.

## About NoteSupreme

[NoteSupreme](https://notesupreme.com/?ref=github) is long-term memory for your AI. You keep notes, specs and research as plain markdown, and every project gets its own MCP URL. Your AI searches what you already know instead of guessing, and uses up to 97% fewer tokens doing it than reading the files raw.

**One account, many Ships.** A Ship is one project: a vault of markdown notes with its own MCP URL and its own chat history. The Free plan includes 5 Ships, no card. Paid plans are unlimited.

**Every Ship gets three MCPs:**

| MCP | Who it's for | What it does |
|---|---|---|
| **Code Mode MCP** | you | One tool. Your AI writes a few lines of JavaScript, a sandbox walks the whole Ship, and only the answer comes back into your context. |
| **Regular MCP** | you, in any app | 23 plain tools (search, read, write, frontmatter, version history…) for apps that don't support Code Mode yet. |
| **Read-only MCP** | other people | Publish a Ship and give the link away. Guests get the whole knowledge graph and none of the write tools. **This repo's MCP is one of these.** |

**Built-in RAG on Google's Open Knowledge Format ([OKF](https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md)), no vector database.** Each note is a markdown file that carries a type, a one-line description and tags, and notes link to each other. Your AI keyword-matches the right entry note, then follows the links a few hops, so it reads a small, relevant slice instead of everything. Nothing to embed or re-index, so a note you saved a second ago is already searchable. A short "how this Ship is organized" note tells every AI how to search that Ship.

**Also in the box:** a desktop workspace with AI chat beside your docs, 30-day version history on every write, import/export of markdown folders, a phone app with voice, and a 3D "2nd Brain" view of your whole account.

Build your own: **[notesupreme.com](https://notesupreme.com/?ref=github)**
