# Telegent · Downloads & feedback

Telegent adds an Agent discussion space beside your Telegram chats. Discuss an idea with its recent chat context, keep Agent history on your Mac, and share selected discussion snapshots through a browser link.

## Download Build 74 · Beta 6

[**Download the Apple Silicon beta**](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.6)

| Version | Use |
| --- | --- |
| [Beta6 / Build74](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.6) | **Current friend beta — start here** |
| [Beta5.1 / Build73](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.5.1) | Previous beta with repaired installer |
| [Beta5 / Build73](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.5) | Superseded ZIP packaging; use Beta5.1 for installation |
| [Beta4 / Build70](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.4) | Previous beta, retained for rollback |

Older unpublished candidates are labeled **Archived draft**. Repository maintainers may see those drafts before published releases; friends see only the public versions. Share the Build74 link above to open the current version directly.

Choose `Telegent-0.1.0-beta.6-build74-macOS-arm64.zip`. Extract it, move Telegent.app to Applications, and open it. Quit an older Telegent before replacing it; keep your existing app data.

- Apple Silicon only. No Intel build.
- Build70 Telegram login and a real Agent reply were confirmed on an Apple Silicon Mac mini running macOS 26.2. Build74 has automated source/UI checks and an integrated arm64 Release build; its complete real-device flow still needs friend testing. Earlier macOS versions remain unvalidated.
- Developer ID signed and Apple notarized. ZIP integrity and signed-bundle contents are verified. Normal-browser first-open on the affected macOS 15.6.1 recipient remains pending. Use the checksums and corresponding source/notices on the release page.

## Start using Agent Chat

1. Sign into your own Telegram account in Telegent.
2. For your first AI activation, open Intents → Settings → Continue with Telegram. Authorize the **same Telegram account** in the browser.
3. Open Agent Chat beside a conversation or create one in Intents. Send a question and wait for the reply.

Hosted AI is an invite beta: Howard must enable your verified numeric Telegram user ID. Native Telegram login alone does not grant AI access. No provider key or development server is required. Howard provides free beta access within service limits and pays model usage; whitelist entries are numeric ID strings, with a current maximum of 20 accounts. If activation says beta access is required, request enrollment; reinstalling will not enable access.

To find your numeric ID for enrollment, open the [Telegram identity check](https://consumer-ai-beta.up.railway.app/auth/telegram/login), authorize Telegram, and send the displayed ID to Howard. This check does not activate AI or read your chats.

First activation uses an additional browser authorization because the AI backend verifies Telegram identity independently. The activation credential is saved on your Mac; renewed authorization can be required after expiry, sign-out or an account change.

## Beta scope

Build74 adds context intervals per Agent conversation: Last 24 hours, Last 7 days, or a custom interval up to 7 days, plus Review exclusions and defaults. Unavailable previews appear unchecked; Send retains the reason and draft, stalled reads/privacy checks time out, and Refresh retries. Question only explicitly disables attachment without sending, including through context-settings recovery. It includes prior sidebar history, reading-position, source-navigation, search/index, first-launch and Telegram Layer223 sync repairs.

Context reads eligible local cached text only, capped at 50 messages / 16 KiB. Protected/service/unknown sources, cache gaps and All Topics may have no usable context; this build adds no full-history fetch or parent-Topic fallback. The reported private Topic cache cause remains unproven. Backend prompt/policy changes are not deployed by this client release. QR/+888 login, source accuracy, continuation after restart, cold-start timing and phone-recipient sharing remain part of the friend trial.

See the [10–15 minute friend test checklist](TESTING.md).

## Feedback

[Report a bug](https://github.com/howardpen9/telegent-releases/issues/new/choose). Include build 74, macOS version, steps, expected result and actual result. Public issues are visible to everyone: omit login codes, API keys and private conversation text. Use the repository's Security reporting options for vulnerabilities when available.

## Data and source

Agent history and manual Memories stay on your Mac. Hosted AI processes submitted questions, recent Agent history and included context through the configured provider. Cloud shares are selected snapshots readable by anyone with the link; they are separate from full-history or Memory synchronization.

See [Privacy](PRIVACY.md) and [Source availability](SOURCE.md). The [Beta6 release](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.6) contains the separate **Telegent-0.1.0-beta.6-build74-source.tar.gz** with native changes, dependency sources/notices and build instructions. GitHub's automatic “Source code” archives contain this documentation repository only. A complete fresh standalone source build remains unverified; the published binary was built from the integrated native checkout.

Telegent derives from [TelegramSwift](https://github.com/overtake/TelegramSwift), with its [GNU GPL v2 license](LICENSE) preserved. It is an independent project, not an official Telegram release.
