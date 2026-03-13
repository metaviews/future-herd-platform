# Agent Architecture

Future Herd uses specialized AI agents as transparent facilitators. Agents do not make decisions. They synthesize, translate, summarize, and surface patterns.

Every agent has a defined role, constrained authorities, and transparent logs. Every agent action is auditable. Agent prompts and system instructions are stored in this directory and are part of the open source codebase. No black boxes.

Agents planned for development:

- Synthesis Agent — condenses discussion threads into structured summaries
- Translation Agent — makes content accessible across languages
- Moderation Agent — first-pass content moderation with human override
- Plain Language Agent — translates policy and technical content into accessible language
- Pattern Detection Agent — surfaces emerging trends and shifting sentiment
- Social Media Monitoring Agent — connects platform to external conversations

Later phases add:

- Scenario Modeling Agent — helps participants understand consequences of different positions
- Bridge-Building Agent — identifies potential areas of compromise between divided clusters
- Institutional Memory Agent — surfaces organizational history relevant to current deliberations

Agent runtime is provider-agnostic. The architecture supports Anthropic, OpenAI, and local open-source models. Agent definitions in this directory will include system prompts, authority constraints, and input/output specifications for each agent.
