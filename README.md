# AI in Production

Engineering talks on building AI agents that actually ship — by [Tuhin Kanti Sharma](https://www.linkedin.com/in/tuhin-kanti-sharma/), Principal Software Engineer, Development Experience.

**Live:** https://tuhinkanti.github.io/ai-in-production/

Each talk lives in its own folder as a self-contained [reveal.js](https://revealjs.com/) deck. Press <kbd>S</kbd> in any deck to open speaker notes.

## Talks

### [How We Built an Autonomous Agent to Optimize Millions in Capacity at Salesforce](autonomous-capacity-agent/slides/tech-talk-v1.html)

`autonomous-capacity-agent/`

Analysis of a large Kubernetes fleet revealed that most containers ran at under 20% of their requested CPU — a significant share of cloud spend paying for compute nobody used. This talk walks through building an autonomous AI agent that right-sizes Helm charts safely, at scale, across thousands of repositories: what worked, what failed, and the engineering patterns that made the agent reliable in production.

The arc:

1. **The capacity problem** — config sprawl across thousands of repositories.
2. **v1 → v2** — where prompt-driven and sub-agent architectures broke.
3. **The reframe** — Agent = Model + Harness.
4. **Two kinds of work** — reasoning vs. structured computation (and where ILP fits).
5. **Context engineering** — iterating on the harness to a plan you can trust, the same plan every run.

## Running locally

```bash
python3 -m http.server 8000
# then open http://localhost:8000/
```

## Links

- LinkedIn — https://www.linkedin.com/in/tuhin-kanti-sharma/
- Blog — https://engineering.salesforce.com/author/tuhin-sharma/
- Newsletter — *SWE in the Age of AI* — https://www.linkedin.com/newsletters/swe-in-the-age-of-ai-7342972190482472960/

## License

Licensed under the [Apache License 2.0](LICENSE). Copyright 2026 Tuhin Kanti Sharma. The views expressed are the author's own.
