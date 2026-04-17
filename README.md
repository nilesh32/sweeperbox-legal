# Sweeperbox Legal

Public-facing legal + support pages for the Sweeperbox iOS app.

## Pages

- [Privacy Policy](./privacy.md)
- [Terms of Service](./terms.md)
- [Support](./support.md)

## Hosting (GitHub Pages)

1. Push this folder to a public GitHub repo named `sweeperbox-legal`.
2. Repo Settings → Pages → Source: `Deploy from a branch` → Branch: `main` / root → Save.
3. After ~1 min, pages are live at:
   - `https://<your-github-username>.github.io/sweeperbox-legal/privacy`
   - `https://<your-github-username>.github.io/sweeperbox-legal/terms`
   - `https://<your-github-username>.github.io/sweeperbox-legal/support`

## Wire up in app

Update `Sweeperbox/Config.swift`:

```swift
static let privacyPolicyURL = URL(string: "https://<you>.github.io/sweeperbox-legal/privacy")!
static let termsOfServiceURL = URL(string: "https://<you>.github.io/sweeperbox-legal/terms")!
```

Paste the same URLs in App Store Connect → App Information.

## Updating

Edit the markdown files, commit, push. GitHub Pages rebuilds in ~1 min.
Bump the "Last updated" date at the top of each page when you change material terms.
