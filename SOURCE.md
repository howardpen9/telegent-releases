# Source availability

Telegent modifies the GPL v2 TelegramSwift macOS client. A separate downloads repository does not remove the requirement to make the distributed client's corresponding source available.

Each published binary release will include a clearly identified corresponding source bundle, dependency notices and build instructions. The source must match that particular binary's native changes and compilation inputs, including needed generated sources and build/staging scripts.

Current status: the first candidate is signed and notarized; the complete source bundle and reproduction checks are being prepared. No public application binary has been published in this repository.

This repository contains public release and support documentation. Its automatic GitHub source archives are not the full application source. The existing development repository is separate and is not exposed by creating this repository.

Private credentials, signing keys, Telegram sessions and user data are excluded from source bundles. Developers supply their own Telegram API configuration and signing credentials to build their own client. Hosted AI provider keys remain on the service.

Upstream base: [TelegramSwift, commit 579cebbf0c01fd41b712eff3647fa7f69db9665d](https://github.com/overtake/TelegramSwift/tree/579cebbf0c01fd41b712eff3647fa7f69db9665d).

The pinned upstream base is provenance, not a substitute for the complete modified source. See the preserved [GPL v2 license](LICENSE), especially section 3.
