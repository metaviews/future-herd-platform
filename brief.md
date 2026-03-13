# Future Herd — Repository Initialization Brief

Feed this document to Claude Code to initialize the repo structure. It assumes you have already created the GitHub repo and cloned it locally.

---

## Context

Future Herd is an open source, agent-driven decision-making platform for agricultural organizations and rural communities. It draws on Decidim (structured participatory governance) and Polis (opinion-mapping through dimensionality reduction) and extends them with an AI agent layer, a peer-driven trust and standing system, and deep ecosystem integration.

The project is backed by the Agricultural Adaptation Council (AAC) and builds out of an existing initiative at thefutureherd.ca (podcast + intelligence digest for agricultural leaders).

The repo is being initialized before any code is written. The first phase is documentation, architecture decisions, and design. Code comes later. The repo needs to be structured to support both — and to be legible to contributors, stakeholders, and the public from day one.

## License

AGPL-3.0. This is a deliberate choice: it ensures that any deployment of Future Herd as a service must keep modifications open. Create the LICENSE file with the full AGPL-3.0 text.

## Repository Structure

Create the following directory structure:

```
future-herd/
├── LICENSE                          # AGPL-3.0
├── README.md                        # Project overview and orientation
├── CONTRIBUTING.md                   # How to contribute
├── CODE_OF_CONDUCT.md               # Community standards
├── docs/
│   ├── roadmap.md                   # Main technical roadmap (I will provide this file)
│   ├── architecture/
│   │   └── README.md                # Index of architecture decision records
│   ├── design/
│   │   └── README.md                # Index of design documents
│   └── research/
│       └── README.md                # Index of research and reference material
├── specs/
│   ├── api/
│   │   └── README.md                # API specification (future)
│   └── data-model/
│       └── README.md                # Data model specification (future)
├── src/                             # Source code (future)
│   └── .gitkeep
├── agents/                          # Agent definitions, prompts, and configurations
│   └── README.md                    # Agent architecture overview and index
└── .github/
    ├── ISSUE_TEMPLATE/
    │   ├── architecture-decision.md
    │   ├── feature-proposal.md
    │   └── bug-report.md
    └── PULL_REQUEST_TEMPLATE.md
```

## File Contents

### README.md

Write a README that covers:

1. **Opening statement.** Use this text verbatim as the opening:

> Our food system is the result of a wide range of decisions that are made by people and producers throughout the agricultural and food supply chain. A society that neither understands these decisions nor has the ability to participate in them is not going to be healthy or democratic. Civic literacy and food literacy are inseparable and part of the same cultural foundation for any aspiring democratic society.

2. **What Future Herd is.** A concise description: modern participation infrastructure for agricultural organizations and rural communities. Open source. Agent-assisted. Built for the realities of rural connectivity and the speed of today's information environment. Draws on Decidim and Polis. Not a social network, not a forum — structured decision-making infrastructure.

3. **Core design principles.** List these as a short section (not a bullet-heavy list — write them as short paragraphs):
   - **Open participation with identity integrity.** Anyone affected by agricultural decisions can participate. No one can participate twice. Organizational affiliation is visible and meaningful but not a gate.
   - **Transparency by default.** Every agent action is logged and auditable. Every deliberation history is preserved. Participation data flows to leadership as structured insight, not filtered summaries.
   - **Peer-driven trust and standing.** An alternative path to standing that is open to anyone, based on peer recognition of quality contributions — not volume, not institutional position.
   - **Ecosystem integration from day one.** The platform connects to where conversations already happen — social media, podcasts, newsletters, news — rather than trying to replace them. Every output is shareable. Every input can come from anywhere.
   - **Rural-first infrastructure.** Offline-capable. Channel-agnostic messaging. Low-bandwidth by design. Tested on the devices and connections people actually have.
   - **Strengthens authority by making it measurable.** The platform does not replace boards, elections, or formal governance. It gives them better information and documented mandates.

