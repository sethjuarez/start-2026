Observe

PERF
- continue in foundry 
- show tracing
- show rubrics
- show evals

ZOOM OUT

COST
- All agents in 365
- show list
- show approvals
- show cost


TUNE
Foundry - start with the impetus of perf + cost
Tuning the agent
- surprise - traces can help auto optimize

Tuning the model
- when we want a smaller model with the right behavior - that's when we tune
- go through FT + REL in Foundry
- cover with waypoint e2e

# Moar Notes
# Executive Summary

The strongest direction from Alysa was:

> **The chapter should explicitly demonstrate Build, Observe, Tune.**

She noted that the current demo has the **build** motion, but lacks a sufficiently clear **observe** motion and needs a more explicit **tune** story. She repeatedly framed this as the core architecture of Seth's chapter and as the feedback Judson was pushing for.

# Key Revisions Alysa Requested

## 1. Start in the GitHub Copilot App

Alysa said she would strongly prefer that Seth begin inside the GitHub app rather than elsewhere.

### Why?

She felt the current flow is confusing because the audience sees an application and then later discovers it was built in GitHub.

Her recommendation:

- Start with the business challenge.
- Immediately move into GitHub.
- Build the application.
- Show how the app solves invoicing/revenue-recovery problems.
- Then continue through the lifecycle.

### Action

**Seth should restructure the opening sequence to begin inside GitHub and build the application first.**

## 2. Resolve the Scout → GitHub Handoff

Alysa explicitly called out that she was unclear on the connective tissue between Scout and Seth's GitHub section.

Open question:

> How do we transition naturally from Scout into Seth's build experience?

Ideas discussed:

- Scout could identify an invoicing problem.
- Scout could trigger an alert.
- Scout could surface missed revenue or invoice inaccuracies.
- That becomes the reason the application must be built.

### Ownership

Jason volunteered to schedule a separate working session with the Scout team and Seth to determine this handoff.

### Outstanding

This remains unresolved.

## 3. Introduce an Explicit "Observe" Layer

This was one of Alysa's strongest themes.

She stated:

> We have build.
>
> We don't really have observe.

Her concern was that the demo currently focuses heavily on creation of the solution but not sufficiently on operating it.

She wants:

- The app built.
- The app deployed.
- Agent behavior observed.
- Operating data surfaced.
- Agent performance reviewed.

Specifically she referenced:

- Agent 365
- Observability
- Visibility into agent behavior
- Identifying when an agent goes rogue

### Desired Story

1. Build
2. Observe
3. Tune

rather than just:

1. Build
2. Deploy

## 4. Add a Clear Frontier Tuning Story

Alysa specifically called out frontier tuning as something that felt missing from the experience.

Her question:

> Once the app is running and the agent is operating, should we demonstrate frontier tuning?

The rationale:

- Developer creates the app.
- Agent is deployed.
- Agent is being used.
- Copilot can reason over the agent.
- Then show optimization/improvement.

### Seth's Response

Seth proposed two versions:

**Option A**

- Use upcoming Microsoft 365 Frontier Tuning capabilities.

**Option B**

- Use Foundry tuning and tracing capabilities.
- Present tuning metrics inside the application.

### Alysa's Position

She was flexible on implementation details but wanted tuning represented explicitly regardless of which technology backed it.

## 5. Build a "Build → Observe → Tune" Chapter Structure

Later Alysa summarized the chapter exactly this way:

> Build, observe, tune.

She stated that if she thought about Seth's chapter as discrete sections, that is how she would organize it.

### Recommended structure

### Chapter A: Build

- Build the app.
- Use GitHub.
- Use enterprise-grade services.
- Create the agent.

### Chapter B: Observe

- Monitor the deployed agent.
- Use Agent 365/observability tooling.
- Review performance.
- Review operational metrics.
- Identify problems.

### Chapter C: Tune

- Perform optimization.
- Tune the agent.
- Improve outcomes.
- Demonstrate closed-loop improvement.

## 6. Demonstrate a Rogue Agent / Optimization Scenario

Alysa provided an example storyline:

- Build the agent.
- Observe it through Agent 365.
- Notice one agent is behaving poorly.
- Tune it.
- Improve outcomes.

She described this as the sort of operating loop Judson wants to see.

### Desired Outcome

Not merely:

> "We built an app."

But:

> "We built it, monitored it, discovered an issue, and optimized it."

## 7. Improve Product Truth Between Foundry, Copilot Studio, and GitHub

Alysa acknowledged there is increasing overlap among:

- GitHub
- Copilot Studio
- Foundry

and the resulting story is becoming fuzzy.

She wants the chapter to:

- stay believable,
- have clean product boundaries,
- avoid confusing transitions,
- maintain a coherent persona journey.

Seth, Bryan, Jessica, and related teams were identified as needing to work through the cleanest implementation path.

# Open Action List for Seth

### High Priority

- Start the chapter in GitHub App.
- Redesign around Build → Observe → Tune.
- Add explicit observability content.
- Add explicit tuning content.
- Determine the Scout → GitHub transition.
- Work with Bryan/Jessica/team on the best product-truth story.

### Medium Priority

- Evaluate Frontier Tuning vs Foundry tuning approach.
- Demonstrate an agent optimization or rogue-agent scenario.
- Integrate Agent 365/FinOps/observability where practical.

### Alysa's Bottom-Line Message

The most important feedback from Alysa was not about a specific technology choice. It was that Judson wants a lifecycle story:

**Build the agent → Observe the agent in production → Tune and improve the agent.**