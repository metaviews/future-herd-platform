# Future Herd — Technical Roadmap

**Open source participation infrastructure for agricultural organizations**

Version 0.1 — March 2026

---

## Premise

Future Herd sits at the intersection of two proven approaches to collective intelligence — Decidim's structured participatory governance and Polis's opinion-mapping through dimensionality reduction — and extends them with an agent layer designed for the specific constraints and rhythms of agricultural communities.

The platform is not a social network. It is not a forum. It is a structured environment where participants — from organizational members to unaffiliated farmers to consumers to community members — can signal positions, observe where their community stands, and contribute to decisions that feed into (but do not replace) formal governance.

The agent layer is what distinguishes Future Herd from existing tools. Agents do not make decisions. They facilitate: synthesizing discussion threads into structured positions, bridging language barriers, detecting emerging fault lines before they calcify, and translating complex policy into plain language. Agents serve the participants, not the leadership — and their operations are transparent and auditable.

---

## Context: The Existing Future Herd Initiative

Future Herd is not starting from zero. The project builds out of an existing initiative (thefutureherd.ca) — a podcast and knowledge base for leaders in the agricultural sector, backed by the Agricultural Adaptation Council (AAC). The AAC is a meta-organization: it coordinates and supports other agri-food organizations across Ontario and beyond. This structural position is a significant strategic advantage.

Because the AAC sits above individual commodity boards, producer associations, and value-chain organizations, the Future Herd platform does not need to begin by recruiting a single pilot organization and hoping it works. Instead, the existing relationships and leadership audience provide a meta-pilot environment: agricultural leaders who already engage with Future Herd content can experiment with the platform's participation tools in the context of cross-sectoral questions about the future of agriculture itself.

This means the demo is the pilot is the product. Leaders from different organizations, representing different commodities and different positions in the value chain, can use Future Herd to deliberate on real questions facing the sector — and in doing so, they experience firsthand what the platform could do for their own memberships. The meta-pilot serves multiple purposes simultaneously: it generates genuine insight about the future of agriculture, it stress-tests the platform with sophisticated users who will find the bugs and missing features, it builds buy-in by letting leaders experience the tool rather than just hear about it, and it creates a visible demonstration of structured digital participation that organizations can point to when considering adoption.

The existing podcast and knowledge base also provide a natural content pipeline for the platform. Episodes and research that surface on thefutureherd.ca become context for deliberation topics. A podcast episode about supply management reform can lead directly to an opinion-mapping exercise where leaders signal where they stand on the key tensions raised. The media layer feeds the participation layer, and the participation layer generates insight that feeds back into the media layer.

---

Future Herd is composed of seven interdependent layers:

**1. Identity and Participation** — Open participation grounded in identity integrity. Anyone affected by agricultural decisions can participate — farmers, workers, consumers, community members, researchers, policy practitioners. Every participant is a verified unique person (one person, one voice). Organizational affiliation is a visible attribute that enriches the opinion map, not a gate that restricts entry. This is the layer that gives the platform its legitimacy: not by excluding voices, but by ensuring every voice is real and every affiliation is honest.

**2. Participation Engine** — The core interaction layer. Two primary modes drawn from Polis and Decidim respectively: opinion mapping (where participants vote agree/disagree/pass on short statements and clustering algorithms reveal natural groupings) and deliberation (where structured proposals move through stages from draft to formal consideration). A third mode — pulse surveys — provides rapid, lightweight sentiment checks on emerging issues.

**3. Trust and Standing** — A peer-driven layer that recognizes quality participation over time. Not gamification — not points for clicking buttons. A system where participants can recognize each other for contributions that make the platform meaningful: well-framed proposals, bridge-building statements, thoughtful dissent, clear explanations of complex issues. This layer acknowledges existing institutional hierarchies (organizational leadership has standing that comes from their role) while creating an alternative path to standing that is open to anyone. A consumer who consistently contributes thoughtful, well-received positions builds visible standing on the platform regardless of institutional affiliation. This is how "open to anybody" becomes structurally real rather than merely formally true.

**4. Agent Layer** — AI agents that serve specific facilitation functions. Not a chatbot. A set of specialized agents with defined roles, constrained authorities, and transparent logs. Every agent action is auditable. Agents synthesize, translate, summarize, and surface patterns. They do not advocate, recommend, or adjudicate.

**5. Governance Bridge** — The interface between participatory signals and formal decision-making structures. Boards and elected leadership receive structured reports: where consensus exists, where division lies, how positions have evolved, what the participation rate was. This layer ensures that Future Herd output is actionable within existing constitutional and bylaws frameworks.

**6. Ecosystem and Extension** — Future Herd does not exist in isolation. People are already discussing agricultural issues on social media, in podcasts, in newsletters, and in private groups. The ecosystem layer connects the platform to where those conversations are already happening — drawing people in, pushing structured insight out, and ensuring the platform remains relevant to the information environment participants actually inhabit. This is not a final phase to be added once the platform is mature. It is a design principle that shapes every phase, starting with the existing Future Herd podcast and intelligence digest as the initial connective tissue.

**7. Infrastructure and Access** — Designed for rural realities. Offline-capable progressive web app. Channel-agnostic messaging layer (SMS, WhatsApp, Signal, email, or whatever a given community actually uses). Low-bandwidth rendering. Accessibility across devices, connectivity levels, and technical literacy.

---

## Phase 0 — Foundation

**Objective:** Establish the core identity system, basic participation mechanics, and infrastructure capable of running the AAC meta-pilot — a cross-sectoral deliberation exercise with agricultural leaders that simultaneously serves as demonstration, stress test, and genuine decision-making platform.

### 0.1 Identity, Integrity, and Inclusive Participation

The hardest problem is the first one — but the problem is not "how do we restrict who gets in." The problem is "how do we ensure one person equals one voice, without gatekeeping who counts as a person worth hearing."

The agricultural sector's existing participation crisis is a crisis of exclusion. Membership in organizations is narrow. Engagement within those memberships is low. The vast majority of people affected by agricultural decisions — farmers who are not members of any board, agricultural workers, rural residents, consumers, processors, retailers, Indigenous communities with food sovereignty concerns — have no structured way to participate in the conversations that shape their food system. A platform that reproduces this exclusion by making organizational membership the price of entry is not solving the problem. It is digitizing it.

The design principle is: **open participation with identity integrity.** Anyone can participate. No one can participate twice. Organizational affiliation is visible and meaningful, but it is not a gate.

