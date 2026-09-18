# GetTranscribe for Cursor

GetTranscribe connects Cursor to public video transcription workflows. It can create and monitor transcription jobs, retrieve complete transcripts, organize content in folders, and help analyze the resulting material.

## Supported sources

- YouTube
- Instagram
- TikTok
- Facebook

Videos must be publicly accessible. Availability can vary when a source platform restricts access.

## Install from Cursor Marketplace

After this plugin is approved, open **Cursor → Customize → Plugins**, search for **GetTranscribe**, and install it for your user or project.

Cursor connects to the hosted MCP endpoint at `https://mcp.gettranscribe.ai/mcp`. On first use, complete the GetTranscribe authorization flow with your own API key. This plugin does not contain API keys or other secrets.

## Use it

Ask Cursor to transcribe a supported public video URL. For example:

```text
Transcribe https://www.youtube.com/watch?v=example and give me the key ideas.
```

You can also ask it to list transcripts, retrieve one by ID, create folders, or summarize and analyze saved results.

## Local testing

1. Copy this repository into `~/.cursor/plugins/local/gettranscribe`.
2. In Cursor, run **Developer: Reload Window**.
3. Open **Customize** and confirm the GetTranscribe skill and MCP server appear.
4. Start a request that requires GetTranscribe and complete authorization when prompted.

## Security and privacy

The MCP server is hosted by GetTranscribe and authenticates each user separately. The plugin only points Cursor at the public MCP endpoint. Do not add API keys to this repository.

## License

MIT. See [LICENSE](LICENSE).
