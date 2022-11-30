# FLAMINGO

<br/>
<p align="center">
<img src="img/flamingo.png">
</a>
</p>
<br/>

Peer to peer NFT credit market and yield generating - liquidity scaling protocol.

## Participants as Capital

- `Borrowers` find best market price against their ERC721 collateral
- `Depositors` ERC20 token holders who want to generate passive yield
- `Allocators` large capital holders who invest in distressed assets and asset backed loans

## Price Discovery

- `English Auction` provides most efficient mechanism of identifying non liquid asset backed loan price
- `Gradual Dutch Auction` with exponential price decay enables the efficient sale of a distressed assets

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

- `note` representing a loan can be freely traded by both parties in any secondary markets during its lifecycle
- which sale results in protocol updating assets owners if sale occurs

## Distressed Asst Loan Auction

- in case of loan default either asset or asset backed loan can be traded on `Dutch Auction` sale by a lender
- `Capital Allocators` participate in these events providng liquidity to both assets and loans

## Options

- `Capital Allocators` can bid on a right to buy asset on the specified fuure in a form of an option
- `insurance` as such is provided to `lenders`
- `options` are traded in `Dutch Auction`

## Example

Alice and Bob both sign a Promissory Note that gives Bob's 100 USDC to Alice for a period of 90 days, while simultaneously locking Alice's NFT into an escrow contract. If, after the 90 day period, Alice does not return Bob's 100 USDC (Principal) plus 10 USD additional (Interest), Alice's NFT will be released into Bob's ownership.

1. `Alice` owns a `property` and seeks a `loan` against its `deed` as `NFT`.
2. `FundOne` owns `100.000` `USDC` and are looking for a `yield generating asset`.
3. `FundTwo` owns `100.000` `USDC` and are looking for a `yield generating asset`.
4. `LiqudatorOne` owns `100.000` `USDC` and looking for a `undervalued asset` to flip.
5. `LiqudatorTwo` owns `100.000` `USDC` and looking for a `undervalued asset` to flip.

## FLOW

1. `Alice` place `NFT` on the `auction` with params:

   - `min` -> `50.000`
   - `max-APR` -> `10%`
   - `duration` -> `360 days`
   - `auction-length` -> `10 days`

2. `FundOne` esitmates:

   - `floor` -> `60.000`
   - `min-APR` -> `5%`

3. `FundTwo` esitmates:

   - `floor` -> `70.000`
   - `min-APR` -> `8%`

4. `English` auctions starts -> `FundsOne` and `FundsTwo`place bids
5. `FundsTwo` wins
   - `70.000` is transfered from Vault to `Alice`
   - `NFT` is placed in `Vault`
   - `NFT-LOAN` is issued to `FundsTwo` with `1 to 1 redemtion`
6. `FundsTwo` can trade `NFT-LOAN` on secondary market
7. `Alice` makes payments on time

## users

1. `borrowers`
2. `depositors`

## deployed

- `smart-contract` is deployed and verified on [TBD]()

- with [ownerTBD]()

## dependencies:

- `PRIVATE_KEY="xxx"` in .env

## run:

## TBD
