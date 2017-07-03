# Ilúvatar

<p align="center">
    <img src="logo.jpg" />
</p>

Main repository for [Ilúvatar Exchange](https://www.iluvatar.exchange).

This is the main repository for all code related to the Ilúvatar Exchange. Any document about macro development planning (aka not bounded to a single project) and non-development subjects (e.g., commercial strategy) must be kept here.

## Ilúvatar Exchange

Ilúvatar Exchange is the newest cryptocurrency exchange to dominate the market in the next months. The current intention is to trade only cryptocurrencies (altcoins) using Bitcoin as medium, avoiding dealing with fiat money and all complications (aka regulations) that it brings.

The exchange will encompass the project bidet, developed in another repository. The idea is to develop it as modular as possible, following a microservice approach and using other state-of-the-art technologies (e.g., Apache Thrift, CDC and Kafka).

## Projects

### [Heimdallr](https://github.com/embatbr/iluvatar-heimdallr)

- *Public?* **NO**

Responsible for registration, authentication and authorization. Higher clearance possible.

### [Isimud](https://github.com/embatbr/iluvatar-isimud)

- *Public?* **NO**

Messaging system (email, push notifications and etc.)

### [Portinari](https://github.com/embatbr/iluvatar-portinari)

- *Public?* **YES**

Front-end responsible for user interface. Returns HTML, JS and updates the graphics.

### [Nasdaq](https://github.com/embatbr/iluvatar-nasdaq)

- *Public?* **YES**

Public API. Trading front-end (only part of the trading system connected to the internet).

### [Bidet](https://github.com/embatbr/iluvatar-bidet)

- *Public?* **NO**

Trading back-end. Validates and stores orders and deals with execution of bids and asks. Accepts requests only from Termopilas.

### [Franz](https://github.com/embatbr/iluvatar-franz)

- *Public?* **NO**

Responsible for maintain data ordering consistency. Creates Kafka queues, Redis instances and any other infrastructure needed.

### [Soroban](https://github.com/embatbr/iluvatar-soroban)

- *Public?* **NO**

Deals with funding (deposits and withdrawls) in conjunction with Heimdallr. Access cryptocurrencies hot and cold wallets.
