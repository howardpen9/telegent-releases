# Telegent · Downloads & feedback

Telegent adds an Agent discussion space beside your Telegram chats. Discuss an idea with its recent chat context, keep Agent history on your Mac, and share selected discussion snapshots through a browser link.

## Download Build 70

[**Download the Apple Silicon beta**](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.4)

Choose `Telegent-0.1.0-beta.4-build70-macOS-arm64.zip`. Extract it, move Telegent.app to Applications, and open it. Quit an older Telegent before replacing it; keep your existing app data.

- Apple Silicon only. No Intel build.
- Confirmed on an Apple Silicon Mac mini running macOS 26.2: Telegram login and a real Agent reply. Earlier macOS versions are not yet validated.
- Developer ID signed and Apple notarized. Checksums and the matching client source are attached to the release.

## Start using Agent Chat

1. Sign into your own Telegram account in Telegent.
2. For your first AI activation, open Intents → Settings → Continue with Telegram. Authorize the **same Telegram account** in the browser.
3. Open Agent Chat beside a conversation or create one in Intents. Send a question and wait for the reply.

Hosted AI is an invite beta: Howard must enable your verified numeric Telegram user ID. Native Telegram login alone does not grant AI access. No provider key or development server is required. If activation says beta access is required, request enrollment; reinstalling will not enable access.

First activation uses an additional browser authorization because the AI backend verifies Telegram identity independently. The activation credential is saved on your Mac; renewed authorization can be required after expiry, sign-out or an account change.

## Beta scope

Build 70 fixes a search keyboard loop that could block sidebar rendering, and includes the earlier first-launch and Telegram Layer223 sync repairs. Mac mini login and Agent replies are confirmed. QR scanning and +888 delivery need further checks; phone-number login is the current tested path. Cold-start timing, DM/topic context accuracy, continuation after restart and phone-recipient sharing remain part of the friend trial, rather than completed acceptance claims.

## Feedback

[Report a bug](https://github.com/howardpen9/telegent-releases/issues/new/choose). Include build 70, macOS version, steps, expected result and actual result. Public issues are visible to everyone: omit login codes, API keys and private conversation text. Use the repository's Security reporting options for vulnerabilities when available.

## Data and source

Agent history and manual Memories stay on your Mac. Hosted AI processes submitted questions, recent Agent history and included context through the configured provider. Cloud shares are selected snapshots readable by anyone with the link; they are separate from full-history or Memory synchronization.

See [Privacy](PRIVACY.md) and [Source availability](SOURCE.md). The release contains a separate **build70-source.tar.gz** with native changes, dependency sources/notices and build instructions. GitHub's automatic “Source code” archives contain this documentation repository only. A complete fresh standalone source build remains unverified; the published binary was built from the integrated native checkout.

Telegent derives from [TelegramSwift](https://github.com/overtake/TelegramSwift), with its [GNU GPL v2 license](LICENSE) preserved. It is an independent project, not an official Telegram release.
