# Minecraft Plugin Release Checklist

A compact, auditable release gate for Paper, Bukkit, and Velocity plugins. Tailor required checks to the plugin and publish tested version support honestly.

## Before tagging
- Confirm the release branch is clean and the version/changelog are updated.
- Run formatting, unit tests, integration tests, and the documented verification script.
- Build against the declared Java and server API versions.
- Review dependency licenses and known advisories.
- Test fresh installation, upgrade/config migration, startup, shutdown, and rollback.
- Inspect the packaged artifact for secrets, debug files, and unintended dependencies.

## Publishing
- Use a protected, signed or otherwise controlled tag process.
- Publish artifact checksum and provenance with release notes.
- Grant write permissions only to the release publishing job.
- Preserve the previous known-good artifact and state the rollback path.

A checklist records process completion; it does not replace technical review.