Critically, openness and organizational legitimacy are not in tension — they reinforce each other. An organization that has earned the trust of its membership and mobilized its people to participate on the platform benefits directly: their verified members show up as a visible, cohesive cohort. The organization's positions carry demonstrated weight because their members chose to participate, not because non-members were excluded. Legitimacy earned through mobilization is stronger than legitimacy claimed through gatekeeping.

For organizations where that capacity is less developed — where membership engagement is low, where trust between leadership and the base is thin — the platform becomes part of how those capabilities are built. Open participation lets leadership see what the broader community actually thinks, where their current membership sits within that landscape, and where the gaps lie. The process of using the platform — seeing how opinions cluster, watching how deliberations unfold, responding to emergent concerns — is itself a capacity-building exercise. Organizations learn to listen at scale, and participants learn that structured participation produces visible results. Over time, this cycle builds the trust and engagement that turns a weak organization into a strong one.

Design approach:

- **Identity integrity, not membership verification, is the foundation.** Every participant is a unique, verified person — one person, one account, one voice. The mechanism for establishing identity integrity is separate from the question of organizational membership. Options include email verification with duplicate detection, phone number verification, government ID verification for higher-assurance contexts, or organizational vouching. The key constraint is that one human being cannot operate multiple accounts. This is the anti-manipulation layer.

- **Organizational affiliation is an attribute, not a prerequisite.** Organizations can upload or sync membership rolls (CSV import initially, API integration later). When a participant's identity matches an organizational roll, their affiliation is confirmed and visible. But participants without any organizational affiliation can still create accounts, vote, submit statements, flag issues, and participate fully. Their contributions are marked as unaffiliated (or self-described, e.g., "dairy farmer, non-member" or "consumer, Ottawa").

- **The opinion map shows everyone.** This is where the architecture does its most important work. When a deliberation runs, the opinion map shows all participants — and organizational affiliation is a visible layer. Leadership can see where their verified members cluster, and they can also see where non-member farmers, workers, consumers, and community members cluster. An organization with strong membership mobilization will see its cohort as a distinct, well-populated cluster — a visible demonstration of the organization's capacity and relevance. An organization with weak engagement will see its members scattered or absent — a signal that capacity-building is needed. Either way, the full picture is more useful than a partial one.

- **Configurable visibility supports both open and internal needs.** Organizations can configure how affiliation layers are displayed. They can highlight their own membership's positions. They can filter views to focus on their members' responses for internal governance purposes. Public deliberations are open by default — this is where the platform's value as a broad listening tool is greatest. Organizations can also run internal-only deliberations when constitutionally appropriate (e.g., a bylaws amendment vote that is genuinely only for dues-paying members). The architecture supports both modes because both are legitimate. The key is that open participation is the default, and restriction is a deliberate choice for specific governance contexts, not the baseline assumption.

- **Self-described identity supports rich context.** Participants can self-describe their relationship to the agricultural system: commodity, region, role (producer, processor, worker, consumer, researcher, policy, etc.), years of experience. This self-described context appears alongside their contributions and enriches the opinion map's clustering. A cluster of "beef producers in Northern Ontario with 20+ years experience" that disagrees with a cluster of "new entrant diversified producers in Eastern Ontario" tells a different story than two anonymous blobs on a scatter plot.

- **Pseudonymous participation is available.** Participants can choose whether their name is visible to other participants, visible only to administrators, or fully pseudonymous. Organizational affiliation and self-described attributes can be displayed without revealing individual identity. This protects participants who may face social or economic consequences for their positions — a real concern in small agricultural communities where everyone knows everyone.

- **Multi-organization affiliation is supported from the start.** A farmer who belongs to both a commodity board and a provincial federation has a single account with multiple verified affiliations. A consumer who is also a part-time farmworker can describe both roles.

Key decisions to resolve early:

- Identity integrity mechanism: what is the minimum viable verification that ensures one-person-one-account without creating a burden that deters participation? Email verification alone is too weak (anyone can create multiple email addresses). Phone verification is stronger but excludes people without phones. A layered approach — email as baseline, phone or organizational vouching as optional strengthening — may be the right balance. This needs user research with the target population.
- Abuse and manipulation detection: beyond one-person-one-account, the platform needs pattern detection for coordinated inauthentic behaviour. If a cluster of accounts all created on the same day all vote identically, that is a signal worth flagging. This is a statistical detection problem, not a gatekeeping problem.
- Privacy architecture: what data does the platform hold, and what are the boundaries? Self-described attributes are voluntary. Organizational affiliation data is shared only with the participant's consent. The platform must be clear about what is visible to whom.
- Rights and affordances by participation tier: while the core principle is open participation, some specific actions may reasonably require higher identity assurance. For example, a constitutional amendment vote within an organization may require verified membership. Proposing a new topic might require a verified identity (not just email). The architecture should support configurable thresholds for specific actions without making exclusion the default.

Tech stack considerations:

- PostgreSQL for participant identity, organizational affiliation, and self-described attributes
- Server-side identity management with layered verification (email baseline, optional phone/organizational/ID verification)
- OAuth2/OIDC for session management
- Duplicate detection system (probabilistic matching across email, phone, name to flag potential multi-accounting)
- Channel-agnostic messaging abstraction layer from day one: a unified notification/interaction interface that supports SMS (Twilio or equivalent), WhatsApp Business API, Signal, email, and potentially other channels. The key design principle is that the platform never hardcodes a delivery channel — it routes through whichever channel the participant has configured. New channels can be added as plugins without modifying core logic.

### 0.2 Core Participation — Opinion Mapping

The Polis model is the right starting point for agricultural organizations because it requires minimal effort from participants and generates maximum insight for leadership.

How it works:

- An administrator (or agent, in later phases) creates a "topic" — a framing question like "How should our organization respond to the proposed labelling regulation?"
- Crucially, participants can also initiate topics. A participant who encounters an emerging issue — a sudden regulatory change, a disease outbreak, a market disruption — can propose a new topic for opinion mapping. Participant-initiated topics enter a lightweight validation stage (configurable per organization or platform-wide: automatic approval, moderator review, or endorsement threshold before activation). This is how Future Herd accommodates the spontaneous and emergent — it does not require leadership to anticipate every issue that matters to the community.
- Seed statements are provided to get the process started. Participants can also submit new statements for consideration within any active topic.
- Each participant sees statements one at a time and votes: agree, disagree, or pass.
- The platform runs dimensionality reduction (principal component analysis or similar) on the vote matrix to identify opinion clusters — groups of participants who tend to vote similarly.
- Results are displayed as a real-time opinion map: clusters are visible, areas of broad consensus are highlighted, and divisive statements are identified.

