# Contributing to MarketingLies

Thanks for helping keep the stamp ridiculous and the joke pointed at the claims.

## Adding a stamp-worthy claim

If you want to add examples for the static catalog, they live in `data/lies.json` as a flat JSON array. Each entry is an object with the following fields:

```json
{
  "claim": "AI-powered threat detection blocks 99.9% of attacks",
  "source_url": "https://example.com/product",
  "control_family": "CA",
  "vibes_rating": 4,
  "notes": "The 'AI' is a regex. The 99.9% is unsourced. The 0.1% would have been more interesting."
}
```

Field details:

- `claim` (string, required) — the security claim, copied as faithfully as possible.
- `source_url` (string, required) — a URL where the claim appears (homepage, product page, pitch deck, vendor questionnaire). Screenshots welcome in the PR, but the URL is the primary record.
- `control_family` (string, required) — one of `QN`, `CP`, `CR`, `CA`, `SO`, `TS`. See the README for definitions.
- `vibes_rating` (integer 1–5) — 1 is a mild fib, 5 is an unhinged whopper.
- `notes` (string, optional) — additional context (what the actual evidence looks like, what's quietly missing, scope gaps).

## Opening a PR

1. Fork the repo.
2. Add your entry as a new object in the `data/lies.json` array.
3. Open a PR with a one-line summary of the claim and where it came from.

## Code of conduct

Be cool. Don't dox anyone. The satire targets the *claim*, not the human who wrote it — most of the time a marketer was handed a feature list and told to make it sound trustworthy. If a claim mentions a specific named individual, think twice before adding it. If the individual *is* the claim (a founder personally vouching for their security posture, an exec making a public claim about their stack on stage), that's fair game.
