# Contributing to MarketingLies

Thanks for helping document the wild claims security and compliance marketing teams commit to the public web.

## Adding a lie

Lies live in `data/lies.json` as a flat JSON array. Each entry is an object with the following fields:

```json
{
  "claim": "SOC 2 Type II compliant",
  "source_url": "https://example.com/trust",
  "control_family": "CR",
  "vibes_rating": 4,
  "notes": "Report dated 2022, scope was a single landing page, sold as enterprise-grade trust signal."
}
```

Field details:

- `claim` (string, required) — the security claim, copied as faithfully as possible.
- `source_url` (string, required) — a URL where the claim appears (trust center, landing page, vendor questionnaire). Screenshots welcome in the PR, but the URL is the primary record.
- `control_family` (string, required) — one of `QN`, `CP`, `CR`, `CA`, `SO`, `TS`. See the README for definitions.
- `vibes_rating` (integer 1–5) — 1 is a mild fib, 5 is an unhinged whopper.
- `notes` (string, optional) — additional context (scope of the cert, methodology gaps, who the auditor actually was).

## Opening a PR

1. Fork the repo.
2. Add your entry as a new object in the `data/lies.json` array.
3. Open a PR with a one-line summary of the claim and where it came from.

## Code of conduct

Be cool. Don't dox anyone. The satire targets the *claim*, not the human who wrote it — most of the time a marketing person was handed a checklist from an automated compliance platform and asked to "make it sound trustworthy." If a claim mentions a specific named individual, think twice before submitting. If the individual *is* the claim (a founder personally vouching for their security posture, a CISO making a public claim about their stack), that's fair game.