Implementation notes:

- The Polis algorithm (based on PCA applied to the vote matrix) is well-documented and has been replicated in several open-source projects. The CompVis method Polis uses is a reasonable starting point, but the implementation should be modular enough to swap in alternative clustering approaches.
- Statement moderation is critical. In the initial phase, this is manual (administrator review). In later phases, agents handle first-pass moderation with human override.
- The opinion map visualization needs to be understandable by people who have never seen a scatter plot used this way. Labels, annotations, and plain-language cluster descriptions are essential. "Group A tends to support market-based solutions; Group B tends to favour regulation" — not "Cluster 1, PC1 = 0.7."
- Vote data is stored per-participant (for audit and for the clustering algorithm) but individual votes are not publicly displayed. Participants see where they sit on the map; they do not see how specific other participants voted (unless the organization configures full transparency).

### 0.3 Core Participation — Pulse Surveys

Lightweight, fast-turnaround sentiment checks. Not the full Polis treatment — just a quick read on a specific question.

- Single question, multiple response options (Likert scale, ranked choice, or simple yes/no/abstain)
- Time-bounded (e.g., open for 48 hours)
- Push notification via the participant's preferred channel (app push, email, WhatsApp, SMS, etc.)
- Results displayed in real time as participation threshold is met
- Configurable quorum — results are not published until a minimum participation rate is reached
- Participants can initiate pulse surveys, not just administrators. A participant-initiated pulse survey requires a configurable endorsement threshold before going live (e.g., 10 participants co-sign the question). This keeps the tool responsive to ground-level concerns without flooding the community with noise.

This is the tool leadership will use most frequently. The opinion mapping is for deep questions; pulse surveys are for "we need a read on this by Friday."

### 0.3.1 Emergent Issue Surfacing

One of the core design principles of Future Herd is that the platform should not require someone at the top to identify every issue worth discussing. Agricultural communities face emergent, spontaneous, and sometimes urgent concerns that do not wait for the next board meeting or the next survey cycle. A disease outbreak. A sudden trade policy shift. A local infrastructure failure. A rumour that is spreading faster than any official response.

Future Herd must accommodate emergence as a first-class capability, not an afterthought. This means:

- Any participant can flag an emerging issue. Flagging is low-friction — a short description and a suggested framing question, submitted through the app or through any connected messaging channel.
- Flagged issues enter a triage process. This can be configured per context: automatic escalation if enough participants flag the same issue (or related issues), moderator review, or a combination. In later phases, the Pattern Detection Agent can identify when multiple independent flags are converging on the same underlying concern.
- Once an emergent issue is triaged and activated, it immediately spawns a lightweight participation space — either a pulse survey for a quick read or a full opinion-mapping topic depending on the assessed complexity.
- Emergent issues carry a visible "origin" tag: participant-initiated, leadership-initiated, agent-detected. This transparency matters. When participants see that the platform is surfacing concerns that came from the ground, not just from the boardroom, participation incentives change fundamentally.
- The speed of emergence matters. Between the moment a participant flags an issue and the moment others can begin participating, the elapsed time should be minutes to hours, not days to weeks. This is what "decision-making at the speed of the internet" means in practice.

The emergent issue layer is also where regular usage generates the most value over time. As participants develop the habit of flagging concerns through Future Herd rather than venting on social media or speculating in private groups, the platform becomes an early warning system for the entire community. Leadership does not have to wait until frustration boils over at an AGM. They see it forming in real time, with structure, and can respond before positions calcify.

### 0.4 Infrastructure

- Progressive Web App (PWA) — installable on mobile, works offline for cached content
- Responsive design tested on low-end Android devices (this is the primary device for many rural users)
- Service worker for offline queuing: if a participant votes while offline, the vote is queued and submitted when connectivity returns
- Channel-agnostic interaction for pulse surveys: participants can vote by replying through whichever messaging channel they use (WhatsApp reply, SMS reply, email link, or in-app). The messaging abstraction layer handles inbound as well as outbound — a vote received via WhatsApp is processed identically to one received via the web interface.
- Server deployment: containerized (Docker), deployable on modest infrastructure. The initial target is a single-server deployment that an organization's IT person (or contracted hosting provider) can manage.
- API-first design: every interaction goes through a documented REST API. The PWA is a client. Other clients (SMS gateway, future integrations) use the same API.

### 0.5 Administration Dashboard

- Organization setup and configuration
- Membership roll management (import, sync, manual add/remove)
- Topic and survey creation
- Results viewing with export (CSV, PDF reports)
- Audit log viewer
- Role-based access: platform admin, organization admin, topic moderator, participant (with configurable affiliation visibility)

### 0.6 Trust and Standing — Foundation

The open participation model means that anyone can join. The trust and standing layer is what makes sustained, quality participation visible and meaningful. It creates a form of earned authority that exists alongside — but independent of — institutional authority.

This is not gamification. It is not a leaderboard that rewards volume. It is a system of peer recognition that reflects what participants actually value: contributions that clarify, that bridge divides, that bring evidence, that make the platform a better place to think together.

**Core mechanics:**

- **Peer recognition.** Participants can recognize specific contributions by others — a well-framed proposal, a statement that shifted their thinking, a piece of evidence that grounded a discussion, a respectful challenge that sharpened a position. Recognition is attached to specific contributions, not to people in the abstract. This keeps the system grounded in what was actually said and done, not in popularity or personality.

- **Standing accrues from recognition, not from activity volume.** A participant who posts ten mediocre statements gets no standing from them. A participant who posts one statement that twenty people recognize as valuable gains standing. This is the critical design distinction from gamification: the platform rewards quality as judged by peers, not quantity as measured by the system.

- **Standing is visible but not ranked.** The platform does not produce a numbered leaderboard. Instead, standing is expressed as a visible attribute — similar to how organizational affiliation is visible. A participant's profile shows their history of recognized contributions, the topics they have been active in, and the peer recognition they have received. Other participants can see this context when evaluating someone's contributions. "This person has been consistently recognized for bridge-building contributions in supply management debates" is more useful than "#47 on the leaderboard."

