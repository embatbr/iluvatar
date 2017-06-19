# Ilúvatar

Main repository for [Ilúvatar Exchange](https://www.iluvatar.exchange).

This is the main repository for all code related to the Ilúvatar Exchange. Any document about macro development planning (aka not bounded to a single project) and non-development subjects (e.g., commercial strategy) must be kept here.

## Ilúvatar Exchange

Ilúvatar Exchange is the newest cryptocurrency exchange to dominate the market in the next months. The current intention is to trade only cryptocurrencies (altcoins) using Bitcoin as medium, avoiding dealing with fiat money and all complications (aka regulations) that it brings.

The exchange will encompass the project bidet, developed in another repository. The idea is to develop it as modular as possible, following a microservice approach and using other state-of-the-art technologies (e.g., Apache Thrift, CDC and Kafka).

## Projects

### [Kernel](https://github.com/embatbr/kernel)

Base code, necessary to deal with databases, queues and any sort of storage system (permanent of ephemeral).

### [Heimdallr](https://github.com/embatbr/heimdallr)

*Uses Kernel?* **YES**

Responsible for registration, authentication and authorization. Higher clearance possible.

### [Portinari](https://github.com/embatbr/portinari)

*Uses Kernel?* **NO**

Front-end responsible for user interface. Returns HTML, JS and updates the graphics.

### [Termópilas](https://github.com/embatbr/termopilas)

*Uses Kernel?* **NO**

Public API. Trading front-end (only part of the trading system connected to the internet).

### [Bidet](https://github.com/embatbr/bidet)

*Uses Kernel?* **YES**

Trading back-end. Validates and stores orders and deals with execution of bids and asks. Accepts requests only from Termopilas.

### [Franz](https://github.com/embatbr/franz)

*Uses Kernel?* **YES**

Responsible for maintain data ordering consistency. Creates Kafka queues and Redis instances.

### [Shannon](https://github.com/embatbr/shannon)

*Uses Kernel?* **YES**

Deals with funding (deposits and withdrawls). Access cryptocurrencies hot and cold wallets.
