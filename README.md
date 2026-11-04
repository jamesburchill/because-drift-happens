# Because Drift Happens™

Because Drift Happens is James Burchill’s public doctrine for recognizing and responding when businesses, processes, assumptions, and technology drift from their original intent. The technical framework applies this thinking to intelligent and autonomous systems, with vocabulary, principles, patterns, and architectural concepts for keeping them observable, accountable, and aligned.

This is a doctrine/framework repository, not a product repository. It is intended to be the canonical public source for the language and operating model behind drift-aware system design, federated agent governance, runtime control planes, and coherent autonomous AgentOps.

## What This Is

Because Drift Happens maintains a broad Drift Doctrine and a technical framework applying it to intelligent and autonomous systems. Readers can follow a [business and organizational path](docs/reading-map.md#business-and-organizational-drift) or a [technical systems and AI governance path](docs/reading-map.md#technical-systems-and-ai-governance).

It provides:

- A shared vocabulary for drift, coherence, governance, federation, intervention, and runtime control.
- Principles for designing autonomous operations that can observe, regulate, and adapt.
- Conceptual architecture patterns for control planes, governance checkpoints, vetoes, escalation paths, and audit trails.
- Failure patterns that help teams recognize drift before it becomes systemic.
- Reference examples that explain governance concepts without binding them to a specific vendor or product.

## What This Is Not

This repository is not:

- A software product.
- A vendor framework.
- A claims-based AI safety manifesto.
- A compliance checklist.
- A substitute for domain-specific risk management.
- A finished doctrine.

The work here is deliberately public, evolving, and conceptual. It should become more precise over time as the language, patterns, and examples are tested against real operational systems.

## Core Premise

Drift is the default.

Autonomous drift is inevitable.

Federated drift compounds.

Awareness reveals drift.

Alignment reduces drift.

Coordination contains drift.

The [doctrine](docs/doctrine.md) contains the canonical six-line form and its explanation.

## Why This Matters Now

Autonomous systems, agents, workflows, organisations, and infrastructure all drift over time. Intent changes. Context decays. Dependencies shift. Data ages. Policies are reinterpreted. Tools behave differently under load. People change the operating environment faster than documentation can keep up.

Multi-agent systems increase this risk because each agent may work from partial context, optimise locally, act asynchronously, delegate recursively, and form indirect dependencies through shared tools, memory, queues, and state. The result can be useful adaptation, but it can also produce alignment decay, authority confusion, policy bypass, and silent degradation.

Because Drift Happens positions the problem around operational coherence rather than vague "AI safety." The question is not whether autonomy is good or bad. The question is whether an autonomous system can remain observable, accountable, governable, and aligned with its declared intent as conditions change.

## Key Concepts

- **Drift:** The movement of system behaviour, state, decisions, or interpretation away from intended operating bounds.
- **Coherence:** Regulated alignment across intent, execution, feedback, and adaptation.
- **Operational coherence:** The ability of a running system to remain understandable, governable, and effective under change.
- **Control plane:** The layer that observes, constrains, coordinates, and intervenes above individual agents and workflows.
- **Governance plane:** The part of the control plane responsible for policy, authority, auditability, accountability, and escalation.
- **Intervention:** A deliberate action that pauses, redirects, rejects, rolls back, contains, or escalates an autonomous process.
- **Federation:** A model where multiple agents, services, teams, or systems retain local autonomy while participating in a larger operating structure.

## Repository Map

- [`docs/`](docs/) contains the doctrine, definitions, principles, failure patterns, examples, diagram plans, RFCs, and conceptual architecture notes.
- [`mkdocs.yml`](mkdocs.yml) configures the public documentation site.
- [`.github/`](.github/) contains issue and pull request templates for public contributions.

## Website

The public site runs at:

https://becausedrifthappens.com/

The site is built with MkDocs and deployed to GitHub Pages.

## Related Work

- [JamesBurchill.com](https://jamesburchill.com/) is the author’s identity, work, and contact hub.
- [The Vault](https://vault.jamesburchill.com/) holds essays and field notes; [Governing Intelligent Systems](https://vault.jamesburchill.com/governing-intelligent-systems/) is its technical reading guide.
- [Driftinel](https://driftinel.com/) is a managed service in development applying this thinking to business monitoring. It helps owners spot slipping commitments and emerging problems with supporting evidence. Purchasing is not yet open.

Earlier implementation names (coherence-os, safeagent, vetoguard, and aired) were prospective references, not a verified catalogue of active projects. They do not define the doctrine or imply current availability.

## Status and Page Metadata

The six-line doctrine is the stable reference within an evolving public framework. Concepts and graphics are working interpretations, examples are hypothetical, and planned work is labelled separately. See the [reading map](docs/reading-map.md#content-maturity) for the maturity definitions.

Each documentation page has YAML front matter with a unique `title` and `description`, a `content_type`, and a `maturity` value. The shared template renders maturity labels, social metadata, and JSON-LD for the website, author, and page. Use `en-CA` for structured-data language and `en_CA` for Open Graph locale. Canonical URLs come from MkDocs; do not duplicate them in front matter or invent publication/review dates.

Allowed maturity values and their public explanations live in `mkdocs.yml` under `extra.maturity_labels`. Existing page URLs are retained, including the planned-diagrams backlog, which is linked from the diagrams overview rather than the primary navigation.

Validate with `python -m pip install -r requirements.txt` in an isolated environment, then `python -m mkdocs build --strict`. Check generated metadata, maturity labels, and internal links before publishing. A successful build does not establish that a deployment occurred.

## License

The doctrine, documentation, diagrams, and examples in this repository are licensed under Creative Commons Attribution 4.0 International. Future code, if added, may be licensed separately.

Because Drift Happens.
