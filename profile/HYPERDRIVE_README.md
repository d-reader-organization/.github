# Encode hackathon submission

During the hackathon we've:
- built & deployed [dPublisher web app](https://dpublisher.app)
- finished [dPublisher Smart Contract](https://github.com/d-reader-organization/d-reader-comic-verse)
- finished [dPublisher backend](https://api-main-mainnet.dreader.io/api) features (mixed with dReader's backend)

**dPublisher**:
- creators can choose to self-publish a comic without any prior crypto knowledge
- for now, if they're not willing to use a digital wallet, we will generate a keypair for them and off-ramp crypto to their fiat account manually. Cost of the Candy Machine and transacting (e.g. signing digital comics to fans) is paid by us.
- in the future, crypto off-ramp will be automated
- interface is mobile friendly, which wasn't an initial idea but a significant portion of initial creators requested "wen mobile"
- so we've killed dPublisher frontend and built it with mobile-first in mind while making it an installable PWA

> **Warning**
> we've previously won hackathons **with dReader**. Our focus for Hyperdrive hackathon was on dPublisher.

References:
- [d-reader-backend](https://github.com/d-reader-organization/d-reader-backend)
- [d-publisher-frontend](https://github.com/d-reader-organization/d-publisher-frontend)
- [d-reader-comic-verse](https://github.com/d-reader-organization/d-reader-comic-verse)