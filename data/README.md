# data/

The catalog of marketing lies.

## Files

- `lies.json` — the array of entries. Each entry follows the schema described in the top-level `CONTRIBUTING.md`.

## Schema

Each entry in `lies.json` is an object with these fields:

| field | type | required | description |
| --- | --- | --- | --- |
| `claim` | string | yes | The marketing claim, copied faithfully. |
| `source_url` | string | yes | A URL where the claim appears. |
| `control_family` | string | yes | One of `QN`, `CP`, `CR`, `CA`, `SO`, `TS`. |
| `vibes_rating` | integer 1–5 | yes | 1 = mild fib, 5 = unhinged whopper. |
| `notes` | string | no | Context, evidence, or commentary. |

## Example entry

```json
[
  {
    "claim": "9 out of 10 dentists recommend this",
    "source_url": "https://example.com/toothpaste-landing",
    "control_family": "QN",
    "vibes_rating": 4,
    "notes": "The cited survey sampled 12 dentists, all employed by the manufacturer's parent company."
  }
]
```

Add new entries as additional objects in the top-level array.
