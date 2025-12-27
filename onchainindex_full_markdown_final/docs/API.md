# OnChainIndex API (v1)

The OnChainIndex API provides read-only access to rankings, dApp profiles, and historical snapshots.

## Principles
- Read-only
- Public
- Rate-limited
- Usage-based, not promotional

## Endpoints

### Get Rankings
GET /api/v1/rankings/{type}

Types:
- most-active
- most-used
- trending

### Get dApp Profile
GET /api/v1/dapps/{slug}

### Get Historical Rankings
GET /api/v1/history/{date}

## Example Response
```json
{
  "rank": 3,
  "name": "Jupiter",
  "category": "DeFi",
  "uaw_7d": 182391,
  "tx_7d": 3200000,
  "verified": true
}
```

## Attribution
Use of the API requires attribution to OnChainIndex.
