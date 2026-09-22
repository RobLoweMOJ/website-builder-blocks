# Website Builder Blocks

## Features

This plugin adds the following custom blocks,
* Accordion
* Filterable listing
* HM Government logo SVG
* Reveal
* Table of contents

## Issues
Raise issues via
[GitHub issues](https://github.com/ministryofjustice/website-builder-blocks/issues)

## Installation
Download `website-builder-blocks-X.Y.Z.zip` from the
[latest release](https://github.com/ministryofjustice/website-builder-blocks/releases/latest),
unzip it and copy the `website-builder-blocks` folder into your WordPress plugin directory.

The repository itself doesn't include the compiled assets (`build/`), so a plain
clone or GitHub's "Download ZIP" won't work until you build it.

### Releasing
Bump the `Version:` header in `website-builder-blocks.php` in your PR. When it's
merged to `main`, the [release workflow](.github/workflows/release.yml) builds the
assets, tags the version and publishes the release zip. Merges that don't bump the
version don't release.

## Development
Compiled assets aren't committed. After cloning, build them with:

```
npm install
npm run build
```

Use `npm run watch` while developing.

## Coding guidelines
This plugin follows
* Standards set by the Wordpress organisation https://codex.wordpress.org/Writing_a_Plugin.
* PHP Framework Interop Group's standards http://www.php-fig.org/
