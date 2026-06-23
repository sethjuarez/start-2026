# Two-Person Demo Split - Build and Manage

This is a proposed presenter split for the current demo flow without changing the underlying story. The goal is to divide the narration into two clear roles that feel natural on stage and easy for the audience to follow.

## Recommended split

- Presenter 1: BUILD
- Presenter 2: MANAGE

This works because the story already has two natural halves. First, we establish the invoice assurance problem, show what Waypoint is doing, and build the first working agent. Then we show how that agent is operated inside the enterprise with governance, evaluation, and cost control.

## Presenter 1 - BUILD

Presenter 1 owns the creation arc. This speaker introduces the business problem, shows the product outcome in Waypoint, and walks through how the first version of the agent is built and brought into an enterprise-ready environment.

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

Presenter 2 owns the operating arc. This speaker picks up once the agent is enterprise-ready and explains how it is used, governed, improved, and run cost-effectively inside Pharma Company.

### Recommended coverage

- Sketch 2 - Microsoft Foundry, M365, and A365 - from M365 or A365 autopilot onward
- Sketch 3 - Hill Climbing
- Suggested Close

### What this speaker is responsible for

- Show how the hosted agent becomes available in M365 or A365 and can be used in Teams
- Explain approvals, listing, access, and auditability in A365
- Show how governance supports production use inside Pharma Company
- Walk through rubric evaluators, generated rubrics, and evaluation runs in Foundry
- Explain how Agent Optimizer improves contract reasoning, evidence use, and recommendation quality
- Show how cost is measured and how hill climbing helps move learned behavior into a smaller model
- Tie quality and cost improvements back to a production setting where many invoice reviews may run every day
- Close by returning to payment accuracy, reduced leakage, and confidence in invoice assurance

### Core message

Once the agent works, the next question is how to run it inside the business with governance, adoption, quality controls, and the right cost profile.

## Why this split works

### 1. It follows the audience's questions

The first half answers: what is the problem, what did we build, and how does it work.

The second half answers: how do we use it, govern it, improve it, and control cost.

### 2. It gives each presenter a distinct role

BUILD sounds like the builder and explainer.

MANAGE sounds like the operator and scale owner.

That makes the transition feel intentional instead of arbitrary.

### 3. It is easy to remember

Build it. Then manage it.

That is a simple frame for the audience and for the presenters.

## Best handoff point

The cleanest handoff is inside Sketch 2, after the hosted agent is deployed in Foundry.

At that point, Presenter 1 has completed the story of how the agent is built and connected to enterprise evidence. Presenter 2 can then pick up with how the agent is used in day-to-day work and how the business governs and improves it over time.

### Example handoff

Presenter 1 can end with a line like:

"At this point, the invoice review agent has moved beyond a local proof of concept. It is connected to the right enterprise evidence, and now it can run as a hosted agent in Foundry."

Presenter 2 can begin with a line like:

"From here, the next question is how this shows up in day-to-day work, and how Pharma Company governs it once more teams start relying on it."

## One important note

Build should not be interpreted too narrowly as only developer setup.

Sketch 0 belongs with BUILD because it defines the invoice assurance job the agent is being built to do. If Sketch 0 were moved into MANAGE, the first speaker would lose the business grounding that makes the technical build meaningful.

A stronger definition is:

- BUILD = problem, product outcome, initial agent creation, and enterprise connection
- MANAGE = enterprise usage, governance, evaluation, optimization, and cost control

## Summary

If we keep the current story as written, the strongest two-person split is:

- Presenter 1 - BUILD: Setup, Sketch 0, Sketch 1, and the first part of Sketch 2
- Presenter 2 - MANAGE: the second part of Sketch 2, Sketch 3, and the close

This keeps the narrative intact while giving each speaker a clear role, a natural handoff, and a distinct point of view for the audience.