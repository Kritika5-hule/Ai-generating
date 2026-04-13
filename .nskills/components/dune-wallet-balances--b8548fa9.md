# Wallet Balances

| Field | Value |
|-------|-------|
| Type | `dune-wallet-balances` |
| ID | `b8548fa9` |
| Category | analytics |
| Tags | dune, balances, wallet, portfolio |
| Description | Token balances with USD valuations |

## Configuration

| Setting | Value |
|---------|-------|
| Blockchain | arbitrum |
| Min Balance Usd | 1 |
| Include N F Ts | Disabled |
| Generate U I | Enabled |

## Environment Variables

| Key | Description | Required | Secret | Default |
|-----|-------------|----------|--------|---------|
| `DUNE_API_KEY` | Dune Analytics API key for blockchain data queries | Yes | Yes |  |

## File Structure

This component would generate the following files:

- `dune-client.ts` (frontend-lib)
- `useWalletBalances.ts` (frontend-hooks)
- `WalletBalances.tsx` (frontend-components)
- `dune-wallet-balances.md` (docs)

## Integration Points

**Provides to:**
- Frontend-scaffold (`17917c17`)

