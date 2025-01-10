# [kwak](https://kwak.tech)
kwak is an Elys Governor, and an team of passionate blochain/defi users!

## [Elys Scan](https://elysscan.io)
Elys Scan is our (Soon to be OSS) Elys dedicated block explorer.
Elys Scan is an advanced tool that that not only indexes transactions, but events. Transactions include Swaps (Market Orders), Adding Liquidity, Staking, etc.
Event's can include when Swaps execute (E.g Limit buys), Liquidiations, Take Profit, etc. *Most* On and Offchain things.

All powered by our

## Elys Indexer
Our Elys inexer (Soon to be OSS) is a modified node that hooks into every message handler to ensure it logs all relevant data to the transaction or event especially in a human readable format.
All data is logged by an [LMDB](https://en.wikipedia.org/wiki/Lightning_Memory-Mapped_Database) database, and provided by a gRPC server to ensure quick and reliable transmission of TXs to the user.

## Private Services
We also do private things for chains/teams, here is some of our work for Elys.
- [Multisig wallet management utilizing Keplr, and an intuitive UI.](https://drive.google.com/file/d/1cNvlfGYoX-KCutE2nIIL-Yi5q4iaYAWj/view?usp=sharing)
  - Allows for Multisigs to be added and their partcipants, as well as signing ratio.
  - Users to upload custom TXs to be signed by the multisig participants
  - When users sign in with Keplr it auto detects the multisig's they're apart of and shows the TXs they can sign on.
  - When the signing ratio is hit, users can broadcast the TX to the network via a button.
- [Price tickers powered by the Coingecko API.](https://drive.google.com/file/d/12BCykmORoeU_qIdbOhiKNjS9geR_Fo42/view?usp=sharing)
- We've made Discord Bots the past that allow users to submit wallet addresses for team review, via a button and modal and shown in an intuitve CSV format. (No image exammples)

## [Nexus](https://github.com/kwak-labs/Nexus)
Nexus is a discord cosmos based tipping bot, all actions are done on-chain. When users first use the bot it generates a custom seed phrase, and connects it to that user.

## [kwak Pot](https://github.com/kwak-labs/kwakpot)
kwak Pot is an cosmos/Elys based lottery where users can purchase tickets and the tickets they purchase get sent into the total pot for that game.
The game isnt smart contract based, but the game results are *cryptographically* secure. It uses the ending block of the lotto's block hash as a seed for the deterministic shuffle of tickets using [Fisher-Yates](https://en.wikipedia.org/wiki/Fisher%E2%80%93Yates_shuffle) shuffle algorithim. Users can verify the games legitness by replaying all the TXs that bough tickets, and putting it through the same algorithim.
