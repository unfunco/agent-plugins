# Agent plugin marketplace

Marketplace of custom agent plugins for GitHub Copilot and Claude Code,
maintained by Daniel Morris.

## Getting started

### Installation and usage

#### GitHub Copilot

Add this repository as a plugin marketplace:

```bash
copilot plugin marketplace add unfunco/agent-plugins
```

Browse the marketplace to see the plugins that are currently available:

```bash
copilot plugin marketplace browse unfunco-agent-plugins
```

Install a plugin:

```bash
copilot plugin install <plugin-name>@unfunco-agent-plugins
```

#### Claude Code

Add this repository as a plugin marketplace:

```bash
claude plugin marketplace add unfunco/agent-plugins
```

Browse the marketplace to see the plugins that are currently available by
running `/plugin` inside a Claude Code session.

Install a plugin:

```bash
claude plugin install <plugin-name>@unfunco-agent-plugins
```

### Maintenance

The marketplace is defined twice, once for each tool, and both files must list
the same plugins:

- [`.github/plugin/marketplace.json`](.github/plugin/marketplace.json) for
  GitHub Copilot
- [`.claude-plugin/marketplace.json`](.claude-plugin/marketplace.json) for
  Claude Code

Validate the Claude Code marketplace after changing it:

```bash
claude plugin validate .
```

## License

© 2026 [Daniel Morris]\
Made available under the terms of the [MIT License].

[daniel morris]: https://unfun.co
[mit license]: LICENSE.md
