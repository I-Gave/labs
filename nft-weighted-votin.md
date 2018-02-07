# Proposal: Weighted NFT Voting

Author(s): Alex Sherbuck alex@igave.io

Last updated: 2018/02/07

## Abstract

Assigning a vote weight to non-fungible assets allows for DAO voting based on asset holdings. The nature of NFTs is that they are valued differently from one another. An organization may decide to weight their assets.

This allows for organizations to govern based on their assets.

## Proposal

My specific use case - We issue an NFT as a receipt for a charitable donation. We would like a DAO that honors each donation's Ether value as a 1:1 vote. So as donor's increase their donations they have a greater say.

Groups could base voting weight on cryptokitty rarity, LAND holdings or auction valuations, etc. It's up to the organization to decide.

## Rationale

Well DAOs are currently run like corporations with shareholders. This type of DAO could be bootstrapped with an ICO. In our project, we plan for our DAPP that issues the NFT to eventually hold more  DAO votes than our ICO contributors.

So this model allows for the users to inherit the organization after some period of time passes.

## References (Optional)

I literally submitted an EIP that puts the idea forward yesterday [here](https://github.com/ethereum/EIPs/pull/874). The current implementation is basically shoe-horned into an ERC-721.

In talking to @eordano about how this could fit with ERC-821 it seems an extension/adapter is the best path forward. I'd like to commit more of my time to getting this working properly.

## Open Issues (Optional)

So in my experiments this is actually quite simple when the weight value never changes. E.g. A cryptokitty generation will never change - a receipt amount never changes, etc. This is easy.

But if you wanted to, say, let weight be determined by the last sale price that gets tricky as its very easy to game that.

