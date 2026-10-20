# BearSSL (bitpart-xyz import)

An unmodified import of upstream BearSSL by Thomas Pornin, https://www.bearssl.org/git/BearSSL
(browse: https://www.bearssl.org/gitweb/?p=BearSSL;a=summary). License: MIT, see `LICENSE.txt` on `master`.

- `master` and the `v*` tags are exact copies of upstream. Nothing here is modified.
- This `sync` branch holds only the import workflow (`.github/workflows/sync.yml`). Every Monday it fetches
  upstream, pushes new commits and tags fast-forward only, and opens an issue listing what arrived. If upstream
  ever rewrites history or moves a tag, the job fails instead of overwriting.
- Consumers pin a commit; nothing moves a pin automatically.
