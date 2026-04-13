# Integration Map

How components connect and what data flows between them.

### Frontend-scaffold --> Openclaw-agent

- **Source**: Frontend-scaffold (`17917c17`)
  - Output ports: App Context (config)
- **Target**: Openclaw-agent (`be978e91`)
  - Input ports: Agent Prompt (config)

### Stylus-rust-contract --> Smartcache-caching

- **Source**: Stylus-rust-contract (`55470ce1`)
  - Output ports: Contract Code (contract)
- **Target**: Smartcache-caching (`28c26bae`)
  - Input ports: Contract Input (contract)

### Stylus-rust-contract --> Auditware-analyzing

- **Source**: Stylus-rust-contract (`55470ce1`)
  - Output ports: Contract Code (contract)
- **Target**: Auditware-analyzing (`c15a93ff`)
  - Input ports: Contract Input (contract)

### Stylus-rust-contract --> Frontend-scaffold

- **Source**: Stylus-rust-contract (`55470ce1`)
  - Output ports: Contract Code (contract)
- **Target**: Frontend-scaffold (`17917c17`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Erc721-stylus --> Ipfs-storage

- **Source**: Erc721-stylus (`34aead19`)
  - Output ports: NFT Contract (contract)
- **Target**: Ipfs-storage (`96b5395e`)
  

### Erc721-stylus --> Frontend-scaffold

- **Source**: Erc721-stylus (`34aead19`)
  - Output ports: NFT Contract (contract)
- **Target**: Frontend-scaffold (`17917c17`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Erc721-stylus --> Dune-nft-floor

- **Source**: Erc721-stylus (`34aead19`)
  - Output ports: NFT Contract (contract)
- **Target**: Dune-nft-floor (`cbe38818`)
  

### Aixbt-momentum --> Aixbt-signals

- **Source**: Aixbt-momentum (`0db99056`)
  - Output ports: Momentum Data (api)
- **Target**: Aixbt-signals (`bf5f77f0`)
  

### Aixbt-signals --> Telegram-notifications

- **Source**: Aixbt-signals (`bf5f77f0`)
  - Output ports: Signals Feed (api)
- **Target**: Telegram-notifications (`6237fdea`)
  

### Dune-nft-floor --> Frontend-scaffold

- **Source**: Dune-nft-floor (`cbe38818`)
  - Output ports: NFT Floor Data (types)
- **Target**: Frontend-scaffold (`17917c17`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Dune-wallet-balances --> Frontend-scaffold

- **Source**: Dune-wallet-balances (`b8548fa9`)
  - Output ports: Wallet Balances (types)
- **Target**: Frontend-scaffold (`17917c17`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Aixbt-momentum --> Frontend-scaffold

- **Source**: Aixbt-momentum (`0db99056`)
  - Output ports: Momentum Data (api)
- **Target**: Frontend-scaffold (`17917c17`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Frontend-scaffold --> Wallet-auth

- **Source**: Frontend-scaffold (`17917c17`)
  - Output ports: App Context (config)
- **Target**: Wallet-auth (`476092ba`)
  
