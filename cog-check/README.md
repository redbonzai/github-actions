# cog-check

This Github Action checks whether the commits follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification using [cogogitto](https://github.com/cocogitto/cocogitto).

## Usage

```yaml
- uses: redbonzai/github-actions/cog-check@v0
```

Override the default values:

```yaml
- uses: redbonzai/github-actions/cog-check@v0
  with:
    from-latest-tag: false
    ignore-merge-commits: false
```

## Inputs

Name                    | Description                                        | Required | Default
----------------------- | -------------------------------------------------- | -------- | --------------
from-latest-tag         | Only checks commits from the latest tagged version | false    | `true`
ignore-merge-commits    | Ignores merge commits                              | false    | `true`
