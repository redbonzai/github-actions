# setup-cocogitto

This action installs the specified version of [cocogitto](https://github.com/cocogitto/cocogitto) to use in your GitHub Actions workflow.

## Inputs

Name    | Description                         | Required | Default
------- | ----------------------------------- | -------- | -------
version | The version of cocogitto to install | false    | "6.1.0"
architecture | The architecture of the machine to install cocogitto on | false | "x86_64-unknown-linux-musl"

## Usage

```yaml
# Uses the latest version of cocogitto (currently 6.1.0)
- uses: redbonzai/github-actions/setup-cocogitto

# Uses a specific version of cocogitto
- uses: redbonzai/github-actions/setup-cocogitto
  with:
    version: "6.1.0"

# Verify the version of cocogitto
- run: cog --version
```
