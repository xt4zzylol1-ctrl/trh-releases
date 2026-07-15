# TRH release automation

This repo-side automation lets Codex publish updates by changing `automation/release-request.json`
and `automation/release.patch` in `xt4zzylol1-ctrl/trh-releases`.

Required repository secrets in `xt4zzylol1-ctrl/trh-releases`:

- `TRH_PAT`: GitHub token with access to the private source repo and gist write access.
- `MAPS_API_KEY`
- `RELEASE_KEYSTORE_BASE64`
- `RELEASE_STORE_PASSWORD`
- `RELEASE_KEY_ALIAS`
- `RELEASE_KEY_PASSWORD`

The local script `setup-remote-publish.cmd` uploads this workflow and writes the secrets from the
current local project files.
