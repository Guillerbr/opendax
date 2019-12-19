Parity cryptonode-wallet Blockchain

The geth image service cryptonode and daemon need to be started:

rake service: daemons [start]
rake service: cryptonodes [start]

Command list helper:

- docker run parity/parity:v2.5.11-stable --help

Connect Main eth account:

- docker run -it parity/parity:v2.5.11-stable

Connect to Kovan network testnet:

- docker run -it parity/parity:v2.5.11-stable --chain kovan

Command create account a princpal network:

- docker run -it parity/parity:v2.5.11-stable account new

Command create testnet Kovan account:

- docker run -it parity/parity:v2.5.11-stable --chain kovan account new



