# marketinglies.lol

A satirical static site about cybersecurity marketing claims. Any vendor can slap "AI-powered threat detection," "blocks 99.9% of attacks," "quantum-safe encryption," or "autonomous SOC" on a landing page — and nobody checks. The pattern is everywhere: claim something impressive, point at a badge, move on. MarketingLies is a public catalog of those claims. See one in the wild, slap the badge on it, move on. Like ShamWow, but for security marketing.

## Live site

https://marketinglies.lol

## The ML-VS concept

The MarketingLies Verification Standard defines six control families. To earn the "Protected by MarketingLies" stamp, a claim must be classifiable into one of these families and backed by evidence. (To not earn it, just keep doing what most security marketing already does.)

- **QN — Quantitative Claims.** Numbers must be reproducible. ("Blocks 99.9% of threats" requires a methodology, not vibes.)
- **CP — Comparative Claims.** Benchmarks must be cited. ("Most secure" requires a comparison and a citation.)
- **CR — Credential Claims.** Certifications must be current and in scope. (A 2022 attestation for a different product doesn't count.)
- **CA — Capability Claims.** Features must actually ship. ("AI-powered" requires a description of what the AI actually does. "Autonomous SOC" requires more than one human and a Slack bot.)
- **SO — Social Proof.** Logos require written permission. ("Trusted by Fortune 500" requires the actual Fortune 500 company saying so.)
- **TS — Testimonials.** Quotes must be attributable to a real person with a real title.

## Contributing

Three ways to help:

1. **Submit lies.** Open a PR adding entries to `data/lies.json`. See `CONTRIBUTING.md` for the schema.
2. **Propose new control families.** Spotted a class of security claim that doesn't fit QN / CP / CR / CA / SO / TS? Open an issue.
3. **Improve the stamp embed.** The "Protected by MarketingLies" stamp is currently inline in `index.html`. A standalone embed (so anyone can slap the badge on anything) is the obvious next step.

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