4. **Project status.** The project is in the documentation and architecture phase. No code has been written yet. The roadmap is in `docs/roadmap.md`. Contributions to architecture decisions, design documents, and research are welcome.

5. **How to get involved.** Point to CONTRIBUTING.md. Mention the Future Herd podcast at thefutureherd.ca. Note that the project is backed by the Agricultural Adaptation Council.

6. **License.** AGPL-3.0 — link to LICENSE file, with a one-sentence explanation of why (ensures modifications remain open even when deployed as a service).

Style notes for the README:
- No emoji
- No badges (yet — add them when there's something to badge)
- Warm but direct tone. This is infrastructure for democratic participation, not a startup pitch.
- Keep it under 200 lines. People should be able to read the whole thing in a few minutes.

### CONTRIBUTING.md

Write a contributing guide that covers:

- **The project is in early stage.** Right now the most valuable contributions are: architecture decision records, design critiques, research references, and domain expertise from people who work in agricultural organizations.
- **How to propose an architecture decision.** Use the architecture-decision issue template. Describe the decision to be made, the options considered, the recommended approach, and the reasoning. ADRs are discussed in issues before being merged as documents.
- **How to contribute design work.** Wireframes, user flow diagrams, and interaction designs go in `docs/design/`. Open an issue first to discuss the scope.
- **How to contribute research.** Relevant research, case studies, and reference material go in `docs/research/`. This includes existing work on participatory governance, opinion-mapping algorithms, rural technology adoption, and agricultural organization governance.
- **Code contributions (future).** Code contributions will be welcome once the architecture is established. The tech stack and development environment will be documented before code contributions are solicited.
- **Communication.** For now, discussion happens in GitHub Issues and Pull Requests. As the community grows, additional channels may be established — using Future Herd itself when it is functional.
- **Review process.** All contributions go through pull request review. Architecture decisions require discussion in an issue before a PR is opened.

### CODE_OF_CONDUCT.md

Use the Contributor Covenant v2.1 (https://www.contributor-covenant.org/version/2/1/code_of_conduct/) as the base. Add a preamble that connects it to the project's values:

> Future Herd is built on the principle that open, structured participation produces better decisions than closed, exclusive processes. That principle applies to the project itself. We expect all contributors to engage with the same respect, transparency, and good faith that we are building into the platform.

For the enforcement contact, use a placeholder: `[ENFORCEMENT CONTACT — TO BE ESTABLISHED]`. Jesse will fill this in.

### docs/ README files

Each README in the docs subdirectories should be a brief index page:

- `docs/architecture/README.md`: "Architecture Decision Records for Future Herd. ADRs document significant technical and design decisions. See CONTRIBUTING.md for how to propose a new ADR." Then list: "No ADRs have been recorded yet. The following decisions are pending: identity integrity mechanism, data model, opinion-clustering algorithm, trust and standing mechanics, PWA framework, messaging abstraction layer, ecosystem integration approach."

- `docs/design/README.md`: "Design documents for Future Herd. Wireframes, user flows, and interaction designs." Then: "No design documents have been created yet. Priority design work includes: opinion mapping participant experience, pulse survey flow, emergent issue flagging, peer recognition mechanics, participant profile and standing display."

- `docs/research/README.md`: "Research and reference material informing Future Herd's design." Then: "Key areas of research include: Polis algorithm and opinion-clustering approaches, Decidim's participatory governance model, peer recognition and trust systems (Stack Exchange, Wikipedia, etc.), rural technology adoption patterns, agricultural organization governance structures in Canada, existing civic tech platforms and their adoption challenges."

### agents/README.md

Write an overview of the agent architecture:

- Future Herd uses specialized AI agents as transparent facilitators. Agents do not make decisions. They synthesize, translate, summarize, and surface patterns.
- Every agent has a defined role, constrained authorities, and transparent logs. Every agent action is auditable.
- Agent prompts and system instructions are stored in this directory and are part of the open source codebase. No black boxes.
- Agents planned for development: Synthesis Agent, Translation Agent, Moderation Agent, Plain Language Agent, Pattern Detection Agent, Social Media Monitoring Agent. Later phases add: Scenario Modeling Agent, Bridge-Building Agent, Institutional Memory Agent.
- Agent runtime is provider-agnostic. The architecture supports Anthropic, OpenAI, and local open-source models.

### specs/ README files

- `specs/api/README.md`: "API specification for Future Herd. The API is not yet defined. It will be documented here using OpenAPI format before implementation begins. The API-first principle means every interaction with the platform goes through a documented API — the web app, messaging integrations, and ecosystem tools all use the same interface."

- `specs/data-model/README.md`: "Data model specification for Future Herd. The data model is not yet defined. It will be documented here before implementation begins. Key entities include: Participant, Organization, Affiliation, Topic, Statement, Vote, Proposal, Amendment, Recognition, Standing, AgentAction."

### .github/ISSUE_TEMPLATE/architecture-decision.md

```yaml
---
name: Architecture Decision
about: Propose a significant technical or design decision
title: "ADR: [Decision Title]"
labels: architecture, decision
---
```

Then the body template:

```
## Decision

What decision needs to be made?

## Context

What is the background? What constraints or requirements are relevant?

## Options Considered

### Option A: [Name]
Description, trade-offs.

### Option B: [Name]
Description, trade-offs.

### Option C: [Name] (if applicable)
Description, trade-offs.

## Recommendation

Which option and why?

## Consequences

What follows from this decision? What does it enable or constrain?
```

### .github/ISSUE_TEMPLATE/feature-proposal.md

```yaml
---
name: Feature Proposal
about: Propose a new feature or capability
title: "Feature: [Title]"
labels: feature, proposal
---
```

Body:

```
## Summary

One-paragraph description of the proposed feature.

## Motivation

What problem does this solve? Who benefits?

## Design

How should this work? Include interaction descriptions, data flow, or mockups as appropriate.

## Relationship to Roadmap

Which phase and section of the roadmap does this relate to?

## Open Questions

What needs to be resolved before this can be implemented?
```

### .github/ISSUE_TEMPLATE/bug-report.md

```yaml
---
name: Bug Report
about: Report a bug or issue
title: "Bug: [Title]"
labels: bug
---
```

Body:

```
## Description

What happened?

## Expected Behavior

What should have happened?

## Steps to Reproduce

1.
2.
3.

## Environment

- Device/OS:
- Browser/Client:
- Connection type:
```

### .github/PULL_REQUEST_TEMPLATE.md

```
## What does this PR do?

## Related Issues

Closes #

## Type of Change

- [ ] Documentation (roadmap, ADR, design doc, research)
- [ ] Specification (API, data model)
- [ ] Agent definition (prompts, configuration)
- [ ] Code (feature, fix, refactor)
- [ ] Infrastructure (CI/CD, deployment, tooling)

## Checklist

- [ ] I have read CONTRIBUTING.md
- [ ] This change is consistent with the project's design principles
- [ ] Documentation has been updated if needed
```

## After Initialization

Once the structure is created, initialize a git repo if not already done, stage all files, and make an initial commit with the message:

```
Initial repository structure: documentation, specs, and community foundations

Establishes project structure for the documentation and architecture
phase. No code yet — this is the framework for collaborative design
of an open source participation platform for agricultural communities.
```

Do NOT push — I will review the local state before pushing to the remote.

## Important Notes

- Do not create any application code. This is a documentation and architecture repo at this stage.
- Do not add any CI/CD configuration yet. That comes when there is code to test.
- Do not add dependency files (package.json, requirements.txt, etc.) yet.
- The roadmap.md file in docs/ will be added separately — just create a placeholder that says "Roadmap document will be added from the current working draft."
- Use consistent formatting: Markdown, no trailing whitespace, single newline at end of file.