# eru

Main repository for [Eru Exchange](https://www.eru.exchange).

This is the main repository for all code related to the Eru Exchange. Any document about macro development planning (aka not bounded to a single project) and non-development subjects (e.g., commercial strategy) must be kept here.

## Eru Exchange

Eru Exchange is the newest cryptocurrency exchange to dominate the market in the next months. The current intention is to trade only cryptocurrencies (BTC-LTC, BTC-ETH and etc.), avoiding dealing with fiat money and all complications (aka regulations) that it brings.

The exchange will encompass the project bidet, developed in another repository. The idea is to develop it as modular as possible, following a microservice approach and using other state-of-the-art technologies (e.g., Apache Thrift, CDC and Kafka).

## Projects

- [Kernel](https://github.com/embatbr/eru-kernel): base code; common to all repositories;
- [Chieftain](https://github.com/embatbr/eru-chieftain): big boss; registration, authentication and authorization; higher clearance possible;
- [Portinari](https://github.com/embatbr/eru-portinari): front-end responsible for UI;
- [Termopilas](https://github.com/embatbr/eru-termopilas): trading front-end; connected to the internet;
- [Babbage](https://github.com/embatbr/eru-babbage): trading back-end; validates and storages orders; receives requests from Termopilas only;
- [Bidet](https://github.com/embatbr/eru-bidet): deals with execution of bids and asks orders;
- [Shannon](https://github.com/embatbr/eru-shannon): deals with hot and cold wallets.
