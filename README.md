# Oliver's mTOR Atlas: plugins for AI assistants

Small install packages for [Oliver's mTOR Atlas](https://mtor-atlas.org), a curated, evidence-labelled corpus of mTOR research. Each one connects your assistant to the Atlas's public, read-only MCP server:

`https://mtor-atlas-mcp.mtor-atlas.workers.dev/mcp` (Streamable HTTP, no key, no account)

The server has 11 tools: search studies by keyword, evidence code, entity or year; look up genes, complexes, drugs and diseases; find signed pathway relations with their supporting and conflicting studies; list contested claims and open questions. Every study carries an evidence code (human, animal, molecular, review...) that says what kind of study it is, not how good it is.

## Claude Code

```
/plugin marketplace add open-mtor-atlas/mtor-atlas-plugins
/plugin install mtor-atlas@mtor-atlas
```

Or without the plugin: `claude mcp add --transport http mtor-atlas https://mtor-atlas-mcp.mtor-atlas.workers.dev/mcp`

## Gemini CLI

```
gemini extensions install https://github.com/open-mtor-atlas/mtor-atlas-plugins
```

## Other clients

Claude.ai, ChatGPT, Cursor and other MCP clients can add the server URL above directly. A local stdio version is on npm as [`mtor-atlas-mcp`](https://www.npmjs.com/package/mtor-atlas-mcp). Source and API documentation: [github.com/open-mtor-atlas/atlas](https://github.com/open-mtor-atlas/atlas/tree/main/mcp), [mtor-atlas.org/api](https://mtor-atlas.org/api/).

## Data and citation

Data CC BY 4.0, dataset DOI [10.5281/zenodo.22059963](https://doi.org/10.5281/zenodo.22059963). Not medical advice.
