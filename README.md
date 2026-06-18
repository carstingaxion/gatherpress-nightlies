# GatherPress Nightly

> [!TIP]
> **Want to test the latest GatherPress features?**
>
> Download the latest [gatherpress-nightly.zip][gatherpress-nightly-zip], [![Try it in WordPress Playground][playground-badge]][blueprint-nightly] or get it from the [Releases](../../releases) page and help test what's coming next to gather.

## What is this?

This repository provides automated nightly builds of GatherPress.

A new build is generated every day from the latest development code, making it easy for testers, site owners, and contributors to stay up to date without checking out source code and running build scripts locally.

## Installation

1. Download the latest [gatherpress-nightly.zip][gatherpress-nightly-zip] or get it from the [Releases](../../releases) page.
2. Install as a normal WordPress plugin.
3. Start testing.

### Use it directly in Playground

You might want to create a WordPress Playground with your plugin or theme and the latest development version of GatherPress for development and compatibility testing.

```json
{
  "$schema": "https://playground.wordpress.net/blueprint-schema.json",
  "steps": [
    {
      "step": "installPlugin",
      "pluginData": {
          "resource": "url",
          "url": "https://github.com/GatherPress/gatherpress-nightlies/releases/latest/download/gatherpress-nightly.zip"
      },
      "options": {
          "activate": true
      }
    }
  ]
}
```


## Automatic Updates

Nightly builds can be updated automatically using the [Git Updater](https://github.com/afragen/git-updater) plugin by **Andy Fragen**.

This allows test sites to stay current with the latest nightly release with minimal effort.

## Important

> [!WARNING]
> Nightly builds are development versions and may contain:

* Bugs
* Incomplete features
* Breaking changes

Do not use nightly builds on production sites!

## Feedback

Found an issue?

Please report it in the *main* [GatherPress/gatherpress](https://github.com/GatherPress/gatherpress/issues/new/choose) repository so the team can investigate and improve future releases.

## Credits

- Replicated from the [Gutenberg Nightlies](https://github.com/Automattic/gutenberg-nightlies) project.
- Credits & thanks to [@bph](https://github.com/bph) for the idea!

<!-- markdownlint-disable-next-line MD047 -->
[gatherpress-nightly-zip]: https://github.com/GatherPress/gatherpress-nightlies/releases/latest/download/gatherpress-nightly.zip
[playground-badge]: https://img.shields.io/badge/Try_it-in_WordPress_Playground-blue?logo=wordpress&logoColor=%23fff&labelColor=%233858e9&color=%233858e9
[blueprint-nightly]: https://playground.wordpress.net/?blueprint-url=https://raw.githubusercontent.com/GatherPress/gatherpress/main/.wordpress-org/blueprints/blueprint-nightly.json