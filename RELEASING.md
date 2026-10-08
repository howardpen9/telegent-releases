# Maintainer release procedure

1. Prepare one Apple Silicon installer; verify Developer ID, Hardened Runtime, secure timestamp, Apple acceptance, stapling and Gatekeeper on the actual package. Record version, build and SHA-256.
2. Assemble and verify the corresponding modified client source, dependency notices and build instructions. Do not substitute the automatic archive of this documentation repository.
3. Verify installation on a clean Apple Silicon Mac, Telegram login with the client's own API identity, enabled-account AI activation and replies, context controls and sharing/recipient reading. Document remaining beta limitations honestly.
4. Create a draft prerelease and attach the installer, corresponding source and `SHA256SUMS`. Keep binaries as release assets rather than Git commits. Review the complete draft before publication.
5. Publish only when the source and product acceptance gates pass. Update the README with the actual tested macOS versions, download link and onboarding steps. Keep Issues open for reports.

Installer or source changes require new hashes and the appropriate checks. Never silently replace a previously accepted installer with a different build.

The documentation repository can be public while a prerelease remains a draft. A draft is not a public download, and its existence does not mean release acceptance has passed.
