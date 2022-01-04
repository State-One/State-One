
<p align="left">
  <img src="./state.png" style="width:300px";>
</p>

**A Decentralized Autonomous State with a DeCentral Bank and privacy preserving Stablecoin System. No private VC round. Only public contribution matters!** 

**Author:** Community 

## Table of Contents 
* [Introduction](#introduction)
* [Overview](#overview)
  * [Governance System](#governance-system)
  * [DeCentral Bank](#decentral-bank)
  * [Token Economics](#token-economics)

## Introduction

A decentralized autonomous state or society (DAS) is a concept in which a group of people govern an organized community independent of 
borders or countries. Ideally these states even don’t require identities. To a certain degree a lot of the existing cryptocurrencies try to integrate mechanisms for this into their protocols. Therefore decentralized governance (DeGov) has 
become one of the important trends in the blockchain space ([see](https://vitalik.ca/general/2021/08/16/voting3.html)). However almost all existing 
solutions have multiple drawbacks and partly rely on tech that prevents the further adoption of the technology.  

**Problems:**
* Inequality of power
* Low turnout
* Privacy

State.One addresses all of these problems with its unique governance system. It does this partly by adapting existing solutions of the centralized world 
and partly by leveraging as well as improving the most successful building blocks of the decentralized ecosystem. Using a decentralized autonomous state, which doesn’t require any identification, as the basis, State.One is able to host an endless variety of decentralized applications. The first one and most significant that should be deployed as part of the core protocol is an algorithmic stablecoin system, which doesn't depend on any centralized system or can be regulated in anyway.   

## Overview

### Governance System

State.One relies on a governance token, called **One** that represents the voting power.   

#### Fair Launch

> "A project that launches as a "pure" DAO from day 1 can achieve a combination of two properties that were previously impossible to combine: (i) sufficiency of developer funding, and (ii) credible neutrality of funding (the much-coveted "fair launch")." [Vitalik 08/2021](https://vitalik.ca/general/2021/08/16/voting3.html)

The distribution of **tokens (=voting rights)** during the initial development process, until the network is deployed, should solely depend on public contributions that are tracked via git. Public contributions can hereby be a variety of things, including marketing and education and aren’t necessarily only focused on the core technology development. It’s up to the token holders to put transparent rules in place about the acceptance of contributions. 

The goal of token holders and the setup itself should be to archive a system, in which tokens are fairly distributed based on actual contribution rather than a unique access to private sales or the overcompensation of the initial contributions. The key assumption is that a fairly distributed token based on actual contribution and involvement will enable a fully decentralized functional governance system in the long run.

It’s important that the rules for incentivizing people are set in place in a transparent way in advance. Retroactiv incentivisation (=airdrops), which are based on luck or insider knowledge are forbidden.  

#### Separation of Powers

> "We aren’t just building businesses so corporate governance won’t work. We aren’t just building economies so economics alone won’t work. We are building global communities, so I’m afraid we are going to need politics."  [outlierventures 02/2019](https://outlierventures.io/research/the-crypto-trias-politica/)

Most of the existing on-chain governance systems oversimplify the entire decision making process, which ultimately leads most of the time to a small group of token holders that actually participate and are in control of the network. These systems therefore can easily be corrupted. In the real world therefore the separation of powers was established and implemented by almost all existing governance systems. This can not only prevent corruption but also improve the efficiency of the decision making process. Furthermore, it allows the implementation of an independent judiciary, that is able to resolve conflicts and even punish misbehaviour, that can not be imblement purely on code basis (e.g. [oracles](#oracles)). 
State.One therefore leverages this existing system and implements it on-chain. Token holders can **lock** their tokens (=voting power) for specific reasons (judiciary or governance) and for a specified time. Once this is done, they can only participate in decisions that are relevant for them. If they actively decide not to participate for a certain time in the process they can delegate their voting power to others. 

#### Privacy

> "Arguing that you don't care about the right to privacy because you have nothing to hide is no different than saying you don't care about free speech because you have nothing to say." Edward Snowden

An increasing number of blockchain projects try to implement DIDs and other identity based systems to prevent sybil attacks and stake “reputation”. While this might increase the security assumptions in the short term, it also increases the attack vectors of the entire network. For example if you know governance bodies or validators or key contributors, you can also influence these in the real world. Therefore the token at stake should be the only mechanisms relevant for securing the network and ideally all parties involved should be anonymous. The “trust” of a decentralized network therefore should only depend on the stake and a transparent governance system and not on the knowledge about individuals. To technically enforce this zero knowledge proofs will be part of the core layer and decision making process.   

### DeCentral Bank

The price volatility of cryptocurrencies as well as the public transaction history are the biggest barriers to widespread adoption that cryptocurrencies face today. Therefore, multiple protocols try to implement so-called “stablecoins”. However, most of them either rely on overcollateralization, which is capital inefficient and/or centralized organisation as well mechanisms. Furthermore, these protocols don’t support private transactions, which makes them useless for companies or individuals that don’t want to share everything immediately publicly with everyone. 

State.One uses an elastic monetary system that can be pegged to the world’s major currencies or even to a basket of choice to retain its purchasing power. The biggest benefit of DeCentral Bank of State.One is hereby the token distribution ([Fair Launch](#fair-launch). Compared to other solutions the voting power is fairly and transparently distributed from the beginning and has no single entity that controls the protocol (e.g. [Terraform Labs](https://finder.terra.money/mainnet/address/terra1dp0taj85ruc299rkdvzp4z5pfg6z6swaed74e6)).   

#### Oracles 

The most important component of such a system are fully functional decentralized oracle solutions. However, most existing oracle solutions are either highly centralized, have no way to slash misbehaviour or use systems like weighted medians for slashing that can theoretically easily be sybil attacked in case they are actually fully decentralized. As pointed out before, State.One therefore establishes an independent judiciary via the [Separation of Powers](#separation-of-powers), which allows the slashing of oracle providers and because of this enables truly decentralized oracle providers.  

#### Stability

The following stability mechanism design is inspired by [Terra Money](https://assets.website-files.com/611153e7af981472d8da199c/618b02d13e938ae1f8ad1e45_Terra_White_paper.pdf). Once an effective oracle solution is implemented, the most efficient way to achieve stability is to establish an on-chain swap mechanism that lets anyone always buy and sell for example 1 State.One Dollar (= StateD) for 1 Dollar (D) (or any other peg): 
- If the demand of StateD increases, the price of 1 StateD goes above 1D. Anyone can now buy 1 StateD for 1D and sell it for more until the price is back to 1.
- If the demand of StateD decreases, the price of 1 StateD goes below 1D. Anyone can now sell 1 StateD for 1D and buy it for less until the price is back to 1. 

These on-chain swap mechanisms should be combined with open source bots that everyone can run and automatically try to benefit from any kind of arbitrage as quickly as possible. 
To enable this swap mechanism a counterparty needs to be established that indirectly is willing to accept short term losses in case the total demand of the currency decreases as well as benefits from an increased demand. Therefore the governance token One will be minted and solt or burnt. This effectively moves the volatility from the stablecoins to the governance token One. It’s assumed that token holders lock their tokens (see [Separation of Powers](#separation-of-powers)) for a longer period of time and thus don’t care about short term losses. 

#### Piravte Payments

### Token Economics

The total amount of voting rights at the launch of the network depends on the hours contributed to the project. At the beginning a contribution of 1 hour should be worth roughly 10 voting rights (tokens). After each distribution of a multiple of 100.000 voting rights, the amount of tokens distributed per hour is halved. 