- **Institutional and participatory standing coexist.** The platform acknowledges both forms of authority. An executive director of a commodity board has institutional standing that comes from their role — and the platform shows that. A consumer advocate with no institutional affiliation who has been consistently recognized for thoughtful contributions has participatory standing — and the platform shows that too. Neither form of standing trumps the other. Both are visible, and participants can weigh them as they see fit.

- **Standing enables, it does not gatekeep.** Higher standing might unlock specific affordances: the ability to fast-track an emergent issue flag, priority visibility for proposed topics, the ability to co-moderate a discussion thread. But it never becomes a prerequisite for basic participation. The path from new participant to recognized contributor is open to everyone, regardless of institutional affiliation.

- **Standing is contextual.** A participant may have high standing in deliberations about trade policy and no standing at all in discussions about animal welfare. Context-specific standing is more honest and more useful than a single global score. It reflects the reality that expertise and quality contribution vary by domain.

- **Recognition is itself visible and auditable.** Who recognized whom, for what contribution, and when — all of this is transparent. This prevents gaming (you cannot secretly trade recognition with allies) and builds trust in the system itself.

**Why this matters for the open participation model:**

Without a trust layer, the platform's openness is formally true but practically hollow. An unaffiliated consumer can technically participate, but they have no path to standing, no way to build a visible track record, no mechanism for their consistent quality contributions to be recognized. The institutional hierarchy remains the only hierarchy, and the platform's promise of openness rings false.

With a trust layer, participation becomes a genuine path to standing. A farmer who is not a member of any organization but who consistently contributes well-framed, evidence-based positions in commodity policy discussions builds visible authority on the platform. An Indigenous food sovereignty advocate who brings perspectives that no existing organization represents can earn standing that makes those perspectives harder to ignore. A young person entering agriculture who asks the questions no one else is asking can be recognized for that contribution.

This is how the platform creates space for new forms of leadership — not by appointing people, but by making the quality of their participation visible over time.

**Phase 0 implementation (foundation):**

In Phase 0, the trust layer is deliberately minimal. The infrastructure stores recognition data and displays contribution history, but the social norms around recognition need to develop organically through the meta-pilot before the system is elaborated. The initial implementation includes:

- Peer recognition of specific contributions (simple, one-click, with optional short note)
- Contribution history visible on participant profiles
- Standing displayed as context alongside contributions (not as a separate ranking)
- No affordance gating based on standing yet — that comes in later phases once the community has established what standing means in practice

### 0.7 Ecosystem Integration — Foundation

The platform does not launch into a vacuum. The existing Future Herd podcast, the intelligence digest (thefutureherd.ca/intelligence/), and the network of relationships with agricultural leaders are the initial ecosystem. From Phase 0, the platform is designed to connect with the information environment where its participants already live.

Social media is where much of this discussion currently takes place, and will continue to take place. Future Herd does not aim to replace social media — it aims to provide structure that social media cannot, while remaining connected to the broader conversation.

**Phase 0 ecosystem elements:**

- **Content pipeline from existing media.** Podcast episodes and intelligence digest items can be linked to deliberation topics. A podcast episode about supply management reform becomes the context for an opinion-mapping exercise. A digest item about a new regulatory proposal becomes the seed for an emergent issue flag. The content-to-participation pipeline is explicit and bi-directional: media draws people in, participation generates insight, and insight feeds back into the media.

- **Shareable outputs.** Every opinion map, every pulse survey result, every deliberation summary produces a shareable artifact — a URL, an image, an embeddable widget. Participants and leaders can share these on their existing social media channels, driving awareness and drawing new participants in. The platform's insight should flow outward, not stay locked behind a login.

- **Social media ingest.** The platform provides tools for surfacing and structuring discussions that are happening elsewhere. An administrator or agent can pull in a social media thread or news article as context for a deliberation. This is not about replacing social media but about giving scattered, fragmented conversation a place to be structured.

- **Open API from day one.** The API-first design is not just an engineering convenience — it is an ecosystem strategy. Third-party tools, news organizations, researchers, and community groups can build on the platform's data (respecting privacy and consent configurations). The API is how Future Herd becomes infrastructure rather than a walled garden.

- **RSS and webhook support.** New topics, deliberation outcomes, and pulse survey results can be published as feeds that other systems consume. Organizations can pipe Future Herd outputs into their existing newsletters, websites, or internal communications without manual re-entry.

---

## Phase 1 — Deliberation and Structured Decision Support

**Objective:** Add Decidim-style structured deliberation to complement the opinion-mapping capability. Introduce the governance bridge.

### 1.1 Proposals and Amendments

Drawing from Decidim's proposal lifecycle:

- Any participant can submit a proposal (text, with optional supporting documents). Organizations can configure whether proposals related to their internal governance require verified membership, but public-facing deliberations are open.
- Proposals move through defined stages: Draft, Open for Comment, Under Revision, Ready for Decision, Decided, Archived
- Participants can endorse proposals (public signal of support, distinct from a formal vote)
- Participants can submit amendments — proposed modifications to a proposal's text
- Amendments can be accepted, rejected, or put to a participant vote by the proposal author or moderator
- Version history is preserved for every proposal — every edit, every amendment, every stage transition is logged

This is where Future Herd starts to interface with formal governance. A proposal that achieves a defined threshold of endorsements and has been through the deliberation stages becomes a candidate for formal board consideration.

### 1.2 Threaded Discussion with Structure

Comment threads under proposals, but with deliberate constraints:

- Comments are tied to specific sections of a proposal (margin-style annotation, not a flat thread)
- Comments can be tagged by type: question, concern, suggestion, support, evidence
- Time-boxed discussion periods prevent indefinite drift
- Summary views (generated by agents in Phase 2) condense long threads into key positions

### 1.3 Governance Bridge v1

The interface between participation and formal decision-making:

- Structured reports generated for board/leadership: participation rates (both overall and among verified members), consensus areas, division points, proposal status, and crucially, any significant divergence between member positions and broader participant positions. This divergence information is not a threat — it is strategic intelligence that helps leadership understand how their membership's views relate to the wider community they operate within.
- Configurable triggers: "If a proposal receives endorsements from >30% of an organization's verified members, it is automatically forwarded to the board agenda." Triggers based on organizational membership thresholds are one of the few contexts where the membership/non-membership distinction has operational significance — because they interface with formal governance structures that are constitutionally defined by membership.
- Decision recording: when a board makes a formal decision on a matter that was deliberated on the platform, the decision is recorded and linked to the deliberation history
- Transparency log: participants can see the path from participatory input to formal decision (or see that their input was received but the board decided otherwise, with recorded rationale)

