# Tech Implementation
> Tech stack and implementation details

**Open Source** is deeply engraved in dReader as a core value and as such, our repositories are always publicly available!

> **Warning**
> **Encode hackathon judges: please also refer to the additional specification at [ENCODE_README.md](./d-reader-organization/.github/blob/main/profile/ENCODE_README.md) document**

### [d-reader-backend](https://github.com/d-reader-organization/d-reader-backend)
> NestJS, TypeScript, Prisma, PostgreSQL, web3.js, metaplex.js

🏗️ Server service for dReader & dPublisher applications

Metaplex Auction House and Candy Machine programs are a foundation to our marketplace as our business logic is deeply integrated with them.

- link: https://api-main-mainnet.dreader.io/api
---

### [d-reader-frontend](https://github.com/d-reader-organization/d-reader-frontend)
> Next.js, TypeScript, React Query, MUI, web3.js

📖 Client application for dReader project

Web interface for seamless discovering, trading, collecting, and reading of digital graphic novels

- link: https://dreader.app

### [d-publisher-frontend](https://github.com/d-reader-organization/d-publisher-frontend)
> Next.js, TypeScript, React Query, MUI, web3.js

📖 Client application for dPublisher project

Web interface for seamless digital comic publishing, analytics tracking, and audience capturing

- link: https://dpublisher.app (coming soon)


---

### [d-reader-landing](https://github.com/d-reader-organization/d-reader-landing)
> Next.js, TypeScript

🔖 Promotional landing page for dReader project

- link: https://dreader.io

---

### [d-reader-mobile](https://github.com/d-reader-organization/d-reader-flutter)
> Flutter

📱 Android application for dReader project

Mobile app for seamless discovering, trading, collecting, and reading of digital graphic novels. Published on Solana dApp store and Google Play store

- link: https://play.google.com/store/apps/details?id=io.app.dreader

---

### [d-reader-comic-verse](https://github.com/d-reader-organization/d-reader-comic-verse)
> Rust, Anchor, Metaplex

‍🫴 Solana Program - standard for dReader digital comics

Comic Verse imposes a standard for signing, using and updating comic NFTs. Comic authors can sign copies, owners can 'unwrap' comics and read the content, dPublisher entity can act as an editorial service.

- link: https://www.npmjs.com/package/dreader-comic-verse

---

### [solomon](https://github.com/d-reader-organization/solomon)
> TypeScript, React, MUI, web3.js

‍🫴 Utility library for Solana dApps, seamless MWA integrations

Reducing boilerplate from our frontend applications as they all share same logic: wallet connections, backend authorization via offline message signing, MWA support...

- link: https://www.npmjs.com/package/@open-sauce/solomon
