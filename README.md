# FLAMINGO

<br/>
<p align="center">
<img src="img/flamingo.png">
</a>
</p>
<br/>

Credit Market for real asset backed NFTs and yield generating - liquidity scaling protocol.

Primary product is a capital market that enables secondary market liquidity for NFT-backed notes.

Participants can deposit capital in order to earn yield from diversified portfolios of NFT-backed notes.

# If you hold:

- `NFT` -> you can borrow cash against it on a open market hence best price is gurarnteed
- `CASH`-> you can generate a yield with an option of liqudating the loan at any time
- `CASH`-> you can purchase an assets at the discount via underperforming loan or a liquidated asset

# Incetives

- `Borrowers` access cash quickly and find best market price for your collateral
- `Depositors` can exit positions at any time, and are not left with a toxic asset
- `Allocators` large capital allocators who invest in distressed asset can snipe assets during market downtrends

# Price Discovery

- `English Auction` identifies NFT backed assets and their loan value
- `Gradual Dutch Auction` enables fire sale of a distressed assets
- `Credit Auctions`

# Example

- you bought an appartment for $200k
- and you have an opportunity to buy another, next door, for a market discount rate of 20%
- you are convinced that you can rent it out for 2k a mnoth
- you do not have cash
-

d assets and asset backed loans

## Loan Auction

- `ERC-721` -> borrower and `ERC20` -> lender place their asset in a the vault
- `borrower` determines max interest and min asset price is willing to accept
- `lenders` place bids on the asset during lenght of the auction
- `loan` is issued at the end of the auction as ERC721 note to lender and borrower

## Loan lfe cycle

- `payments` are made to the protocol by borrower that routes them back to the lender
- `early-loan-repayment` can me made by borrower -> principal + interest goes swaps with the collateral
- `loan-defoult` as result of missed repayments is manifested in collateral transfer to lender

## Secondary Markets

- `note` representing a loan can be freely traded by both parties in any secondary markets during its lifecycle, which sale results in protocol updating assets owners if sale occurs

## Example

1.  - `Alice and Bob` both sign a Promissory Note that gives Bob's 100 USDC to Alice for a period of 90 days, while simultaneously locking Alice's NFT into an escrow contract.
    - If, after the 90 day period, Alice does not return Bob's 100 USDC (Principal) plus 10 USD additional (Interest), Alice's NFT will be released into Bob's ownership.

2.  - `Alice` owns a property and seeks a loan against its deed in form of NFT.
    - `Capital_1` and `Capital_2` own 100.000 USDC each and are looking for a yield generating asset.
    - `Capital_3` and `Capital_4` own 100.000 USDC each and are looking for buying assets under their fair market value

## credit history

account holders build credit history based on their loan repayments that allows for uncolaterised loan issuance

## contracts

- `EnglishAuction`
- `Vault.sol`
- `LPToken.sol`

## deployed

- `smart-contract` is deployed and verified on [TBD]()

- with [ownerTBD]()

## dependencies:

- `PRIVATE_KEY="xxx"` in .env

## run:

## TBD