### 1.4 Notification and Engagement System

- Configurable notification preferences per participant (email, SMS, push, digest)
- Smart notification batching to avoid notification fatigue (daily digest by default, immediate for time-sensitive votes)
- Engagement nudges: if a participant hasn't participated in a topic where their cluster is underrepresented, a gentle prompt (not a guilt trip)
- Seasonal awareness: notification timing should respect agricultural calendars. Don't push survey notifications during harvest.

### 1.5 Trust and Standing — Deliberation Layer

Building on the Phase 0 foundation, the trust layer now integrates with structured deliberation:

- Peer recognition expands to include deliberation-specific contributions: well-crafted proposals, constructive amendments, comments that shift the discussion, and evidence-based arguments.
- Standing becomes contextual by topic domain. A participant's standing in trade policy deliberations is distinct from their standing in animal welfare discussions. This reflects the reality that expertise and quality contribution vary by domain.
- Standing begins to enable specific affordances: participants with established standing can co-moderate discussion threads, fast-track emergent issue flags, and receive priority visibility for proposed topics. These affordances are earned through peer recognition, not appointed by administrators.
- Bridge-building recognition: a specific recognition type for contributions that help opposing clusters find common ground. This incentivizes the behaviour the platform most needs — not agreement, but productive engagement across divides.

### 1.6 Ecosystem Integration — Deliberation Layer

- **Deliberation outputs feed outward.** Proposal summaries, opinion maps, and decision outcomes are published as structured content that organizations can embed in their newsletters, websites, and social media. A commodity board can share "Here is where our community stands on the labelling proposal" directly from the platform to their existing communications channels.
- **External content feeds in.** News articles, policy documents, research papers, and social media discussions can be linked as evidence within deliberations. The platform becomes a place where scattered information is organized around specific decisions.
- **Podcast integration deepens.** Future Herd podcast episodes can be directly linked to active deliberations. A guest's argument on the podcast becomes a reference point in the deliberation. Deliberation outcomes can inform future podcast topics — closing the loop between media and participation.
- **Intelligence digest integration.** The thefutureherd.ca/intelligence/ digest items can trigger or inform deliberations automatically. A digest item about a regulatory change can spawn a pre-seeded opinion-mapping topic, reducing the time from "issue identified" to "community response structured."

---

## Phase 2 — Agent Layer

**Objective:** Introduce AI agents as transparent facilitators. Every agent action is logged, auditable, and overridable.

### 2.1 Agent Architecture

Agents are not a monolithic AI system. They are a set of specialized, constrained agents with defined roles and authorities. The architecture follows a principal hierarchy:

- **The participants are the ultimate principals.** Agents serve the community of participants, not just organizational leadership.
- **Organization administrators configure agent authorities.** They decide which agents are active and what they are permitted to do.
- **Agents cannot take any action that is not explicitly within their defined authority.** No emergent behavior, no scope creep.
- **Every agent action is logged to an immutable audit trail.** Members can inspect what any agent did, when, and why.

Agent runtime considerations:

- Agents run server-side on the Future Herd infrastructure
- LLM calls go through a controlled gateway with rate limiting, cost tracking, and content filtering
- Organizations can choose their LLM provider (Anthropic, self-hosted open models, etc.) — the agent layer is provider-agnostic
- Agent prompts and system instructions are open source and auditable. No black boxes.
- Agent outputs are always marked as agent-generated. There is no ambiguity about whether a human or an agent produced a given summary or translation.

### 2.2 Synthesis Agent

Role: Condense long discussion threads and complex proposal histories into structured summaries.

Authorities:
- Read all public discussion content within a topic
- Generate summaries tagged as agent-produced
- Cannot edit, delete, or modify any human-generated content
- Cannot submit proposals or cast votes

Outputs:
- Thread summaries: "Here are the main positions expressed in this discussion, organized by theme"
- Proposal evolution summaries: "This proposal has been amended three times. Here are the key changes and the reasons given"
- Consensus/division reports: "Broad agreement exists on X. The main disagreement is between those who favour Y and those who favour Z"

### 2.3 Translation Agent

Role: Make content accessible across languages (particularly relevant for Canadian agricultural organizations operating across English and French, or communities with immigrant farmer participation).

Authorities:
- Read all public content
- Generate translations tagged as agent-produced
- Cannot modify original content

Implementation:
- Real-time translation of proposals, comments, and summaries
- Bilingual display option (original + translation side by side)
- Terminology glossary for agricultural and organizational terms (to ensure consistent translation of domain-specific language)

### 2.4 Moderation Agent

Role: First-pass moderation of submitted statements and comments.

Authorities:
- Flag content for human review (cannot remove content unilaterally)
- Apply content tags (off-topic, duplicate, needs-clarification)
- Generate moderation recommendations with reasoning

Constraints:
- Cannot suppress any participant's content without human moderator confirmation
- All flagging decisions include written reasoning visible to the content author
- Appeals go directly to human moderators
- Moderation criteria are published and configurable by the organization

### 2.5 Plain Language Agent

Role: Translate policy documents, regulatory language, and technical agricultural content into accessible language.

This is particularly important for agricultural deliberations where participants need to understand complex regulatory proposals, trade agreements, or scientific findings — and where the people most affected by these policies may not have the technical background to parse them in their original form.

Authorities:
- Read documents uploaded by administrators
- Generate plain-language summaries tagged as agent-produced
- Generate glossaries of technical terms
- Cannot alter original documents

### 2.6 Pattern Detection Agent

Role: Surface emerging trends, shifting sentiment, and potential fault lines.

Authorities:
- Analyze voting patterns and discussion trends across topics and time
- Generate pattern reports for administrators
- Flag rapid shifts in opinion clusters or unusual participation patterns

Constraints:
- Reports are descriptive, never prescriptive ("Participation among dairy farmers has dropped 40% this month" — not "You should reach out to dairy farmers")
- Cannot identify individual participants in pattern reports (only aggregates and clusters)
- Pattern reports are available to all participants, not just leadership (transparency by default)

### 2.7 Trust and Standing — Agent Integration

Agents interact with the trust layer in specific, transparent ways:

