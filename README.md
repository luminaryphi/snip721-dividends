Modification of the SNIP-721 Impl allowing for dividend distribution to nft holders.

`deposit_rewards()` sends SNIP-20 tokens into the contract to be be divided up for each nft share so it can be claimed. The SNIP-20 token is set during `init`

`claim_tokens` allows the nft owner to claim all rewards for a specified nft. As the nfts are what are linked to token allocation, not a user address, you must specify each token you are claiming.

Transfer of nfts will automatically claim the SNIP-20 tokens for you, before sending it to the new address.