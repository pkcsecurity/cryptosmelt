# Cryptosmelt

## For the Libra Folks

Greetings. Joshua Maddux is a Security Developer at PKC. We've added his project here so it's together with the other projects. He's talking at Blackhat and DefCon this year, so, if you see him, say "Hi."

Cryptonote and Cryptonote-Lite pool software, written in Rust and using Postgres as the data store.
Currently cryptosmelt is round-based-pay-per-share only, but there are plans to include other reward mechanisms,
particularly PPLNS, in the future.

# Dependencies

- Rust (nightly version)
- Postgres 9.5 or later

# Installation

Install the Rust nightly version. This is easiest to do via [rustup](https://www.rustup.rs/):

```
curl https://sh.rustup.rs -sSf | sh
rustup install nightly
```

_Nightly is needed because of the dependency upon [mithril's](https://github.com/Ragnaroek/mithril) Cryptonight hash implementation._

Then checkout this repo and enter your pool wallet address as `pool_wallet` in `config.toml`. Then execute `cargo run` and the server will listen on the ports configured in that file.

# Recommended tools

- Intellij has a Rust plugin that is already excellent: https://intellij-rust.github.io
