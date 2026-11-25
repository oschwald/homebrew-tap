# Homebrew tap

Homebrew packages maintained by Gregory Oschwald.

## MaxMindDB MCP Server

The [MaxMindDB MCP Server](https://github.com/oschwald/maxminddb-mcp) release workflow updates this tap after each stable release.

Install on macOS with:

```sh
brew install --cask oschwald/tap/maxminddb-mcp
```

Upgrade with:

```sh
brew upgrade --cask oschwald/tap/maxminddb-mcp
```

The binary is not signed or notarized by Apple. Homebrew marks downloaded files as quarantined, so macOS may refuse to run it. If an MCP client cannot start the server, or macOS says the developer cannot be verified, clear the quarantine flag after installing and after each upgrade:

```sh
xattr -d com.apple.quarantine "$(brew --prefix)/bin/maxminddb-mcp"
```

See the [installation guide](https://github.com/oschwald/maxminddb-mcp#installation) for configuration and Claude Desktop extensions.
