# Buoy Design

**Design system linting and drift detection for modern frontend teams.**

Buoy helps teams maintain design consistency by detecting when code drifts from your design system. Like ESLint for your design tokens.

## What We Build

| Project | Description |
|---------|-------------|
| [buoy](https://github.com/ahoybuoy/buoy) | Core scanners, CLI, and MCP server for design system analysis |
| [buoy-action](https://github.com/marketplace/actions/buoy-design-drift-detection) | GitHub Action for CI/CD drift detection |
| [buoy.design](https://buoy.design) | Cloud platform with PR comments, @buoy mentions, and design graphs |

## Quick Start

### GitHub Action (Free)

```yaml
- uses: ahoybuoy/buoy@v1
  with:
    github-token: ${{ secrets.GITHUB_TOKEN }}
```

### CLI

```bash
npx @ahoybuoy/cli check
```

### @buoy Mentions

Install the [Buoy GitHub App](https://buoy.design) and mention `@ahoybuoy` in any PR comment:

> @ahoybuoy why is this color hardcoded?

Buoy will analyze your code and respond with design system context.

## What Buoy Catches

- Hardcoded colors instead of design tokens
- Magic spacing values (padding, margin, gap)
- Arbitrary Tailwind values (`bg-[#123456]`)
- Typography inconsistencies
- Missing component usage

## Links

- [Documentation](https://buoy.design/docs)
- [GitHub Marketplace](https://github.com/marketplace/actions/buoy-design-drift-detection)
- [Discord Community](https://discord.gg/buoy)

---

Built with care by the Buoy team.
