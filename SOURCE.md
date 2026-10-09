# Build 73 source availability

[Release v0.1.0-beta.5](https://github.com/howardpen9/telegent-releases/releases/tag/v0.1.0-beta.5) provides the installer and `Telegent-0.1.0-beta.5-build73-source.tar.gz` separately. SHA256SUMS covers both archives.

Acceptance flags inside the source manifest refer to full fresh-build/product acceptance at packaging time; they do not describe whether this limited beta download is public.

The source archive contains the modified native client, 30 initialized native module snapshots, generated Swift/header inputs, pinned dependency source, SwiftPM source checkouts, the approved Telegent icon, build/staging/signing support, and original license/notice texts. SOURCE_MANIFEST.json binds individual files to build 73 and its installer digest. BUILD.md describes the toolchain, native dependency recipes, compilation, staging and reproduction limits; THIRD_PARTY_NOTICES.md indexes retained notices, with a component map in support/SHIPPED_COMPONENTS.md.

The maintainer independently verified all archive members and their content/modes/links against the manifest and checked the 38,028 frozen native compilation inputs. The binary passed an integrated arm64 Release build. **A complete fresh build from the standalone archive has not yet been accepted.** Legacy dependency bootstrapping still needs work; this is not a claim of a byte-identical or one-command reproducible signed installer. Please report missing inputs or build failures through Issues.

GitHub's automatic “Source code” archives contain this distribution repository's documentation, not the complete native client. The separate development repository and its Git history are not published through this snapshot.

Private credentials, signing keys, Telegram sessions and user data are excluded. Developers supply their own Telegram API identity and signing credentials for a separate distribution. Hosted AI provider keys remain on the service; the hosted backend is separate from the native source archive.

Upstream native base: [TelegramSwift 579cebbf0c01fd41b712eff3647fa7f69db9665d](https://github.com/overtake/TelegramSwift/tree/579cebbf0c01fd41b712eff3647fa7f69db9665d). The Layer223 repair follows Telegram-iOS revision 189d25c32e1d9b44a4cf606291eb241491016115. Exact source-module commits are recorded in SOURCE_MANIFEST.json. The upstream base alone does not replace the modified source. Original [GNU GPL v2](LICENSE) and dependency terms are preserved.
