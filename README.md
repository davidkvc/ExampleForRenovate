# Renovate repro for discussion 38773

Self-hosted renovate config:

```js
module.exports = {
  platform: 'github',
  repositories: ['davidkvc/ExampleForRenovate'],
};
```

Run renovate with:

```sh
export RENOVATE_PLATFORM="github"
export RENOVATE_TOKEN= "github_pat_xxx"
npx renovate@41.154.0
```

## Current behavior

Renovate doesn't consider Serilog for updates even though newer versions exist.

## Expected behavior

Renovate should create issue to update Serilog.

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/38773
