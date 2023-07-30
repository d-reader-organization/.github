# Encode hackathon submission

During the hackathon we've:
- deployed [dReader web app](https://dreader.app)
- published [dReader mobile app](https://play.google.com/store/apps/details?id=io.app.dreader) on google play
- finished [dPublisher Smart Contract](https://github.com/d-reader-organization/d-reader-comic-verse)
- partially built the [dPublisher web app](https://drive.google.com/file/d/1XSduUUTdQul6lO3E6wzjLzw5xa4O_n-L/view)
- finished remaining dPublisher backend functionalities

> **Note** 
> To learn more about dPublisher & dReader visit repositories on [README.md](https://github.com/d-reader-organization/.github/blob/main/profile/README.md) specification

## Solana Foundation: Best Consumer Application
> An application that is a consumer-first product that anyone, even people outside of crypto, can use.

This is still work in progress but... in a matter of ~2 weeks dPublisher & dReader will finish it's migration to being consumer-first.

As for **dReader**:
- Readers will be able to download the app and use it without even having a wallet. How?
- We're offering "free to read" content on the platform. No need to connect a wallet if you just want to read free comics
- Users that want to collect comics and care about digital ownership will be prompted to (install and) connect a wallet app.
- In Q4 2023 we'll integrate session keys so users don't have to sign each and every minor transaction (e.g. when opening comics)
- In 2024 we'll implement monthly subscriptions (via visa). No need to connect a wallet if you don't want to own the digital content

As for **dPublisher**:
- Creators can choose to self-publish a comic without any prior crypto knowledge
- For now, if they're not willing to use a digital wallet, we will generate a keypair for them and off-ramp crypto to their fiat account manually. Cost of the Candy Machine and transacting (e.g. signing digital comics to fans) is paid by us.
- In the future, crypto off-ramp will be automatic

## Solana Foundation: Most innovative Application
> An innovative or unexpected application that doesn’t fit in the other categories, but is a clear winner nonetheless.

dPublisher and dReader projects are innovative in a way that they're focused on a comic niche.
It's the first digital app for comic collecting in which:
- users have self-custody
- users can unwrap their comics and have them signed
- comic pages are published on arweave and encrypted, only NFT owner can decrypt them
- users can engage with creators via DMs
- creators can self-publish digital collectible comics

## Phantom Bounty
> Create a dApp which makes use of durable nonces!

For the purpose of the hackathon we've built a POC/MVP which is explained better in the [durable nonces demo video](https://drive.google.com/file/d/13D8DFU3Zps5K89JaiOnNuiY7Lvr7vxQ6/view?usp=sharing) recorded by Athar.

Code base can be found at the `durable-nonces-mvp` branch: [https://github.com/d-reader-organization/d-reader-backend/tree/durable-nonces-mvp](https://github.com/d-reader-organization/d-reader-backend/tree/durable-nonces-mvp)

Our MVP uses durable nonces for:
- buying NFTs on primary sales -> high volume mints should be handled better by marketplaces by relying more on durable nonces
- sending many transactions (e.g. buying multiple NFTs on secondary) -> when trying to buy 50 NFTs some transactions are bound to fail, this effect can be negated

We're looking to expand our usage of durable nonces with:
- co-signing comics -> multiple creators will be able to sign a comic and this would require a transaction with no expiry so an async multi-sig can be possible
- P2P trading -> exchange comic A for a comic B with another user by signing a transaction with no expiry. When the other user signs the transaction, it's executed
- Comic gifting -> gift a comic to someone instead of airdropping it to their wallet. This way the gift recipient can choose to explicitly accept or reject it rather than just having it dropped in their wallet. Again, wallet A signs a transaction with no expiry and wallet B is asked to sign it

## Elusiv Bounty
> Build an MVP with the Elusiv SDK for a new or existing application.

Elusiv MVP code base can be found at the `elusiv-mvp` branch: [https://github.com/d-reader-organization/d-reader-frontend/tree/elusiv-mvp](https://github.com/d-reader-organization/d-reader-frontend/tree/elusiv-mvp)
But best to read the solution explanation at [elusiv-mvp.pdf](https://drive.google.com/file/d/1XdbnCNnVLAVHUiwPGIjuleOcjBR3bey4/view?usp=sharing)

Our MVP uses Elusiv nonces for tipping artists anonymously. In the future we would like to expand and explore the following options:
- anonymous transactions on our Comic NFT marketplace
- anonymous P2P comic NFT swaps
- private payments for contract/commission work
- private crypto off ramps
- private royalty share

## Full disclaimer:

**We've previously won hackathons with dReader**. Hence why our focus for this Encode hackathon was on dPublisher (backend CRUDs, web app, smart contract) and shipping new features on dReader (web app, comic signing, comic unwrapping...)