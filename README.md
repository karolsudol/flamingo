# FLAMINGO

<br/>
<p align="center">
<img src="img/flamingo.png">
</a>
</p>
<br/>

- `Flamingo` is a peer to peer `NFT credit market` and `yield generating` - `liquidity scaling` protocol.
- Implementation of Discrete `Gradual Dutch Auction` with `exponential price decay` for `ERC721`
- `GDA` enable the efficient sale of assets that do not have `liquid markets`
-

## USERS

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
8.

Alice and Bob both sign a Promissory Note that gives Bob's 30 ETH to Alice for a period of 90 days, while simultaneously locking Alice's CryptoPunk into an escrow contract. If, after the 90 day period, Alice does not return Bob's 30 ETH (Principal) plus 1 ETH additional (Interest), Alice's CryptoPunk will be released into Bob's ownership.

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
