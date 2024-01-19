# Star Notary

<p>
An NFT Marketplace for registering, naming, and trading Stars!
</p>

## Showcase:

[![Star Notary Showcase](https://img.youtube.com/vi/ZsvL5tF50P4/0.jpg)](https://www.youtube.com/watch?v=ZsvL5tF50P4)

## Architecture:

<img src="public/architecture.png" alt="architecture">

#### Ethereum

<p>
Chosen blockchain infrastructure for the Star Notary Smart Contract!
</p>

#### RPC Provider

<p>
Provides communication to the Blockchain, Infura is a good example
</p>

#### Star Notary Listener

<p>
Listens for smart contract events, confirms the event using the provided confirmation blocks (default is 12), consumes the Star Notary API after confirmation
</p>

#### Star Notary API

<p>
Creates, updates, and queries database for star NFTs, publishes all updated stars to the websocket endpoint
</p>

#### Client

<p>
User facing web-app. Integrates with Metamask, calls contract transactions for changes in star NFT state, calls contract view functions to improve user feedback in between confirmations, queries Star Notary API
</p>
