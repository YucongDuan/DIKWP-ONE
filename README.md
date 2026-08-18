# DIKWP ONE

[中文说明](README.zh-CN.md)

## One AI answer. One accountable action. One result.

**DIKWP ONE is the public front door to a 363-repository research portfolio—compressed into one tool people can use in 60 seconds.**

Paste an AI answer. DIKWP ONE produces an Action Card that makes five things explicit:

1. what is grounded;
2. what is still uncertain;
3. what we understand now;
4. who is affected;
5. the one next action, owner and review point.

After the action, record an Outcome Receipt: what happened, who benefited or was harmed, what must be corrected, and what happens next.

No account. No cloud upload. No framework lecture before value.

![DIKWP ONE preview](docs/preview.png)

## Try it in 30 seconds

Open `index.html` directly, or run:

```bash
python run.py serve
```

Then visit `http://127.0.0.1:8081`.

CLI:

```bash
python run.py analyze examples/research_claim.json --out outputs/research_claim
python run.py close outputs/research_claim/action_card.json examples/research_outcome.json --out outputs/research_claim
python run.py portfolio data/portfolio_snapshot_2026-08-17.json
python run.py repo-gate examples/new_repo_proposal.json
python run.py selftest
```

## Why this repository exists

The public YucongDuan profile showed **363 repositories** on 17 August 2026. The problem is no longer idea generation. The bottleneck is attention, adoption, maintenance and material return.

DIKWP ONE is the reset:

- one pinned public entry;
- one promise;
- one browser tool;
- one canonical issue queue;
- one result loop;
- one route to a scoped paid pilot.

See [`PORTFOLIO_363_ANALYSIS.md`](PORTFOLIO_363_ANALYSIS.md).

## The tool

The public language is ordinary; the DIKWP structure remains underneath:

| Public question | DIKWP position |
|---|---|
| What is grounded? | D |
| What differs or remains unknown? | I |
| What do we understand now? | K |
| Who is affected and what matters? | W |
| What happens next? | P |

An Action Card is not the end. The Outcome Receipt closes the loop:

```text
answer → action → owner → result → affected-party feedback → correction
```

## Four ways to create return

1. **Use it** — build a real Action Card.
2. **Prove it** — report what changed, including failure.
3. **Maintain it** — own one test, translation or integration.
4. **Fund a pilot** — bring one workflow and one measurable outcome.

The project does not run a free private support queue. Structured work enters public issues or a scoped pilot.

## Three pilot wedges

DIKWP ONE remains one product, but organizations can apply it to three high-value workflows:

- **AI action review** — review an agent answer before tool execution;
- **evidence-to-decision** — turn research, policy or procurement evidence into one owned action;
- **institutional handoff** — preserve affected parties, review dates and outcome correction across teams.

See [`PILOT.md`](PILOT.md) and [`COMMERCIAL_SERVICES.md`](COMMERCIAL_SERVICES.md).

## Adversarial attention design

This repository assumes that:

- most people will not inspect 363 repositories;
- complex names lose to familiar outcomes;
- admiration does not become adoption automatically;
- free support expands until the founder burns out;
- useful ideas may be copied while origin is omitted;
- institutions prefer fixed scope, named owners and measurable outcomes.

The countermeasures are implemented in the repository—not left as advice. See [`ATTENTION_THREAT_MODEL.md`](ATTENTION_THREAT_MODEL.md).

## Founder-energy compact

For 60 days after publication:

- do not create another public repository for a related idea;
- route new ideas to Issues or modules here;
- accept a new flagship only if it brings a new external owner, adopter, dataset, experiment or paid workflow;
- publish one result every week, not one new architecture every day.

See [`FOUNDER_ENERGY_COMPACT.md`](FOUNDER_ENERGY_COMPACT.md).

## Live portfolio sync

The release contains a dated public snapshot. To refresh from GitHub when network access is available:

```bash
python scripts/sync_github.py --user YucongDuan --out data/portfolio_live.json
python run.py portfolio data/portfolio_live.json
```

The sync uses GitHub's public REST endpoint and does not require a token for ordinary public use, subject to rate limits.

## Public support and result reporting

- Support boundary: [`SUPPORT.md`](SUPPORT.md)
- Public adoption registry: [`ADOPTION_REGISTRY.md`](ADOPTION_REGISTRY.md)
- Weekly result template: [`RESULT_REPORT_TEMPLATE.md`](RESULT_REPORT_TEMPLATE.md)

Generate a weekly result note from Outcome Receipts:

```bash
python run.py weekly-report outputs --week-ending 2026-08-23 --out outputs/weekly_result
```

## Origin and attribution

DIKWP ONE is a community-facing implementation derived from Yucong Duan's DIKWP research on Data, Information, Knowledge, Wisdom and Purpose.

- GitHub: https://github.com/YucongDuan
- Research profile: https://www.researchgate.net/profile/Yucong-Duan
- Machine-readable origin: [`data/origin.json`](data/origin.json)
- Citation: [`CITATION.cff`](CITATION.cff)

Every exported card and receipt includes an origin field and a content digest.

## License

Apache License 2.0. The license does not grant a trademark right or permission to imply endorsement. Organization-specific implementation, training and maintained deployment can be commissioned separately.
