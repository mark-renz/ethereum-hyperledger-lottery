# Lottery Process Flow Diagram

Lotteries are an excellent use case for Ethereum. This repo will show the process flow diagram of lotteries in Ethereum and Hyperledger to show it's difference


## Ethereum
Following are the process diagrams of the lottery games.

* [Simple Lottery](https://github.com/johnmackyllego/lottery/blob/master/ethereum/simple-lottery/Simple-lottery.jpg)  - This simple-lottery is nonrecurring, uses blockhashes for random numbers, and has only
one winner.

* [Recurring Lottery](https://github.com/mark-renz/ethereum-hyperledger-lottery/tree/master/ethereum/recurring)  - The
recurring lottery will occur in rounds so that a new prize pool is started every
time the old one closes. It will also allow users to purchase multiple
tickets in one transaction instead of just one and add a couple of security
improvement

* [RNG Lottery](https://github.com/mark-renz/ethereum-hyperledger-lottery/tree/master/ethereum/rng) - The RNG Lottery is non-recurring, the numbers are randomly generated. Also after the round all users must reveal their tickets or else it will drop.


* [Powerball](https://github.com/mark-renz/ethereum-hyperledger-lottery/tree/master/ethereum/powerball)  - In Powerball, the user picks six numbers per ticket. The first five
numbers are standard numbers from 1–69, and the sixth number is a
special Powerball number from 1–26 that offers extra rewards. Every three
or four days, a drawing is held, and a winning ticket consisting of five
standard numbers and a Powerball number is picked. Prizes are paid out
based on the number of winning numbers matched on your ticket.

## Hyperledger
Following are the process diagrams of the lottery games.

* [Simple Lottery](https://github.com/mark-renz/ethereum-hyperledger-lottery/tree/master/hyperledger/simple)

* [Recurring Lottery](https://github.com/mark-renz/ethereum-hyperledger-lottery/tree/master/hyperledger/recurring)

* [RNG Lottery](https://github.com/mark-renz/ethereum-hyperledger-lottery/tree/master/hyperledger/rng)

* [Powerball](https://github.com/mark-renz/ethereum-hyperledger-lottery/tree/master/hyperledger/powerball)

## Changes from ethereum to hyperledger design

* **Wallet** - wallet does not exist from hyperledger so we've created accounts
so we can save the users identity and token count. This will act as a wallet
where we deduct or pass the reward token for the lottery.

* **Public blockchain** - hyperledger is a private blockchain so the solution we present is to create
the accounts inside one chaincode. This way all users, in the chaincode, will publicly allowed to see all data
inside one chaincode.

* **Addresses** - in ethereum, users are identified through their addresses. In our design, users will be
identified through the account they have registered.

## Contributors:

* Use cases is based from a book that is tutorial for building games using ethereum
* [John Machy Llego](https://github.com/johnmackyllego) 
* [Paul Kristian Erandio](https://github.com/tensaipaul) 
* [Mark Renz Manalo](https://github.com/mark-renz)
* [Justine Mervic Berango](https://github.com/hustino)
* [Kevin Perez](https://github.com/kvzprz)
