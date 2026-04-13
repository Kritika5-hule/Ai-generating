# AIXBT Signals

| Field | Value |
|-------|-------|
| Type | `aixbt-signals` |
| ID | `bf5f77f0` |
| Category | intelligence |
| Tags | aixbt, signals, alerts, activity |
| Description | Real-time project activity alerts |

## Configuration

| Setting | Value |
|---------|-------|
| Categories | LISTING, FUNDING, PARTNERSHIP |
| Min Conviction Score | 0.7 |
| Limit | 20 |

## Environment Variables

| Key | Description | Required | Secret | Default |
|-----|-------------|----------|--------|---------|
| `AIXBT_API_KEY` | AIXBT API Key for market intelligence | Yes | No |  |

## File Structure

This component would generate the following files:

- `aixbt-client.ts` (frontend-lib)

## Integration Points

**Depends on:**
- Aixbt-momentum (`0db99056`)

**Provides to:**
- Telegram-notifications (`6237fdea`)

