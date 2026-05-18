# amlmarketplaces/stability

Claude Code marketplace federating all `@amlplugins/stability-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-stability": {
      "source": { "source": "github", "repo": "amlmarketplaces/stability" }
    }
  },
  "enabledPlugins": {
      "stability-control@aml-stability": true,
      "stability-edit@aml-stability": true,
      "stability-generate@aml-stability": true,
      "stability-three-d@aml-stability": true,
      "stability-upscale@aml-stability": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/stability`, cached under `~/.claude/plugins/cache/aml-stability/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (6 total)

- `stability-control` — [@amlplugins/stability-control](https://github.com/amlplugins/stability-control)
- `stability-edit` — [@amlplugins/stability-edit](https://github.com/amlplugins/stability-edit)
- `stability-generate` — [@amlplugins/stability-generate](https://github.com/amlplugins/stability-generate)
- `stability-three-d` — [@amlplugins/stability-three-d](https://github.com/amlplugins/stability-three-d)
- `stability-upscale` — [@amlplugins/stability-upscale](https://github.com/amlplugins/stability-upscale)
- `stability-video` — [@amlplugins/stability-video](https://github.com/amlplugins/stability-video)

## Related

- npm packages: `@amlplugins/stability-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
