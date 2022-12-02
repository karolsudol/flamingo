# FLAMINGO

<br/>
<p align="center">
<img src="img/flamingo.png">
</a>
</p>
<br/>

Credit Market for NFTs and yield generating - liquidity scaling protocol.

Primary product is a capital market that enables secondary market liquidity for NFT-backed notes.

Participants can deposit capital in order to earn yield from NFT-backed notes.

# If you hold:

- `NFT` -> you can borrow cash against it on a open market hence best price is gurarnteed
- `CASH`-> you can generate a yield with an option of liqudating the loan at any time
- `CASH`-> you can purchase an assets at the discount via underperforming loan or a liquidated asset

# Incetives

- `Borrowers` access cash quickly with best market price and repurchase staked asset on an operan market
- `Depositors` can exit positions at any time, when asset price goes up or down, and are not left with a toxic asset
- `Allocators` large capital allocators who invest in distressed asset can snipe assets during market downtrends

# Price Discovery

Typically, an asset price is determined by its last sale. However, flamingo's constant asset price evaluation is enabled by secondary credit market hence the underlying asset.

- `English Auction` identifies NFT backed assets and their loan value
- `Gradual Dutch Auction` enables fire sale of a distressed assets

# Example

1. Alice locks a NFT for 10 days auction.

   - She wants min $100k cash
   - She values the NFT at 150k
   - re-paid monthly x 12
   - wth max 20% API paid weekly
   - she can exit the loan early by paying pricipal + interest

2. Bob and John stake $100k USDC

   - She receives no bis, NFT is un-staked so she re-stakes with value to 100$
   - Bobs bids 20% API
   - John bids 10% API - wins auction

3. John and Alice receive a credit note as NFT

   - Alice accepts recurring payment of (10K/12) + 2% fee $835

   - off chain worker makes a sucessful scheduled 1st payment
   - off chain worker makes an un-sucessful scheduled 2nd payment
   - protocol liquidates the loan by transfering staked NFT from Alice to John

   - off chain worker makes a sucessful scheduled 1st paymen
   - Alice places credit note on auction for $150k total

4. John has a toxic asset that he wants to get rid of asap.
   - John places NFT on a Dutch auction with %120k starting price floow of $80k and drop rate of 1% per 1 hr
   - Bob bids 100k and wins he owns the NFT
   - Bob stakes the NFT on auction again, process repeats

## Credit History and Data

- every asset's bid, no bid, sale data etc is emited as logs and placed on a DB
- every users data purchase and credit history is avialble via logs too
- each borrowes credit score is also calculated

## Loan lfe cycle

- `payments` are made to the protocol by borrower that routes them back to the lender
- `early-loan-repayment` can me made by borrower -> principal + interest goes swaps with the collateral
- `loan-defoult` as result of missed repayments is manifested in collateral transfer to lender

## Secondary Markets

- `note` representing a loan can be freely traded by both parties in any secondary markets during its lifecycle, which sale results in protocol updating assets owners if sale occurs

## contracts

- `EnglishAuction.sol`
- `DucthAuction.sol`
- `Vault.sol`
- `CreditNoteNFT.sol`
- `RecurringPayments`

## deployed

- `smart-contract` is deployed and verified on [TBD]()

- with [ownerTBD]()

## dependencies:

- `PRIVATE_KEY="xxx"` in .env

## run:

## TBD
