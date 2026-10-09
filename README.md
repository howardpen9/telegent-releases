# Telegent · Downloads & feedback

Telegent adds an Agent discussion space beside your Telegram chats. Discuss an idea with its recent chat context, keep Agent history on your Mac, and share selected discussion snapshots through a browser link.

## Download Build 73

[**Download the Apple Silicon beta**](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.5)

| Version | Use |
| --- | --- |
| [Beta5 / Build73](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.5) | **Current friend beta — start here** |
| [Beta4 / Build70](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.4) | Previous beta, retained for rollback |

Older unpublished candidates are labeled **Archived draft**. Repository maintainers may see those drafts before published releases; friends see only the public versions. Share the Build73 link above to open the current version directly.

Choose `Telegent-0.1.0-beta.5-build73-macOS-arm64.zip`. Extract it, move Telegent.app to Applications, and open it. Quit an older Telegent before replacing it; keep your existing app data.

- Apple Silicon only. No Intel build.
- Build70 Telegram login and a real Agent reply were confirmed on an Apple Silicon Mac mini running macOS 26.2. Build73 includes new UI fixes with automated checks; installation and the complete updated flow still need friend testing. Earlier macOS versions remain unvalidated.
- Developer ID signed and Apple notarized. Checksums and the matching client source are attached to the release.

## Start using Agent Chat

1. Sign into your own Telegram account in Telegent.
2. For your first AI activation, open Intents → Settings → Continue with Telegram. Authorize the **same Telegram account** in the browser.
3. Open Agent Chat beside a conversation or create one in Intents. Send a question and wait for the reply.

Hosted AI is an invite beta: Howard must enable your verified numeric Telegram user ID. Native Telegram login alone does not grant AI access. No provider key or development server is required. Howard provides free beta access within service limits and pays model usage; whitelist entries are numeric ID strings, with a current maximum of 20 accounts. If activation says beta access is required, request enrollment; reinstalling will not enable access.

To find your numeric ID for enrollment, open the [Telegram identity check](https://consumer-ai-beta.up.railway.app/auth/telegram/login), authorize Telegram, and send the displayed ID to Howard. This check does not activate AI or read your chats.

First activation uses an additional browser authorization because the AI backend verifies Telegram identity independently. The activation credential is saved on your Mac; renewed authorization can be required after expiry, sign-out or an account change.

## Beta scope

Build 73 fixes Sidebar → Open in Intents navigation races, stale List search/pagination replies and missing index-error recovery. It preserves saved drafts and tabs when an index read fails, and improves Retry/status spacing. It includes Build70’s search hang, first-launch and Telegram Layer223 sync repairs. Mac mini login and Agent replies were confirmed on Build70; Build73’s full real-device flow remains part of this friend trial. QR scanning and +888 delivery need further checks; phone-number login is the current tested path. Cold-start timing, DM/topic context accuracy, continuation after restart and phone-recipient sharing remain part of the friend trial, rather than completed acceptance claims.

See the [10–15 minute friend test checklist](TESTING.md).

## Feedback

[Report a bug](https://github.com/howardpen9/telegent-releases/issues/new/choose). Include build 73, macOS version, steps, expected result and actual result. Public issues are visible to everyone: omit login codes, API keys and private conversation text. Use the repository's Security reporting options for vulnerabilities when available.

## Data and source

Agent history and manual Memories stay on your Mac. Hosted AI processes submitted questions, recent Agent history and included context through the configured provider. Cloud shares are selected snapshots readable by anyone with the link; they are separate from full-history or Memory synchronization.

See [Privacy](PRIVACY.md) and [Source availability](SOURCE.md). The release contains a separate **build73-source.tar.gz** with native changes, dependency sources/notices and build instructions. GitHub's automatic “Source code” archives contain this documentation repository only. A complete fresh standalone source build remains unverified; the published binary was built from the integrated native checkout.

Telegent derives from [TelegramSwift](https://github.com/overtake/TelegramSwift), with its [GNU GPL v2 license](LICENSE) preserved. It is an independent project, not an official Telegram release.
