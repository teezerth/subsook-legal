# Store legal pages (HTTPS for App Store Connect)

Static **Privacy Policy** and **Terms of Use** for App Store / Play Console listing URLs.

## Deploy with GitHub Pages

1. Repo **Settings** → **Pages** → Source: **GitHub Actions** (workflow included)
2. After deploy, URLs (default):

   - Privacy: `https://subsook.github.io/SubSook/privacy`
   - Terms: `https://subsook.github.io/SubSook/terms`

3. Paste these into App Store Connect → App Information.

## Local preview

```bash
npx --yes serve store-legal -p 3456
# http://localhost:3456/privacy/
# http://localhost:3456/terms/
```

## Sync with in-app copy

Source of truth for legal text: [`docs/privacy-policy.md`](../docs/privacy-policy.md) and [`docs/terms-of-service.md`](../docs/terms-of-service.md). When you change those, regenerate HTML or edit `privacy/index.html` and `terms/index.html` to match.
