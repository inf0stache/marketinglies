# Contributing to MarketingLies

Thanks for helping document the wild claims marketing departments commit to the public web.

## Adding a lie

Lies live in `data/lies.json` as a flat JSON array. Each entry is an object with the following fields:

```json
{
  "claim": "9 out of 10 dentists recommend this",
  "source_url": "https://example.com/page-where-the-claim-appears",
  "control_family": "QN",
  "vibes_rating": 4,
  "notes": "Optional context — how you found it, what the actual evidence looks like (or doesn't)."
}
```

Field details:

- `claim` (string, required) — the marketing claim, copied as faithfully as possible.
- `source_url` (string, required) — a URL where the claim appears. Screenshots welcome in the PR, but the URL is the primary record.
- `control_family` (string, required) — one of `QN`, `CP`, `CR`, `CA`, `SO`, `TS`. See the README for definitions.
- `vibes_rating` (integer 1–5) — 1 is a mild fib, 5 is an unhinged whopper.
- `notes` (string, optional) — additional context.

## Opening a PR

1. Fork the repo.
2. Add your entry as a new object in the `data/lies.json` array.
3. Open a PR with a one-line summary of the claim and where it came from.

## Code of conduct

Be cool. Don't dox anyone. The satire targets the *claim*, not the human who wrote it — most of the time the person who shipped a sketchy line was following orders, not setting strategy. If a claim mentions a specific named individual, think twice before submitting. If the individual *is* the claim (a founder's personal pitch, an influencer's product line), that's fair game.