- The Synthesis Agent incorporates standing context when generating summaries. Contributions from participants with high peer recognition in the relevant domain receive more prominent placement in summaries — not because the agent defers to authority, but because peer recognition is a signal of contribution quality. This weighting is visible and auditable.
- The Pattern Detection Agent monitors the trust system itself for gaming patterns: reciprocal recognition clusters, sudden spikes in recognition for specific participants, or coordinated recognition campaigns. Anomalies are flagged for human review.
- The Moderation Agent factors in participant standing when triaging flags. A flagged contribution from a participant with established standing and no moderation history is treated differently than one from a new account — not by suppressing the flag, but by routing it appropriately.
- No agent can grant or revoke standing. Standing is exclusively peer-driven. Agents can surface standing-related information but cannot manipulate it.

### 2.8 Ecosystem Integration — Agent Layer

- **Social media monitoring agent.** A specialized agent that monitors configured social media channels, news feeds, and other external sources for discussions relevant to active deliberations. When significant external conversation is detected, the agent can surface it as context within the platform — a link, a summary, or a prompt to consider external perspectives. This keeps the platform connected to the broader information environment without requiring participants to manually import content.
- **Outbound synthesis for external channels.** Agents generate shareable summaries optimized for different channels: a concise summary for social media, a structured briefing for newsletters, an embeddable visualization for websites. These outputs make the platform's insight flow naturally into the information ecosystem.
- **Podcast and digest integration automation.** Agents can generate structured briefings from active deliberations that feed directly into the Future Herd intelligence digest or inform podcast episode preparation. The loop from external content into the platform and from platform insight back out to media becomes increasingly automated.

---

## Phase 3 — Federation and Inter-Organization Collaboration

**Objective:** Enable multiple organizations to connect, share relevant deliberations, and collaborate on issues that cross organizational boundaries.

### 3.1 Federation Protocol

Agricultural issues rarely respect organizational boundaries. A labelling regulation affects commodity boards, provincial federations, processors, and retailers. Future Herd needs to support cross-organizational deliberation without collapsing organizational identity.

Design approach:

- Each Future Herd instance is sovereign. An organization owns its data and controls its configuration.
- Federation is opt-in and configurable. An organization can choose to federate specific topics or proposals with specific partner organizations.
- Federated topics maintain separate voting and discussion spaces per organization, with a shared view that shows cross-organizational opinion maps.
- Member identities are verified within their home organization. Federated views show organizational affiliation but not individual identity (unless both organizations configure otherwise).
- Federation protocol should be built on ActivityPub or a similar open standard to allow interoperability with other platforms in the future.

### 3.2 Cross-Organization Opinion Mapping

When multiple organizations federate around a topic, the opinion map expands:

- Intra-organization clusters are visible as before
- Inter-organization patterns become visible: "Cattle producers in Alberta and Ontario cluster together on this issue despite being in different organizations"
- Leadership at each organization sees both their own community's positions and the broader landscape

### 3.3 Shared Proposal Spaces

For issues that require coordinated action across organizations:

- Joint proposals can be submitted to multiple federated organizations simultaneously
- Each organization's participants deliberate independently
- Cross-organizational endorsement counts are visible
- Formal decisions remain within each organization's governance structure

### 3.4 Trust and Standing — Federation Layer

Standing travels across federation boundaries, but with appropriate translation:

- A participant's standing within their home organization or context is visible in federated deliberations, but it is clearly labeled by origin. High standing in an Ontario dairy farmers' deliberation is meaningful context in a cross-Canada dairy policy discussion, but it does not automatically confer standing in a beef producers' deliberation.
- Cross-organizational recognition becomes possible. When participants from different organizations recognize each other's contributions in federated spaces, this creates a form of cross-organizational standing that reflects the platform's ability to surface quality thinking regardless of institutional origin.
- The federation layer makes the alternative hierarchy most visible. In a cross-sectoral deliberation, institutional position becomes just one attribute among many. A consumer advocate with high participatory standing sits alongside a commodity board president, and both are visible for what they bring.

### 3.5 Ecosystem Integration — Federation Layer

- **Federated deliberations produce shared public outputs.** When multiple organizations deliberate on a cross-cutting issue, the combined opinion map and deliberation outcomes are publishable as a shared artifact — demonstrating cross-sectoral perspective in a way no single organization could produce.
- **External stakeholder observation.** Federated deliberations can be configured to allow observation (but not participation) by external stakeholders — policymakers, researchers, journalists. This creates a transparent window into how the sector is thinking about an issue, without compromising the participation space.
- **Integration with policy processes.** Federated deliberation outcomes can be structured as formal submissions to government consultations, regulatory processes, or trade negotiations. The platform produces the evidence of broad, structured input that policy processes claim to want but rarely receive.

---

## Phase 4 — Advanced Agent Capabilities

**Objective:** Extend the agent layer to support more sophisticated facilitation, while maintaining transparency and human authority.

### 4.1 Scenario Modeling Agent

Role: Help participants understand the potential consequences of different positions.

- Given a proposal (e.g., "Support a 10% tariff on imported dairy products"), the agent generates scenario analyses: potential impacts on different farm types, price projections, trade implications
- Sources are cited. Assumptions are stated explicitly. Uncertainty is quantified where possible.
- Multiple scenarios are always presented (best case, worst case, most likely) — the agent never presents a single projected outcome

### 4.2 Bridge-Building Agent

Role: Identify potential areas of compromise between divided opinion clusters.

- Analyzes the vote matrix to find statements that partially satisfy multiple clusters
- Generates "bridge proposals" — suggested framings that might reduce polarization
- Bridge proposals are clearly marked as agent-generated and require human sponsorship before entering the deliberation process

### 4.3 Institutional Memory Agent

Role: Maintain and surface organizational history relevant to current deliberations.

- When a new topic is opened, the agent identifies past deliberations on related subjects
- Surfaces historical positions: "This community discussed a similar proposal in 2023. Here is what participants decided then, and here are the key arguments"
- Tracks position evolution over time: how has the organization's collective stance on a given issue shifted?

### 4.4 Agent Teams

Multi-agent coordination for complex facilitation tasks:

- Synthesis + Translation working together on multilingual summaries
- Pattern Detection + Institutional Memory identifying recurring cycles
- Scenario Modeling + Plain Language making complex projections accessible
- Coordination protocol ensures agents don't duplicate effort or produce contradictory outputs
- Human-in-the-loop checkpoints at each stage of multi-agent workflows

