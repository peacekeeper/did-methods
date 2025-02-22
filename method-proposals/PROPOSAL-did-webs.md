# DID method standardization proposal: did:example

This is a proposal to include `did:webs` in the initial set of DID methods that will be standardized by the DID Methods WG.

## Description

 Like its cousin, `did:web`, the `did:webs` method uses traditional web infrastructure to publish DIDs and make them discoverable. Unlike `did:web`, this method’s trust is not rooted in DNS, webmasters, X509, and certificate authorities. Instead, it uses [KERI](https://trustoverip.github.io/tswg-keri-specification/) to provide a secure chain of cryptographic key events by those who control the identifier.

## Existing materials

* [DID Method Specification](https://trustoverip.github.io/tswg-did-method-webs-specification/)
* A somewhat out-of-date, but still helpful reference [implementation](https://github.com/hyperledger-labs/did-webs-resolver)

## Meeting the selection criteria

Document here how this DID method meets the [DID method selection criteria](../selection-criteria/).

| **Criteria** |
| -------- |
| **Alignment with DID Core specification** |
| Fully compliant with core spec. |
| **Security and privacy features** |
| Publication and discoverability depend on the Web, which diminishes decentralization and privacy. Security is robust due to KERI. |
| **Scalability and performance** |
| With the proper infrastructure available, `did:webs` will scale and perform well. |
| **Ease of implementation and use** |
| Because of KERI, the implementation learning curve is moderate to high. Users must likely exhibit greater accountability, thoughtfulness, and autonomy than for other methods.|
| **Community adoption and support** |
| There is a [KERI working group](https://www.trustoverip.org/our-work/working-groups/) at Trust-Over-IP (TOIP) and an active [developers group](https://github.com/WebOfTrust/keri). Adoption is minimal at present, but organizations like the [Global Legal Identifier Foundation (GLEIF)](https://www.gleif.org/en) are active champions.|
| **Compliance with relevant regulations and best practices** |
| Highly compliant. |
| **Global government-approved crypto** |
| All crypto is first-class and based on current government-approved standards. |
| **Privacy-preserving crypto** |
| The crypto itself is highly privacy-preserving. |
| **Digitally signed cryptographic log of changes to the DID Document** |
| Yes. |
| **Multi-factor binding to DNS** |
| Unkown. |
| **Specification with multiple implementers** |
| Partial. There are multiple implementations of KERI itself. There might not be multiple implementations of `did:webs` itself. |
| **Scope/domain of the types of entities/subjects addressed/named by a particular method** |
| Wide. |
| **Estimate of the daily transaction volume of each scope/domain** |
| Unkown. |
| **DID Methods that do not serve the needs of a particular company or government** |
| Does not. |
| **Governance: Clear frameworks for updates, dispute resolution, and decision-making** |
| Yes. The current standardization body is Trust-Over-IP (TOIP) |
| **Usability: Simple implementation for developers** |
| Moderately complicated. Current reference implementations might be outdated and/or incomplete. |
| **Sustainability: Energy efficiency and eco-friendly infrastructure** |
| Unkown. |
| **Economic Feasibility: DIDs costs of use must be reasonable** |
| Unknown. |
| **Legal Recognition: Cross-border frameworks for DID acceptance** |
| Presumably good. |
| **Revocation and Recovery: Decentralized mechanisms for key rotation and DID recovery** |
| Absolutely. |
| **Emerging Markets: Offline-friendly, low-bandwidth** |
| Yes. |
| **Long-lived DIDs needed for long-lived VCs** |
| Yes. |
| **Low and predictable marginal cost at scale (millions of accounts)** |
| Unkown. |
| **Ability to create and update identifiers rapidly (within seconds)** |
| Yes. |
| **Support for key rotation** |
| Yes. |
| **Reliable and predictable-latency operation, for updating and resolving** |
| Yes. |
| **Resolution should not require additional state or context** |
| Unkown. |
| **DIDs are permanent and immutable account identifiers** |
| UNCLEAR CRITERION |
| **Consider support for various DID Traits: https://identity.foundation/did-traits/** |
| Updateable, Updateable Service Endpoints, Deactivatable, Deletable, Self-Certifying, Rotatable Verification Methods, Pre-rotation of Keys, Multi-Signature Verification Method, Globally Resolvable, Centrally Hosted, United States of America NIST-approved Cryptography |
| **Consider categories defined by DID Rubric: https://www.w3.org/TR/did-rubric/** |
| Not evaluated. |
| **Who WANTS to standardize the DID method and commits to doing the work?** |
| Trust-Over-IP. GLEIF. Other private parties. There is a high liklihood that standardization work would be financially subsidized by parties of interest.|
| **Are there AT LEAST two WG members who support standardization of a DID method?** |
| Yes. |
| **Are there no trademark or IP issues?** |
| None. |
| **Diversity of the set of selected DID methods** |
| n/a |
| **At least one ephemeral DID method** |
| Yes. |
| **At least one web-based DID method** |
| Yes. |
| **At least one fully decentralized DID method** |
| No. |

## Supporting use cases

The `did:webs` method supports any use case supported by other web-based identifiers (like `did:web`). It is highly discoverable but also highly secure.
