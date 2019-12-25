# Parity cryptonode-wallet Blockchain

The geth image service cryptonode and daemon need to be started:

```rake service:daemons[start]```

```rake service:cryptonodes[start]```

```rake service:cryptonodes[stop]```

```rake service:cryptonodes[restart]```


#### Command list helper:

```docker run parity/parity:v2.5.11-stable --help```

#### Connect Main eth account:

```docker run -it parity/parity:v2.5.11-stable```

#### Connect to Kovan network testnet:

```docker run -it parity/parity:v2.5.11-stable --chain kovan```

#### Connect to Ropsten network testnet:

```docker run -it parity/parity:v2.5.11-stable --chain ropsten```

#### Command create account a main network:

```docker run -it parity/parity:v2.5.11-stable account new```

#### Command create testnet Kovan account:

```docker run -it parity/parity:v2.5.11-stable --chain kovan account new```

#### Command create testnet Ropsten account:

```docker run -it parity/parity:v2.5.11-stable --chain ropsten account new```

#### Command account list testnet Kovan:

```docker run -it parity/parity:v2.5.11-stable --chain kovan account list```

## Jsonrpc-apis personal


#### Mainnet account jsonrpc

```docker run -it parity/parity:v2.5.11-stable --chain mainnet --jsonrpc-apis personal```

#### Ropsten jsonrpc

```docker run -it parity/parity:v2.5.11-stable --chain ropsten --jsonrpc-apis personal```

#### Kovan jsonrpc

```docker run -it parity/parity:v2.5.11-stable --chain kovan --jsonrpc-apis personal```

## APIS 

```docker run -it parity/parity:v2.5.11-stable --chain kovan --jsonrpc-apis <COMAND>```

List api <COMAND>
  
* web3
* net
* eth
* eth_pubsub
* eth_pubsub
* personal
* parity
* parity_accounts
* parity_set
* pubsub
* signer
* trace
* shh
* secretstore

## Useful docker commands

#### CLI parity bash or sh

```docker exec -it <CONTAINER-ID> sh``` or ```docker exec -it <CONTAINER-ID> bash```

#### Check logs container

```docker logs -f <COINTAINER-D>```
or
```docker-compose logs -f parity```

#### Check status container

```docker-compose ps```


docker exec -it opendax_parity_1 sh
opendax_parity_1



## References

* https://wiki.parity.io/
* https://wiki.parity.io/JSONRPC






