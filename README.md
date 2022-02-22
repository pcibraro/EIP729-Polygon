# EIP729-Polygon

This is a port of the Subgraph (https://github.com/wighawag/eip721-subgraph)[https://github.com/wighawag/eip721-subgraph] but configured to index EIP729 contracts from the Matic network.

# example graphQL query
```
{
  tokens {
    contract
    tokenID
    owner
    tokenURI
  }
}
```
or

```
{
  tokens(orderBy: mintTime) {
    contract
    tokenID
    owner
    tokenURI
    mintTime
  }
  
  tokenContracts {
    id
  }
}
```
