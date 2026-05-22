# data/

The catalog of security marketing lies.

## Files

- `lies.json` — the array of entries. Each entry follows the schema described in the top-level `CONTRIBUTING.md`.

## Schema

Each entry in `lies.json` is an object with these fields:

| field | type | required | description |
| --- | --- | --- | --- |
| `claim` | string | yes | The security/compliance claim, copied faithfully. |
| `source_url` | string | yes | A URL where the claim appears (trust center, landing page, etc.). |
| `control_family` | string | yes | One of `QN`, `CP`, `CR`, `CA`, `SO`, `TS`. |
| `vibes_rating` | integer 1–5 | yes | 1 = mild fib, 5 = unhinged whopper. |
| `notes` | string | no | Context, evidence, or commentary. |

## Example entry

```json
[
  {
    "claim": "SOC 2 Type II compliant",
    "source_url": "https://example.com/trust",
    "control_family": "CR",
    "vibes_rating": 4,
    "notes": "Report dated 2022. Scope was a single marketing landing page, not the actual product. Sold on the homepage as 'enterprise-grade trust.'"
  }
]
```

Add new entries as additional objects in the top-level array.
