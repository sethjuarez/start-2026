# Three-Person Demo Split - Build, Manage, Optimize

This is a proposed three-presenter split for the current demo flow without changing the underlying story. The goal is to divide the narration into three clear roles that feel natural on stage, give each presenter a distinct chapter, and help the audience follow the progression from initial build to enterprise operation to continuous improvement.

## Recommended split

- Presenter 1: BUILD
- Presenter 2: MANAGE
- Presenter 3: OPTIMIZE

This works because the story already moves through three natural stages.

1. Build the first working agent around a real invoice assurance problem.
2. Manage that agent inside the enterprise with governance and day-to-day usage.
3. Optimize quality and cost once the agent is running at production scale.

## Presenter 1 - BUILD

Presenter 1 owns the creation arc. This speaker introduces the business problem, shows the product outcome in Waypoint, and walks through how the first version of the agent is built and connected to enterprise evidence.

### Recommended coverage

- Setup
- Sketch 0 - Waypoint Invoice Reconciliation
- Sketch 1 - GitHub Copilot App - Our First Agent POC
- Sketch 2 - Microsoft Foundry, M365, and A365 - up through hosted deployment in Foundry

### What this speaker is responsible for

- Establish the business pressure created by increased CMO activity
- Show that invoice assurance is about validating billed work against contracts, receipts, approvals, QA release, and related operating evidence
- Start with visible outcomes in Waypoint so the audience sees matched, variance, and disputed invoices with real dollar impact
- Explain the local proof of concept clearly as a first working approximation, not the final operating model
- Show how the agent moves from local or simulated data into enterprise data with the right tools and guardrails
- End at the point where the agent is deployed as a hosted agent in Foundry

### Core message

We started with a real invoice assurance problem in Waypoint, proved the task locally, and then connected that work to enterprise data and hosted execution.

## Presenter 2 - MANAGE

Presenter 2 owns the operating and governance arc. This speaker picks up once the agent is enterprise-ready and explains how it is used in daily work and governed inside Pharma Company.

### Recommended coverage

- Sketch 2 - Microsoft Foundry, M365, and A365 - from M365 or A365 autopilot onward

### What this speaker is responsible for

- Show how the hosted agent becomes available in M365 or A365 and can be used in Teams
- Explain how people engage with the agent in the flow of invoice assurance work
- Show approvals, listing, access, and auditability in A365
- Explain how governance supports production use inside Pharma Company
- Make clear that the agent is no longer an isolated prototype. It is now a managed enterprise asset

### Core message

Once the agent is working, the next question is how to put it in front of the right people, govern its use, and make it trustworthy in day-to-day operations.

## Presenter 3 - OPTIMIZE

Presenter 3 owns the improvement and cost arc. This speaker explains how the running system gets better over time and becomes more efficient to operate at scale.

### Recommended coverage

- Sketch 3 - Hill Climbing
- Suggested Close

### What this speaker is responsible for

- Show Foundry rubric evaluators and how rubrics can be generated from traces
- Show the generated rubrics and how evaluations are run against them
- Explain how Agent Optimizer improves contract reasoning, evidence use, and recommendation quality
- Show cost in A365 and explain why cost matters once many invoice reviews run every day
- Walk through hill climbing and explain how learned behavior is carried into a smaller model
- Explain how RLE helps the smaller model approach the larger model's quality at a lower operating cost
- Close by tying quality and cost improvements back to better payment decisions, reduced leakage, and stronger confidence in invoice assurance

### Core message

After the agent is in production, the next goal is to improve its quality, measure its performance, and reduce the cost to run it at scale.

## Why this split works

### 1. Each presenter gets a full chapter

This split gives each speaker a clear narrative lane instead of making one presenter feel like a short add-on.

- BUILD = make it real
- MANAGE = make it usable and governed
- OPTIMIZE = make it better and less expensive to run

### 2. It follows the maturity curve of the solution

The audience can follow a simple progression.

- Can we build it?
- Can we run it in the business?
- Can we improve it and scale it efficiently?

### 3. It gives Sketch 3 a clear purpose

In a two-person split, the hill-climbing section can feel like an extra chapter at the end. In a three-person split, it becomes the final act of the story and gets the attention it deserves.

## Best handoff points

### Handoff 1 - BUILD to MANAGE

The cleanest handoff is inside Sketch 2, after the hosted agent is deployed in Foundry.

At that point, Presenter 1 has completed the story of building the agent and connecting it to enterprise evidence. Presenter 2 can then pick up with how the agent is used in day-to-day work and how the business governs that usage.

#### Example handoff

Presenter 1 can end with a line like:

"At this point, the invoice review agent is no longer just a local proof of concept. It is connected to enterprise evidence and running as a hosted agent in Foundry."

Presenter 2 can begin with a line like:

"From here, the next question is how that agent shows up in daily work, and how Pharma Company governs it once more teams start relying on it."

### Handoff 2 - MANAGE to OPTIMIZE

The cleanest second handoff comes after M365 or A365 usage and governance are established.

At that point, Presenter 2 has shown that the agent is available to the business and managed appropriately. Presenter 3 can then move into how the team improves quality and controls operating cost over time.

#### Example handoff

Presenter 2 can end with a line like:

"So now the agent is available in the places people work, and the business has the approvals, access controls, and audit trail to manage it in production."

Presenter 3 can begin with a line like:

"Once that foundation is in place, the next step is to make the agent better at its job and more cost-effective to run every day."

## One important note

The main risk in a three-person split is making the MANAGE section feel too short if the M365 and A365 section is brief in the live demo.

If that happens, Presenter 2 may feel more like a transition speaker than an owner of a full chapter. If needed, MANAGE can be broadened slightly to include more framing around why governance matters once agents leave the local proof-of-concept stage.

Even with that caution, this is still a strong split because it matches the actual progression of the story.

## Summary

If we keep the current story as written, the strongest three-person split is:

- Presenter 1 - BUILD: Setup, Sketch 0, Sketch 1, and the first part of Sketch 2
- Presenter 2 - MANAGE: the second part of Sketch 2 focused on M365 or A365 usage and governance
- Presenter 3 - OPTIMIZE: Sketch 3 and the close

This keeps the narrative intact while giving each speaker a clear role, clear handoff points, and a distinct point of view for the audience.