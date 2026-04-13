# Architecture

## Dependency Graph

```mermaid
graph TD
  55470ce1["Stylus-rust-contract (stylus-rust-contract)"]
  34aead19["Erc721-stylus (erc721-stylus)"]
  0db99056["Aixbt-momentum (aixbt-momentum)"]
  b8548fa9["Dune-wallet-balances (dune-wallet-balances)"]
  28c26bae["Smartcache-caching (smartcache-caching)"]
  c15a93ff["Auditware-analyzing (auditware-analyzing)"]
  96b5395e["Ipfs-storage (ipfs-storage)"]
  cbe38818["Dune-nft-floor (dune-nft-floor)"]
  bf5f77f0["Aixbt-signals (aixbt-signals)"]
  17917c17["Frontend-scaffold (frontend-scaffold)"]
  6237fdea["Telegram-notifications (telegram-notifications)"]
  be978e91["Openclaw-agent (openclaw-agent)"]
  476092ba["Wallet-auth (wallet-auth)"]
  17917c17 --> be978e91
  55470ce1 --> 28c26bae
  55470ce1 --> c15a93ff
  55470ce1 --> 17917c17
  34aead19 --> 96b5395e
  34aead19 --> 17917c17
  34aead19 --> cbe38818
  0db99056 --> bf5f77f0
  bf5f77f0 --> 6237fdea
  cbe38818 --> 17917c17
  b8548fa9 --> 17917c17
  0db99056 --> 17917c17
  17917c17 --> 476092ba
```

## Execution / Implementation Order

1. **Stylus-rust-contract** (`55470ce1`)
2. **Erc721-stylus** (`34aead19`)
3. **Aixbt-momentum** (`0db99056`)
4. **Dune-wallet-balances** (`b8548fa9`)
5. **Smartcache-caching** (`28c26bae`)
6. **Auditware-analyzing** (`c15a93ff`)
7. **Ipfs-storage** (`96b5395e`)
8. **Dune-nft-floor** (`cbe38818`)
9. **Aixbt-signals** (`bf5f77f0`)
10. **Frontend-scaffold** (`17917c17`)
11. **Telegram-notifications** (`6237fdea`)
12. **Openclaw-agent** (`be978e91`)
13. **Wallet-auth** (`476092ba`)