### 4.5 Trust and Standing — Mature System

By Phase 4, the trust layer has been shaped by community practice through the meta-pilot and organizational deployments. The mature system includes:

- **Standing-informed scenario modeling.** The Scenario Modeling Agent can draw on the standing system to identify participants with domain expertise and surface their contributions as particularly relevant context for scenario analysis — without overriding the views of other participants.
- **Recognition of bridge-building becomes a core platform value.** The Bridge-Building Agent and the trust layer's bridge-building recognition type work together: participants who are recognized by peers for cross-cluster contributions become visible as the platform's most valued contributors. This is the alternative hierarchy at its most powerful — the people the community recognizes as making the platform work well.
- **Standing portability across contexts.** As the platform matures, participants may wish to reference their Future Herd standing in external contexts — applications, policy submissions, professional profiles. The platform can provide verifiable standing attestations that demonstrate a participant's history of recognized contributions without revealing their specific positions or votes.

### 4.6 Ecosystem Integration — Mature System

- **Data integration for evidence-based deliberation.** Weather and market data feeds provide real-time context for deliberations (e.g., a deliberation about drought response shows current conditions). Agricultural census and statistics are accessible within the platform. Regulatory tracking flags when relevant regulations change, alerting the community and prompting new deliberations where past positions may need revisiting.
- **Public transparency layer.** Organizations and the platform as a whole can make selected deliberation outcomes public — anonymized opinion maps, decision histories, and cross-sectoral consensus statements. This is the food literacy dimension of the project: making agricultural governance visible to the broader public in structured, interpretable form. Structured data export serves researchers, journalists, and policymakers.
- **Developer and extension ecosystem.** Plugin architecture for custom agents, integrations, and visualizations. Full API documentation and developer portal. Community governance for the open-source project itself — Future Herd should use Future Herd to govern Future Herd.
- **Social media as a two-way bridge.** The platform's social media integration, which began as basic shareable outputs in Phase 0 and grew through agent-powered monitoring in Phase 2, is now a mature two-way bridge. Structured insight flows out to where people are. Emergent discussions flow in and are given structure. The platform does not compete with social media — it provides the deliberation and decision-making infrastructure that social media cannot.

---

## Technical Stack (Recommended)

This is a starting recommendation, not a prescription. The stack should be evaluated against the specific deployment constraints of pilot organizations.

**Backend:** Rust or Go for the core API server (performance, safety, single-binary deployment). Python for agent orchestration and data analysis (ecosystem support for ML/NLP libraries).

**Database:** PostgreSQL as the primary data store. TimescaleDB extension for time-series participation data. Redis for caching and real-time features.

**Frontend:** Progressive Web App built with a lightweight framework (Svelte or Preact preferred over React for bundle size — rural bandwidth matters). Server-side rendering for initial page loads.

