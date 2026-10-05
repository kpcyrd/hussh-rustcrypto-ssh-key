# [RustCrypto]: SSH [![Project Chat][chat-image]][chat-link] [![dependency status][deps-image]][deps-link]

Pure Rust implementation of components of the Secure Shell ([SSH]) protocol.

This is a fork of the RustCrypto SSH repository, with all dependencies of the
`ssh-key` crate updated to the latest RustCrypto ecosystem, and the RSA feature
removed (since that may still take some time).

Since the Debian-Rust tooling doesn't support RC versions, forking into a
different crate name and a non-RC version allows immediate upload, which in
turn would unblock a new upload of russh, which in turn would address the
following in Debian sid:

- CVE-2026-42189
- CVE-2026-46673
- CVE-2026-46702
- CVE-2026-46705
- CVE-2026-48107
- CVE-2026-48108
- CVE-2026-48110
- CVE-2026-68930
- CVE-2026-73429
- CVE-2026-73430
- CVE-2026-73489
- CVE-2026-102820
- CVE-2026-102821
- CVE-2026-102822
- CVE-2026-102823
- CVE-2026-102824
- CVE-2026-102825

## Crates

| Name           | crates.io                                                                                               | Docs                                                                                     | Description                                          |
|----------------|---------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------|------------------------------------------------------|
| `ssh‑cipher`   | [![crates.io](https://img.shields.io/crates/v/ssh-cipher.svg)](https://crates.io/crates/ssh-cipher)     | [![Documentation](https://docs.rs/ssh-cipher/badge.svg)](https://docs.rs/ssh-cipher)     | SSH symmetric encryption ciphers                     |
| `ssh‑derive`   | [![crates.io](https://img.shields.io/crates/v/ssh-derive.svg)](https://crates.io/crates/ssh-derive)     | [![Documentation](https://docs.rs/ssh-derive/badge.svg)](https://docs.rs/ssh-derive)     | Custom derive support for `ssh-encoding`             |
| `ssh‑encoding` | [![crates.io](https://img.shields.io/crates/v/ssh-encoding.svg)](https://crates.io/crates/ssh-encoding) | [![Documentation](https://docs.rs/ssh-encoding/badge.svg)](https://docs.rs/ssh-encoding) | Decoders and encoders for SSH protocol data types    |
| `ssh‑key`      | [![crates.io](https://img.shields.io/crates/v/ssh-key.svg)](https://crates.io/crates/ssh-key)           | [![Documentation](https://docs.rs/ssh-key/badge.svg)](https://docs.rs/ssh-key)           | SSH key and certificate library with signing support |
| `ssh‑protocol` | [![crates.io](https://img.shields.io/crates/v/ssh-protocol.svg)](https://crates.io/crates/ssh-protocol) | [![Documentation](https://docs.rs/ssh-protocol/badge.svg)](https://docs.rs/ssh-protocol) | SSH protocol implementation (WIP)                    |

## License

All crates licensed under either of

- [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
- [MIT license](http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.

[//]: # "badges"
[chat-image]: https://img.shields.io/badge/zulip-join_chat-blue.svg
[chat-link]: https://rustcrypto.zulipchat.com/#narrow/stream/346919-SSH
[deps-image]: https://deps.rs/repo/github/RustCrypto/SSH/status.svg
[deps-link]: https://deps.rs/repo/github/RustCrypto/SSH

[//]: # "links"
[RustCrypto]: https://github.com/RustCrypto/
[SSH]: https://en.wikipedia.org/wiki/Secure_Shell
