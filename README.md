# My App

A Web3 dApp composed with [[N]skills](https://www.nskills.xyz).

## Blueprint: selected nodes

These components were included in this generation:

- **Stylus Rust Contract** — Guide for building Rust smart contracts on Arbitrum Stylus
- **ERC-721 Stylus NFT** — Deploy and interact with ERC-721 NFTs on Arbitrum Stylus
- **AIXBT Momentum** — Track social momentum and cluster convergence for projects
- **Dune Wallet Balances** — Fetch wallet token balances with USD values using Dune Analytics
- **SmartCache Caching** — Enable contract caching for cheaper gas - mycontracts (original) + cached-contracts (with caching)
- **Auditware Analyzer** — Security analysis with Radar for Rust smart contracts
- **IPFS Storage** — Decentralized storage with Pinata or Web3.Storage
- **Dune NFT Floor Price** — Fetch NFT collection floor prices and statistics using Dune Analytics
- **AIXBT Signals** — Real-time event signals for project activity
- **Frontend Scaffold** — Generate a Next.js Web3 application with wagmi, RainbowKit, and smart contract integration
- **Telegram Notifications** — Send-only Telegram integration for alerts and updates
- **OpenClaw** — Prompt-driven OpenClaw agent block
- **Wallet Authentication** — Wallet connection with RainbowKit and WalletConnect

## Project structure

```
my-app/
├── apps/
│   └── web/                    # Next.js app (install dependencies here)
│       ├── src/
│       ├── package.json
│       └── ...
├── contracts/                  # Rust/Stylus smart contracts
│   ├── mycontract/            # Original contract (no caching)
│   │   └── src/lib.rs
│   └── cached-contract/       # Contract with is_cacheable helper
│       └── src/lib.rs
├── docs/                       # Documentation
├── scripts/                     # Deploy / utility scripts (if generated)
├── .gitignore
└── README.md
```

## Quick start

### Prerequisites

- **Node.js** 18+ and **npm** (comes with Node.js)
- **Rust** toolchain and **cargo-stylus** for building/deploying Stylus contracts (see `docs/` and [Stylus SDK](https://github.com/OffchainLabs/stylus-sdk-rs))

### Step-by-step

1. **Clone and enter the project**

   ```bash
   git clone <your-repo-url>
   cd <your-repo-name>
   ```

   ![Clone and enter the project](https://raw.githubusercontent.com/Cradle-app/NSkills/main/apps/web/public/clone-and-enter.png)

2. **Install dependencies** for the Next.js app (this project has no root `package.json`; dependencies live under `apps/web`):

   ```bash
   cd apps/web
   npm install
   ```

   ![Install dependencies](https://raw.githubusercontent.com/Cradle-app/NSkills/main/apps/web/public/install-dep.png)

3. **Environment variables**

   ```bash
   cp .env.example .env
   ```

   Edit `.env` and set:

   - `STYLUS_RPC_URL`: Arbitrum RPC URL for deployment
   - `DEPLOYER_PRIVATE_KEY`: Private key for deployment
   - `AIXBT_API_KEY`: AIXBT API Key for market intelligence
   - `DUNE_API_KEY`: Dune Analytics API key for blockchain data queries
   - `PINATA_API_KEY`: Pinata API key
   - `PINATA_SECRET_KEY`: Pinata secret API key
   - `NEXT_PUBLIC_WALLETCONNECT_PROJECT_ID`: WalletConnect Cloud project ID for wallet connections
   - `TELEGRAM_BOT_TOKEN`: Bot token from @BotFather

   ![Environment variables](https://raw.githubusercontent.com/Cradle-app/NSkills/main/apps/web/public/env-var.png)

### ERC-721 Integration

Add the `ERC721InteractionPanel` to `apps/web/src/app/page.tsx`:

```tsx
import { WalletButton } from '@/components/wallet-button';
import { ERC721InteractionPanel } from '@/lib/erc721-stylus/src';

export default function Home() {
  return (
    <main className="flex min-h-screen flex-col items-center justify-center p-24">
      <div className="max-w-5xl w-full text-center">
        <h1 className="text-4xl font-bold mb-8">
          My DApp
        </h1>
        <p className="text-lg text-gray-600 dark:text-gray-400 mb-12">
          A Web3 application built with Cradle
        </p>

        <div className="flex justify-center">
          <WalletButton />
        </div>

        <ERC721InteractionPanel />
      </div>
    </main>
  );
}
```

### Run the web app

```bash
cd apps/web && npm run dev
```

Open [http://localhost:3000](http://localhost:3000).


## Documentation

Check the `docs/` folder for guides that match your blueprint (e.g. frontend setup, contract deployment, API routes).

## License

MIT

---

Generated with [[N]skills](https://www.nskills.xyz)
