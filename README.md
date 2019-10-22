# Aragon Basic Prediction Market App

> Prediction markets (also known as predictive markets, information markets, decision markets, idea futures, event derivatives, or virtual markets) are exchange-traded markets created for the purpose of trading the outcome of events. The market prices can indicate what the crowd thinks the probability of the event is. A prediction market contract trades between 0 and 100%.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Prediction_market)

## Prediction Market
In this prediction market, trading is split into shares. Each share pays out 100 wei if the answer resolves to Yes, and 0 wei if the answer resolves to No. In this way, the price per share reflects the market’s possibility of resolving to Yes. If the price for the preceding market is 10, the market thinks there’s a 10% probability that Ethereum will be above $2,000 at the beginning of 2020. To start a market, a market creator must post collateral for the payouts, 100 wei for each share. If the market resolves to Yes, the collateral is paid out to the owners of the shares. If the market resolves to No, the collateral is paid back to the market creator.

In exchange for taking on this risk, the market creator is allowed to charge a fee on every trade. Typical fees on cryptocurrency exchanges are between 0.1% and 0.25%. Our contract will charge 0.2% on each side of a trade, but this can be changed easily.

## What is an Aragon App
Most smart contracts have a `owner = msg.sender` instruction giving the deployer of the contract some special previliges. These functions are usualy
introduced in the DApp in order to avoid unknown problems that might arise due to a bug or simply to upgrade the application.

However, having one private key or even a multisug account control a contract subverts the most usefull propery of a dApp, its decentralised architecture. **MOST** dApps are not dApps at all because they are governed by a few keys at best, and usualy just one.

This dApp leverages [AragonOS](https://github.com/aragon/aragonOS), a governance framework giving the governance of the dApp to a [DAO](https://github.com/aragon/aragon.js/tree/master/packages/aragon-client)

## How To Run The dApp localy

### Dependencies

### Instructions

### Libraries
