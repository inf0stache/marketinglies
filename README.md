# marketinglies.lol

A satirical static site about cybersecurity marketing claims and the rise of automated SOC 2. Any startup can slap a "SOC 2 Type II" badge, a "zero-trust architecture" line, and a "bank-grade encryption" claim on their landing page — and nobody checks. Vanta, Drata, Secureframe and friends made it possible to "get compliant" in two weeks by ticking boxes a script generates. MarketingLies is a public catalog of those claims paired with the **MarketingLies Verification Standard (ML-VS)** — a deliberately absurd parody of an automated compliance platform. If you can produce evidence, you get the stamp. If you can't, you get it anyway, because nobody checks. That's the joke. That's also the industry.

## Live site

https://marketinglies.lol

## The ML-VS concept

The MarketingLies Verification Standard defines six control families. The framing is a parody of SOC 2 Trust Service Criteria, but applied to the kind of claims security marketing teams actually make.

- **QN — Quantitative Claims.** Numbers must be reproducible. ("99.99% uptime" requires actual SLO data, not vibes.)
- **CP — Comparative Claims.** Benchmarks must be cited. ("Most secure" requires a methodology.)
- **CR — Credential Claims.** Certifications must be current and in scope. ("SOC 2 Type II" requires a recent report, not a 2022 attestation for a different product.)
- **CA — Capability Claims.** Features must actually ship. ("Zero-trust architecture" requires a description of what was actually built.)
- **SO — Social Proof.** Logos require written permission. ("Trusted by Fortune 500" requires the actual Fortune 500 company saying so.)
- **TS — Testimonials.** Quotes must be attributable to a real CISO with a real title.

## Contributing

Three ways to help:

1. **Submit lies.** Open a PR adding entries to `data/lies.json`. See `CONTRIBUTING.md` for the schema.
2. **Propose new control families.** Spotted a class of security claim that doesn't fit QN / CP / CR / CA / SO / TS? Open an issue.
3. **Improve the stamp embed.** The "Protected by MarketingLies" stamp is currently inline in `index.html`. A standalone embed so other trust centers can carry the stamp is a good next step.

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
