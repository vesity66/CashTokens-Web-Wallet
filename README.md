# [CashTokens Web Wallet](https://wallet.mycashtokens.org/)
Official CashTokens Web Wallet (BitcoinCash Network) - [wallet.mycashtokens.org](https://wallet.mycashtokens.org/)

![CashTokens](https://i.ibb.co/GCSZbRx/asda2-cleaned.jpg)

- CashTokens are a built-in, optional feature of the [Bitcoin Cash network](https://bch.network). 

This is the code repository for [My CashTokens Webwallet](https://wallet.mycashtokens.org/), a webwallet with CashTokens support for chipnet.
It is built with the mainnet-js library.
It started in early January as a minimum viable product but has grown into a full-fledged webwallet.
The webwallet will move to mainnet after the CashTokens upgrade on May 15th.
The project has proven helpful to iron out issues, bugs and missing features in the mainnet-js library.

#### Details
The Webwallet creates a single address chipnet wallet which is persisted in between sessions in indexedDb.
The Webwallet uses m/44'/0'/0'/0/0 as derivation path for seedphrases, this is the mainnet-js default.
You can back-up the wallet by getting the seed phrase from the settings view.
The webwallet uses example_bcmr as a hardcoded metadata registry for tokenmetadata.
After making a transaction a link to a chipnet blockexplorer is logged in the console (press F12 to access).

#### Faucet
To get started with the webwallet and create your own CashTokens on chipnet, get a tBCH balance from the chipnet faucet!

#### Planned features
You can find the planned features on the issues page on GitHub.
Feel free to open a new issue to report bugs or suggest improvements!
Currently not planning on adding transaction history to the webwallet.

#### How it was made
The project was started with the help of this getting-started blogpost for mainnet-js.
Since the way to import it had been changes with version 1.0.0 as can be read on its github release page.
Chota as a styling library and Switchery for toggle switches.
For icons the webwallet uses icongr.am.
blockies is used to generate blocky identicons for tokens.
The chaingraph demo instance is used to query on-chain tokeen info about gensis supply and minting UTXOs.
Finally, bitjson/qr-code is used to generate the qr-codes.

Netlify automatically publishes the latest version of this repo: My CashTokens Webwallet.

#### Special thanks to
bitcoincashautist, pat from mainnet-js, damascene & bitjson
