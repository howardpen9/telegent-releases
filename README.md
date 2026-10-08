# Telegent · Releases & feedback

Telegent is a macOS Telegram client with a private Agent discussion space. Discuss an idea beside a chat, choose its background, and share the discussion and context you want someone else to understand.

This repository is the public home for downloads, release notes and feedback.

## Download status

**The first Apple Silicon beta is being prepared. No public installer is available yet.**

The candidate has passed Developer ID signing and Apple notarization. Corresponding source preparation and clean-device onboarding, Agent replies and sharing acceptance are still pending. Notarization alone does not verify those product flows.

Published installers will appear on the [Releases page](https://github.com/howardpen9/telegent-releases/releases). GitHub's automatically generated “Source code” archives contain this repository's documentation; they are not the Telegent installer or the complete application source.

## First beta

- Apple Silicon Macs only. Intel is not supported in this first beta.
- The supported macOS versions will be stated after device acceptance.
- Sign in with your Telegram account. First AI activation currently also requires Telegram authorization in a browser.
- Hosted AI access is limited to enabled beta accounts. A successful Telegram login does not automatically enable AI access.
- No personal AI provider key or local development server is required for the hosted beta.

## Feedback

[Report a bug](https://github.com/howardpen9/telegent-releases/issues/new/choose) or suggest an improvement through Issues. Include the app build, macOS version, the steps you took and what you expected.

Public issues are visible to everyone. Do not attach API keys, login codes, private messages or unredacted screenshots. For vulnerabilities, use private reporting from the repository's [Security tab](https://github.com/howardpen9/telegent-releases/security), once available.

## Data and source

Agent history and manual Memories are stored on your Mac. Hosted AI processes your submitted question, recent Agent history and any included context through the AI service and its configured provider. Shared links contain the snapshots you choose to publish; anyone with the link can read them. Cloud sharing is separate from full-history or Memory synchronization.

See [Privacy](PRIVACY.md) and [Source availability](SOURCE.md). Telegent is derived from [TelegramSwift](https://github.com/overtake/TelegramSwift) under the [GNU GPL version 2](LICENSE). Each published binary release must provide its corresponding client source and required notices.

Telegent is an independent project, not an official Telegram release.
