# Start Demo - Story Flow

## Audience and Tone
- Mixed audience
- Slightly more business and technical decision makers than developers
- Technical presentation style
- Spoken delivery should stay concrete and clear, with minimal internal shorthand unless needed

## Core Story
A competitor announces a superior allergy treatment launching in November, putting our market position at risk.

In response, the business forms a small cross-functional team to assess the threat, model the constraints, and accelerate our next-gen product launch.

The team starts by gathering data and building the case. Then they validate supply chain limits across plants, materials, and equipment. Finally, they prepare a recommendation for leadership.

At the center of this effort is an autonomous Production Planning agent. An IT business analyst builds it in Copilot Studio using the Operations BRD. The agent connects to Work IQ and D365 ERP, aggregates data across three plants, flags capacity and material constraints, proposes optimized run orders, and runs what-if analysis that the team can review and approve.

This gives us a concrete path for the demo: start from active work in GitHub Copilot App, bring an existing app or skill in from Copilot Studio, improve and deploy the agent with Foundry and IQs, show how agents appear in Teams and M365, and then bridge into governance with Agent 365, Defender, and MDASH.

## Proposed Sketch Set

### Sketch 1 - App Triage in GitHub Copilot App
Purpose: Establish the business problem and show how the cross-functional team organizes the response in GitHub Copilot App.

Why this title:
- More concrete than a generic product tour
- Ties the app UI to a real business event
- Sets up a specific work item that becomes the agent story

Story beats:
- Open with the competitive threat and the need to respond quickly.
- Introduce the project manager and operations lead as the core team.
- Use GitHub Copilot App to show home, my work, automations, and quick chats as the control surface for the response.
- Narrow into the live project where the team is tracking the accelerated launch plan.
- Move into sessions, worktrees, rubber duck, and canvas to show how the team turns discussion into a scoped implementation path.
- End on a concrete next step: bring an existing Production Planning agent or Copilot Studio skill into the development flow.

Suggested timing: 1:45 to 2:00

Transition out:
- We have the business case and a clear work item. Now we take that agent from local code to a hosted, managed service.

### Sketch 2 - Promote a Local Agent to the Cloud
Purpose: Show the path from a local supply chain agent to a hosted agent with Microsoft controls, IQ connections, and observability.

Why this title:
- Clear technical progression
- Easy to narrate for a mixed audience
- Leaves room for VS Code, Foundry, hosted execution, and Teams/M365 endpoints

Story beats:
- Start in VS Code with the local Production Planning agent running on Windows.
- Show the agent doing useful work against the supply chain scenario.
- Attempt a risky action and show it being constrained by MxC or OS-level containment.
- Introduce toolbox and the IQs that ground the agent in internal and external context.
- Bring in Foundry to connect the right model, knowledge, and deployment path.
- Deploy as a hosted agent that runs in its own managed environment.
- Show traces, rubric generation, and optimization as the basis for improvement.
- Land with agents showing up in Teams and M365 as part of daily work.

Suggested timing: 2:45 to 3:15

Transition out:
- Once the agent is running in production, the next question is how to improve quality and behavior over time.

### Sketch 3 - Improve the Agent
Purpose: Explain the three practical paths for improving agent quality after deployment.

Why this title:
- Easier to understand than Hill Climbing
- Preserves the technical idea without requiring extra explanation
- Works for business leaders and developers alike

Story beats:
- Frame this as the next step after traces and optimization.
- Explain three ways to improve the agent:
  1. Custom code plus custom data
  2. Your data with Foundry support
  3. M365 feedback and reinforcement loops
- Tie each path back to the supply chain scenario so it feels like a continuation, not a side topic.
- Keep this sketch tight and conceptual.

Suggested timing: 1:00 to 1:15

Transition out:
- As more agents go live across the business, quality is only part of the story. We also need visibility, policy, and response.

### Sketch 4 - Govern the Agent Fleet
Purpose: Bridge into Protect and Observe by showing that live agents are visible, governed, and secure.

Why this title:
- Stronger and more active than Security and Governance
- Matches the fleet language in the broader story
- Sets up the handoff naturally

Story beats:
- Open in Agent 365 with overview, registry, map, and requests.
- Show that the supply chain agent now lives alongside the rest of the fleet.
- Call out healthcare policy, posture, and governance status.
- Bring in Defender and MDASH as the security handoff.
- Mention code scanning, sandbox validation, and findings flowing back as a Copilot PR before release.
- Show the bridge to deeper investigation and response in the next section.

Suggested timing: 0:45 to 1:00

Transition out:
- We have shown how to build, promote, improve, and govern agents. From here, we go deeper on protection and observability.

## Cross-Cutting Threads to Keep Consistent
- One continuous supply chain story across all four sketches
- The same Production Planning agent should appear in each sketch in a different stage of maturity
- Keep Work IQ, Foundry IQ, Web IQ, and Fabric IQ additive, not a checklist
- Keep Agent 365 and observability visible early enough that governance does not feel bolted on at the end
- Use MxC and Windows 11 or Scout as proof of containment and enterprise manageability

## Open Questions
- Final product naming to use on stage: GitHub Copilot App, Agent 365, Foundry, MDASH, MxC, IQ names
- Which Copilot Studio artifact we are actually bringing into GitHub Copilot App
- Whether Sketch 2 should explicitly mention Frontier Tuning or save that for Sketch 3
- Whether healthcare posture should be foregrounded in Sketch 4 or kept as a brief policy proof point

## Recommended Next Step
Create four sketch skeletons as separate .sk files with revised titles, rough rows, and clear transitions.