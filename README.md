# go-puppet.github.io

The Hugo landing page for **[go-puppet](https://github.com/go-puppet)** — a
pure-Go implementation of the Puppet language. Served at
<https://go-puppet.github.io>.

Built with Hugo (extended) and deployed to GitHub Pages by the
`deploy-pages` workflow (Pages source: GitHub Actions). The page ships a
light/dark/system theme toggle (default: system).

```sh
hugo server   # local preview at http://localhost:1313
```

BSD-3-Clause.

## The design is not here

It comes from the shared Hugo module
[`go-fleettools/landingkit`](https://github.com/go-fleettools/landingkit),
pinned in `go.mod` (Renovate bumps it); `kit.go` keeps `go mod tidy` from
deleting that requirement. `[params.brand]` in `hugo.toml` is read from the logo by
`landingkit brand`. A file under `layouts/partials/` with the name of one of the
kit's would silently override it.
