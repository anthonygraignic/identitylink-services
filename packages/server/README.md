<h1 align="center">Welcome to 3box-verifications-v2 server 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000" />
  <a href="#" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" />
  </a>
  <a href="https://twitter.com/pi0neerpat" target="_blank">
    <img alt="Twitter: pi0neerpat" src="https://img.shields.io/twitter/follow/pi0neerpat.svg?style=social" />
  </a>
</p>

<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->

[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)

<!-- ALL-CONTRIBUTORS-BADGE:END -->

> A decentralized identifier (DID) verification service for 3Box. Available methods include Twitter, Discord, and Github.

## Install

```sh
yarn install
```

Copy `.template.env` to `.env` and update the variables. You'll need the following:

- `VERIFICATION_ISSUER_DOMAIN` - The issuer domain for the claim. For example, if you enter `verifications.3box.io`, the claim issuer will be `did:web:verifications.3box.io`.
- Public/private keys for your `did-jwt` signer
- Twitter developer tokens
- Github API token
- Redis database URL
- (optional) Segment token

## Test

Run jest

```bash
yarn test
```

You can also test against real-world data. You will need a recent (<30m) Tweet & Gist containing a `did`. See `/test-examples` for a real-world data test suite and other useful scripts.

```bash
sls offline --host 0.0.0.0
```

## Deploy

```bash
# Load your AWS credentials first
sls deploy
```

## Author

👤 **Patrick Gallagher**

- Website: https://patrickgallagher.dev
  - Twitter: [@pi0neerpat](https://twitter.com/pi0neerpat)
  - GitHub: [@pi0neerpat](https://github.com/pi0neerpat)

## Show your support

Give a ⭐️ if this project helped you!

---

_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_