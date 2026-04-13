# AIXBT Momentum

| Field | Value |
|-------|-------|
| Type | `aixbt-momentum` |
| ID | `0db99056` |
| Category | intelligence |
| Tags | aixbt, momentum, social, trends, analytics |
| Description | Track social heat and project trends |

## Configuration

| Setting | Value |
|---------|-------|
| Project Id | bitcoin |
| Interval | 24h |
| Include Historical Data | Enabled |
| Track Cluster Convergence | Enabled |

## Environment Variables

| Key | Description | Required | Secret | Default |
|-----|-------------|----------|--------|---------|
| `AIXBT_API_KEY` | AIXBT API Key for market intelligence | Yes | Yes |  |

## Documentation

### AIXBT Integration


# AIXBT Intelligence Integration

This module provides access to AIXBT's market intelligence layer.

## Setup

1. Get your API Key from [aixbt.tech](https://aixbt.tech/settings/api-keys).
2. Add `AIXBT_API_KEY` to your `.env` file.

## Usage

### Fetching Trending Projects

```typescript
import { AIXBTClient } from './src/intelligence/aixbt-client';

const client = new AIXBTClient(process.env.AIXBT_API_KEY);
const trending = await client.getTrendingProjects(5);
console.log('Top projects by momentum:', trending);
```

### AI Research with Indigo

```typescript
import { generateResearchReport } from './src/intelligence/indigo';

const report = await generateResearchReport(
  'Summarize the current sentiment for Arbitrum Stylus',
  process.env.AIXBT_API_KEY
);
console.log(report);
```


## File Structure

This component would generate the following files:

- `aixbt-client.ts` (frontend-lib)

## Integration Points

**Provides to:**
- Aixbt-signals (`bf5f77f0`)
- Frontend-scaffold (`17917c17`)

