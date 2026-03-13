# Data Model

The data model is not yet defined. It will be documented here before implementation begins.

Key entities include:

- Participant (identity, verification level, self-described attributes)
- Organization (membership rolls, configuration, governance settings)
- Affiliation (participant-organization relationship, verification status)
- Topic (framing question, status, origin — participant/leadership/agent)
- Statement (text, author, moderation status)
- Vote (participant, statement, position — agree/disagree/pass)
- Proposal (text, stage, version history, endorsements)
- Amendment (proposed modification, status, linked proposal)
- Recognition (peer recognition of a specific contribution)
- Standing (accrued standing by participant, contextual by domain)
- AgentAction (agent, action type, inputs, outputs, timestamp — audit trail)
