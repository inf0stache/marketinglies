# marketinglies.lol

A satirical static site about unverified marketing claims. Anyone can write "AI-powered," "trusted by thousands," or "99.99% uptime" on a landing page and nobody checks. MarketingLies is a public catalog of those claims paired with the **MarketingLies Verification Standard (ML-VS)** — a SOC 2-style framework that maps each claim on a site to the evidence backing it. The joke is also a real proposal: if you can't produce the artifact, you don't get the stamp.

## Live site

https://marketinglies.lol

## The ML-VS concept

The MarketingLies Verification Standard defines six control families. To earn the "Protected by MarketingLies" stamp, every claim on a site must be classifiable into one of these families and backed by evidence.

- **QN — Quantitative Claims.** Numbers must be reproducible. ("10,000+ users" requires a query and a timestamp.)
- **CP — Comparative Claims.** Benchmarks must be cited. ("Faster than X" requires a methodology link.)
- **CR — Credential Claims.** Certifications must be current. ("SOC 2 compliant" requires a report date.)
- **CA — Capability Claims.** Features must actually ship. ("AI-powered" requires a description of the model.)
- **SO — Social Proof.** Logos require written permission from the named party.
- **TS — Testimonials.** Quotes must be attributable to a real person with a real title.

## Contributing

Three ways to help:

1. **Submit lies.** Open a PR adding entries to `data/lies.json`. See `CONTRIBUTING.md` for the schema.
2. **Propose new control families.** If you spot a class of claim that doesn't fit QN / CP / CR / CA / SO / TS, open an issue.
3. **Improve the stamp embed.** The "Protected by MarketingLies" stamp is currently inline in `index.html`. A standalone embeddable version (so other sites can carry the stamp) is a good next step.

## Local development

Single static HTML file. No build step.

```
python3 -m http.server
```

Or just open `index.html` in a browser.

## License

MIT. See `LICENSE`.

## Credit

Built by Oscar Sanchez Jr. — **inf0stache** on the usual channels.
