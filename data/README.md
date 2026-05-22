# data/

The catalog of cybersecurity marketing lies.

## Files

- `lies.json` — the array of entries. Each entry follows the schema described in the top-level `CONTRIBUTING.md`.

## Schema

Each entry in `lies.json` is an object with these fields:

| field | type | required | description |
| --- | --- | --- | --- |
| `claim` | string | yes | The security claim, copied faithfully. |
| `source_url` | string | yes | A URL where the claim appears. |
| `control_family` | string | yes | One of `QN`, `CP`, `CR`, `CA`, `SO`, `TS`. |
| `vibes_rating` | integer 1–5 | yes | 1 = mild fib, 5 = unhinged whopper. |
| `notes` | string | no | Context, evidence gaps, or commentary. |

## Example entry

```json
[
  {
    "claim": "AI-powered threat detection blocks 99.9% of attacks",
    "source_url": "https://example.com/product",
    "control_family": "CA",
    "vibes_rating": 4,
    "notes": "The 'AI' is a regex with a system prompt. The 99.9% is unsourced. The 0.1% is doing all the work."
  }
]
```

Add new entries as additional objects in the top-level array.
