# Neon Updates

Public version metadata and release notes for Stars & Stripes Mods components.
This repository contains no framework source, paid assets, credentials, player
data or production configuration. The framework source repository is private.

## Feed

`latest.json` is the canonical version feed. Each component has an independent
version; a phone release does not announce an update to the entire framework.

Feed URL:
https://raw.githubusercontent.com/starsstripesmods-dev/neon-updates/main/latest.json

Schema version 1 requires a `components` object containing named components
with a `version` string. Versions follow [Semantic Versioning](https://semver.org/).
Existing Neon revision suffixes are compared, not discarded.

## Publishing

1. Test and package the component privately.
2. Assign a new component version and document it in `CHANGELOG.md`.
3. Deploy the tested package and publish its version in `latest.json`.
4. Verify the feed and the server's update-check output.

Only names, versions and release notes belong here. Review every public commit.
Never upload archives, source, server.cfg, .env, API tokens or database exports.

This feed reports update availability. It does not download or install code,
grant access to private packages, or replace a release backup.
