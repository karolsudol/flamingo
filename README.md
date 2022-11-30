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

1.  - `Alice and Bob` both sign a Promissory Note that gives Bob's 100 USDC to Alice for a period of 90 days, while simultaneously locking Alice's NFT into an escrow contract.
    - If, after the 90 day period, Alice does not return Bob's 100 USDC (Principal) plus 10 USD additional (Interest), Alice's NFT will be released into Bob's ownership.

2.  - `Alice` owns a property and seeks a loan against its deed in form of NFT.
    - `Capital_1` and `Capital_2` own 100.000 USDC each and are looking for a yield generating asset.
    - `Capital_3` and `Capital_4` own 100.000 USDC each and are looking for buying assets under their fair market value

## credit history

## deployed

- `smart-contract` is deployed and verified on [TBD]()

- with [ownerTBD]()

## dependencies:

- `PRIVATE_KEY="xxx"` in .env

## run:

## TBD
