# Telegent Build74 friend test

Allow about 10–15 minutes. Automated navigation, history/retry, Sidebar feedback, AppKit composer/IME and Release isolation/startup checks passed; actual installation and product behavior must be recorded separately. Build70’s Mac mini login/reply checkpoint does not establish Build74 acceptance. Context-state/source tests likewise do not prove a private Topic cache is readable.

## Friend flow (about 10–15 minutes)

1. Install the build from its GitHub release, open it and sign into Telegram. Record build/macOS/Apple Silicon chip, time until the chat list appears, and any persistent Connecting/Updating state.
2. Ask Howard to enroll your numeric Telegram user ID. Open **Intents → Settings → Continue with Telegram**, authorize the same account once, create an Agent Chat and confirm a complete reply. Whitelist enrollment does not replace this current activation step.
3. Open Agent Sidebar from a DM or group/topic. Check the exact source/Topic title and context status. Try Last 24 hours, Last 7 days and a valid custom interval, then Review and exclude a self-authored test message. Ask about harmless content from that exact source. Confirm unavailable context shows its reason and an unchecked control; Refresh retries, ordinary attachment Send retains the draft, and explicit Question only disables attachment without sending. Do not interpret the source label alone as proof of imported content.
4. Type a multiline English/繁體中文 draft, resize Sidebar, expand with **Open in Intents**, check the same conversation/source, and return. Test List search/clear/scroll and reopen the App to check the saved draft/history and continuation.
5. Share one self-authored conversation with only the selected test context. On a phone, verify the friend can read/copy it without installing Telegent, then revoke it and check that the link no longer reads.

Record each item as PASS, FAIL or NOT RUN. Report failures through the [GitHub issue form](https://github.com/howardpen9/telegent-releases/issues/new/choose) with build, OS and exact reproduction steps; omit private messages, authentication codes and keys. QR/+888 login, real Apple 注音 typing, source/topic accuracy, reopen continuation, cold-start timings and recipient-phone sharing remain distinct real-device checks.

## Beta access

The current consumer service reads `TELEGENT_ALLOWED_TELEGRAM_IDS` as a JSON array of **strings**, for example `["123456789","987654321"]`; usernames and phone numbers are not IDs. Empty `[]` enables no account. The current implementation accepts at most 20 entries. An unenrolled account can use native Telegram but cannot activate hosted AI. Removing an ID denies subsequent authenticated requests. Railway applies new environment variables through its deployment lifecycle; verify the new deployment succeeds before asking the friend to retry activation.

Friends do not supply a provider key or run a backend. Howard pays provider usage within the configured beta budgets; “free testing” describes the friend's access. Agent history, continuation state and Memories stay on the Mac. Cloud sharing publishes an explicitly selected snapshot; it does not synchronize every local conversation.
