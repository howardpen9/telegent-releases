# Beta data handling

## On your Mac

Telegram login sessions, Agent conversation history and manual Memories remain on your Mac. Full-history and Memory cloud synchronization are not part of the first beta. Memories are not automatically extracted or attached to every question.

## AI requests

Questions sent to the hosted Agent are processed by the Telegent service and its configured model provider. Requests may include recent Agent discussion and the Telegram context you include. The context control lets you omit the loaded context from a request.

Current chat import is bounded: recent text from the current room or Topic, normally the last 24 hours, capped at 50 messages and 16 KiB. Cache coverage and content protection can limit availability; an unavailable or partial state is not a guarantee of complete history.

The service retains authentication, quota and request-status metadata. AI continuation content is returned to and held on the Mac; this is not a cloud backup of your conversations. Local storage does not mean AI inference happens locally.

## Sharing

Sharing publishes a snapshot of the discussion and contexts you selected. Anyone with the resulting link can read the snapshot without installing Telegent. Only share content you intend those readers to see. Existing copies made by a recipient are outside the share service's control.

The current hosted service supports bounded-expiry snapshots and owner-authenticated revocation. End-to-end native and phone acceptance is required before the first public beta.

## Public support

GitHub Issues are public. Reproduce problems using invented sample text where possible. Remove private messages, account details, access tokens and login codes from screenshots or reports.