**Agent Layer:** Provider-agnostic LLM gateway. Support for Anthropic API, OpenAI API, and local models (llama.cpp, Ollama). Agent orchestration framework (custom, not dependent on a specific vendor's agent SDK).

**Real-time:** WebSocket connections for live opinion map updates. Server-Sent Events as a fallback for constrained clients.

**Messaging Layer:** Channel-agnostic abstraction with plugin adapters. Initial adapters for: email (SMTP/SendGrid), SMS (Twilio), WhatsApp Business API, and web push notifications. The abstraction layer handles both outbound (notifications, magic links, vote prompts) and inbound (vote replies, issue flags). Additional channel adapters (Signal, Telegram, etc.) can be added without modifying core platform logic. Each adapter handles the specific constraints of its channel (character limits for SMS, rich formatting for email, interactive buttons for WhatsApp).

**Deployment:** Docker Compose for single-server deployment. Kubernetes manifests for scaled deployment. Terraform modules for cloud provisioning. Documentation for bare-metal deployment on modest hardware (a local organization should be able to run this on a decent server in a closet if they want to).

**Federation:** ActivityPub-based protocol for inter-instance communication.

---

## Governance of the Project Itself

Future Herd is open source. The project's own governance should embody the principles the software promotes.

- **License:** AGPL-3.0 (ensures that modifications to the platform remain open, even when deployed as a service)
- **Contribution model:** Open contributions with a core maintainer team. RFC process for significant architectural changes.
- **Decision-making:** Use Future Herd itself (once functional) for project governance decisions. Until then, a simple RFC + lazy consensus model among core contributors.
- **Funding model:** Sustainable open source. Potential revenue streams include hosted deployment services, custom agent development, training and support, and grants from agricultural and democratic governance funders. The software itself remains free and open.

---

## Pilot Strategy: The Meta-Pilot

The AAC's structural position transforms the pilot problem. Instead of the traditional open-source challenge of "find a willing organization, hope they stick with it," Future Herd can run a meta-pilot that serves as demonstration, stress test, and genuine decision-making exercise simultaneously.

### The Meta-Pilot Design

The initial deployment targets agricultural leaders who already engage with the Future Herd podcast and knowledge base (thefutureherd.ca). These are executive directors, board chairs, policy leads, and senior staff from organizations across the agri-food sector. They are not end-user farmers (yet) — they are the people who will decide whether to deploy Future Herd within their own organizations.

The meta-pilot asks these leaders to use the platform to deliberate on cross-sectoral questions that genuinely matter: the future of agricultural data governance, approaches to climate adaptation, workforce challenges, trade policy priorities, food security strategy. These are not synthetic test cases. They are live questions where structured input from diverse organizational leaders has real value.

This design addresses multiple risks at once:

**Buy-in through experience, not pitch decks.** A leader who has personally used Future Herd to see where their peers stand on a contentious issue understands the tool's value in a way no demo can replicate. When they consider deploying it for their own membership, they are evaluating a tool they have already used, not one they have been told about.

**Sophisticated user feedback.** Agricultural organization leaders are demanding users. They will identify UX problems, missing features, and edge cases that a typical beta test would miss. They will also identify political and governance sensitivities that pure technologists would never anticipate.

**Real content from day one.** The existing podcast and knowledge base provide a natural pipeline. A Future Herd episode on supply management reform becomes the context for an opinion-mapping exercise. A research brief on agri-food labour markets becomes the foundation for a structured proposal. Content and participation reinforce each other.

**Visible proof of concept.** The meta-pilot itself produces a visible artifact: a structured, documented picture of where agricultural leaders stand on key issues, how their positions cluster, and where consensus and division exist. This artifact has value to policymakers, funders, and the broader agricultural community. It demonstrates that the tool works by producing something useful, not just by existing.

**Risk identification in a low-stakes environment.** If the opinion-mapping algorithm produces confusing results, if the emergent issue surfacing generates too much noise, if the notification system annoys people — better to discover this with a group of 50-200 leaders who understand they are testing infrastructure than with 2,000 members who just want to be heard.

### From Meta-Pilot to Organizational Deployment

The meta-pilot is not an end in itself. The explicit goal is to transition from sector-level experimentation to organization-level deployment. The path:

1. Leaders use Future Herd for cross-sectoral deliberation through the AAC context.
2. Individual leaders identify specific use cases for their own organizations ("We could have used this for our labelling consultation last year").
3. The platform's multi-organization architecture allows a leader's organization to spin up its own instance (or namespace within a shared instance) and begin onboarding its own membership.
4. The meta-pilot continues in parallel with organization-level deployments, maintaining the cross-sectoral deliberation space while individual organizations run their own internal participation processes.

This creates a natural growth path that does not depend on cold outreach or speculative adoption.

### Success Metrics

The meta-pilot should run for a minimum of six months, with ongoing evaluation across these dimensions:

**Participation quality.** Are leaders engaging substantively (voting, submitting statements, flagging issues) or just observing? What is the ratio of active to passive participants?

**Insight utility.** Do the opinion maps and deliberation outcomes produce information that participants and the AAC report as genuinely useful? Does the output inform actual decisions or conversations?

**Adoption intent.** How many participating leaders express interest in deploying Future Herd within their own organizations? What barriers do they identify?

**Platform reliability.** Uptime, performance under load, channel delivery rates, offline sync reliability.

**Emergent issue responsiveness.** How quickly do participant-flagged issues move from submission to active participation? Do leaders report that the platform surfaced concerns they were not already aware of?

**Agent trust (once Phase 2 begins).** Do participants find agent-generated summaries accurate and useful? Do they report understanding how agents operate?

---

## Risks and Open Questions

**Adoption risk.** The target audience spans a wide range of technical comfort. Onboarding must be radically simple. If a participant cannot begin participating within two minutes of arriving at the platform, the friction is too high.

**Manipulation risk.** Open participation increases the attack surface for coordinated manipulation. Organized groups could create accounts to distort opinion maps. The identity integrity layer (one person, one account) is the first line of defence. The clustering algorithm provides a second: coordinated voting tends to show up as a distinct cluster rather than shifting the overall map, making manipulation visible rather than invisible. The Pattern Detection Agent provides a third. But the platform must be designed to make manipulation attempts legible and auditable, not to prevent them through exclusion.

**Agent trust.** Members may not trust AI-generated summaries or moderation. The transparency-first design (every agent action logged, auditable, overridable) is the primary mitigation, but building trust will take time and demonstrated reliability.

**Connectivity.** Rural broadband in Canada is improving but remains uneven. The channel-agnostic messaging layer is essential — some participants will have reliable mobile data for WhatsApp, others will depend on SMS, others will have wifi at home but nothing in the field. The PWA must be genuinely functional on 3G-equivalent connections, and the offline queuing must be reliable.

**Organizational politics.** Some leaders will not want to see what their members actually think. This is a feature, not a bug. The meta-pilot partially mitigates this risk: leaders who participate in cross-sectoral deliberation experience the value of transparency before they face the question of deploying it for their own membership. But the transition from meta-pilot participant to internal champion will still require careful navigation of organizational dynamics.

**Data sovereignty.** Agricultural organizations handle sensitive data (membership information, positions on politically charged issues). Data hosting and jurisdiction must be carefully managed. Canadian organizations will likely require Canadian data residency.

**Scale economics.** LLM API costs for the agent layer need to be sustainable. The provider-agnostic architecture allows organizations to use local models for cost-sensitive deployments, but the quality trade-offs need to be honestly assessed.

---

## Immediate Next Steps

1. **Architecture decision records (ADRs)** for the key early decisions: authentication and identity integrity, data model for participation and organizational affiliation, opinion-clustering algorithm, trust and standing mechanics, PWA framework selection, messaging abstraction layer design, ecosystem integration approach.

2. **Wireframes** for the core participant experiences: opinion mapping, pulse survey, results dashboard, emergent issue flagging, peer recognition, and participant profile (showing standing and contribution history). Additionally, wireframes for the leadership deliberation view specific to the meta-pilot.

3. **Meta-pilot scoping with the AAC.** Define the initial set of cross-sectoral questions for the meta-pilot. Identify the first cohort of leaders to invite. Establish the relationship between the existing thefutureherd.ca content pipeline (podcast and intelligence digest) and the participation platform. Define how podcast episodes and digest items will seed deliberation topics from day one.

4. **Core data model and API specification.** Define the REST API before writing implementation code. The data model must support open participation with organizational affiliation, the trust and standing layer, and the meta-pilot's cross-sectoral structure from the start. Design the API with ecosystem integration in mind — every output should be sharable, embeddable, and subscribable.

5. **Identity integrity prototype.** Build the participant enrollment flow with layered verification (email baseline, optional phone/organizational vouching). For the meta-pilot, verification can leverage the AAC's existing relationships (invited leaders are pre-verified through the AAC network), but the architecture should support open enrollment from the start.

6. **Opinion-mapping proof of concept.** Implement the Polis-style vote matrix and clustering algorithm with synthetic data. Validate that the visualization is interpretable by non-technical users. Then test it live with a small group from the meta-pilot cohort on a real question.

7. **Messaging abstraction layer prototype.** Build the channel-agnostic notification and interaction layer with at least two adapters (email and one instant messaging channel). Test delivery reliability and inbound vote processing across channels.

8. **Trust and standing design document.** Before implementation, develop a detailed design for the peer recognition mechanics, standing accrual, and contextual display. This should be informed by research into existing peer recognition systems (Stack Exchange, Wikipedia, Polis cluster dynamics) and by early conversations with meta-pilot participants about what kinds of contribution they would want to recognize.

9. **Ecosystem integration prototype.** Build the shareable output pipeline: opinion maps and pulse survey results that generate shareable URLs, images, and embeddable widgets. Connect the intelligence digest to the platform so that digest items can seed deliberation topics. This is how the platform begins to exist in the broader information environment from its first deployment.