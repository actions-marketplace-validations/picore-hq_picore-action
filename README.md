# picore

GitHub Action for application security — exposes `scan` and `upload` sub-actions usable independently.

## Usage

### Full action (scan + upload)

```yaml
steps:
  - uses: actions/checkout@v4
  - uses: your-org/picore@v1
```

### Scan only

```yaml
steps:
  - uses: actions/checkout@v4
  - uses: your-org/picore/scan@v1
```

### Upload only

```yaml
steps:
  - uses: actions/checkout@v4
  - uses: your-org/picore/upload@v1
```

## Release

Push a semver tag to trigger an automatic GitHub Release and update the floating major tag (`v1`):

```bash
git tag v1.0.0
git push origin v1.0.0
```

## License

MIT
