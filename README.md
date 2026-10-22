# sovereign-apps

Curated catalog of root-requiring Android apps for the Sovereign
toolkit's Root App Store — read by the app from `apps.json` in this
repo.

## Rules

- **Links and metadata only.** This repo never hosts APK files.
- Every free entry points at the developer's **official** release
  (their GitHub releases or official site). No mirrors, ever.
- `sha256` and `cert_sha256` are recorded only after the exact
  official APK has been downloaded by Sovereign's maintainer and
  hashed locally. They are never copied from a blog, a mirror, or a
  third-party listing.
- An entry without both hashes is locked in the app
  ("verification pending") and cannot be installed.
- Paid apps appear as Play link-outs only. Sovereign never downloads,
  hosts, or redistributes them.
- At install time the app re-checks both hashes; any mismatch stops
  the install and deletes the downloaded file.

## Entry format

See `apps.json`: name, package, developer, license, version,
source_url, apk_url, sha256, cert_sha256, root_note, paid.
