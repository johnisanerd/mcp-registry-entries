# MCP Registry entries

`server.json` files for johnvc Apify Actors listed in the official MCP Registry
(`io.github.johnisanerd/*`), published from GitHub Actions with GitHub OIDC.

- Publish one entry: run **Publish to MCP Registry** with `server` set to a folder
  under `servers/` (tick `dry_run` to run the checks only).
- Change an entry's status: run **Set MCP Registry status**.

Publish about three entries a day, a few hours apart. Never list
youtube-download-api.

Each entry's `websiteUrl` points at its docs page on alphaosint.com (`/mcp/<name>/`), which lists
the tools, parameters, outputs, client setup and prices. GitHub's MCP Registry review (Nov 2026)
asked for that and for no affiliate links, so registry entries never carry `fpr=` and leave out
`repository` while the linked repo READMEs still do.

GitHub's review (ticket 173176, Nov 10) reads the registry entry and its linked GitHub repository,
not `websiteUrl`, and the registry rejects entries without `repository`. So every reviewed entry sets
`repository` to its folder in johnisanerd/alphaosint-mcp-servers (`subfolder: servers/<name>`), whose
README has the tools, parameters, example, client setup, billing note and no referral links.
