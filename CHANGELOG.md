# Neon Release Notes

## neon_phone 1.1.1-neon.2 - 2026-10-03

- Use the Stars & Stripes Mods public version feed instead of the upstream
  GitHub release endpoint.
- Retry temporary HTTP failures with a bounded backoff and request timeout.
- Report unavailable checks separately from a confirmed current version.
- Compare Neon revision suffixes and ignore build metadata correctly.
- Allow an explicit server-console recheck with `neonphoneupdate`.
- Keep update checking separate from package installation.

This is an update-checker patch to the existing Neon Phone integration, not a
new upstream phone release or an announcement about other Neon components.
