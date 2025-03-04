# gha-debian-tmate

A GitHub Action that starts an interactive tmate debugging session in a Debian-like environment.

## Usage

```yaml
steps:
  - uses: actions/checkout@v4
  - name: Setup Debug Session
    uses: yourusername/gha-debian-tmate@v1
    with:
      timeout-minutes: 30  # optional, default is 30
```

## Development

To test the action locally:

```bash
git tag -d test || true ; git push origin :refs/tags/test || true ; git tag test && git push origin test
```
