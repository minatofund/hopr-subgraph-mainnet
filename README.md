# Hopr Subgraph Mainnet
HOPR on Ethereum mainnet subgraph

## Deploy on Explorer
This subgraph has been deployed. You can find the details and use playground here.

https://thegraph.com/explorer/subgraph/minatofund/hopr-subgraph-mainnet

## Demo
* Video Demo 

[https://www.youtube.com/watch?v=28TcZ4TBjZ4](https://www.youtube.com/watch?v=28TcZ4TBjZ4)

* Live Demo (Staging)

[https://knowyourdefistg.z11.web.core.windows.net/](https://knowyourdefistg.z11.web.core.windows.net/)

* Live Demo PR

[https://github.com/KnowYourDeFi/knowyourdefi.github.io/pull/1](https://github.com/KnowYourDeFi/knowyourdefi.github.io/pull/1)


## Sample Query

```
{
  accounts(first: 5) {
    id
    index
    totalSupply
    HoprBalance
  }
  accountSnapshots(first: 5) {
    id
    index
    account {
      id
    }
    HoprBalance
  }
}
```

Response
```
{
  "data": {
    "accountSnapshots": [
      {
        "HoprBalance": "85000000",
        "account": {
          "id": "0x0000000000000000000000000000000000000000"
        },
        "id": "0x0000000000000000000000000000000000000000-11891539",
        "index": "1"
      },
      {
        "HoprBalance": "85000001",
        "account": {
          "id": "0x0000000000000000000000000000000000000000"
        },
        "id": "0x0000000000000000000000000000000000000000-11966495",
        "index": "27920"
      },
      {
        "HoprBalance": "98333333",
        "account": {
          "id": "0x0000000000000000000000000000000000000000"
        },
        "id": "0x0000000000000000000000000000000000000000-11966499",
        "index": "27923"
      },
      {
        "HoprBalance": "130208333",
        "account": {
          "id": "0x0000000000000000000000000000000000000000"
        },
        "id": "0x0000000000000000000000000000000000000000-11966545",
        "index": "27932"
      },
      {
        "HoprBalance": "0",
        "account": {
          "id": "0x0000000000000eb4ec62758aae93400b3e5f7f18"
        },
        "id": "0x0000000000000eb4ec62758aae93400b3e5f7f18-11955475",
        "index": "25862"
      }
    ],
    "accounts": [
      {
        "HoprBalance": "130208333",
        "id": "0x0000000000000000000000000000000000000000",
        "index": "1",
        "totalSupply": true
      },
      {
        "HoprBalance": "0",
        "id": "0x0000000000000eb4ec62758aae93400b3e5f7f18",
        "index": "6368",
        "totalSupply": false
      },
      {
        "HoprBalance": "0",
        "id": "0x00000000000064c443ef440577c26525a3c34a30",
        "index": "5562",
        "totalSupply": false
      },
      {
        "HoprBalance": "4.479165703413467007",
        "id": "0x0000000000007f150bd6f54c40a34d7c3d5e9f56",
        "index": "4222",
        "totalSupply": false
      },
      {
        "HoprBalance": "0",
        "id": "0x0000000000c9b1dde987a6abe20a2af8d9e636d9",
        "index": "7247",
        "totalSupply": false
      }
    ]
  }
}
```
