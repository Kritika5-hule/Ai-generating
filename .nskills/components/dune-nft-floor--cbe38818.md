# NFT Floor Price

| Field | Value |
|-------|-------|
| Type | `dune-nft-floor` |
| ID | `cbe38818` |
| Category | analytics |
| Tags | dune, nft, floor, collections |
| Description | Collection floor prices and stats |

## Configuration

| Setting | Value |
|---------|-------|
| Blockchain | ethereum |
| Generate U I | Enabled |
| Cache Duration | 300000 |

## Environment Variables

| Key | Description | Required | Secret | Default |
|-----|-------------|----------|--------|---------|
| `DUNE_API_KEY` | Dune Analytics API key for blockchain data queries | Yes | Yes |  |

## File Structure

This component would generate the following files:

- `dune-client.ts` (frontend-lib)
- `useNFTFloor.ts` (frontend-hooks)
- `NFTFloorCard.tsx` (frontend-components)
- `dune-nft-floor.md` (docs)

## Integration Points

**Depends on:**
- Erc721-stylus (`34aead19`)

**Provides to:**
- Frontend-scaffold (`17917c17`)

