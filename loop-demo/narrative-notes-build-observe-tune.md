Setup: Pharma Company is under pressure to move faster while relying more heavily on contract manufacturing organizations (CMOs). That increases the volume and complexity of CMO invoices. More suppliers, more contract terms, more milestone logic, and more approval context all make payment decisions harder to trust. Waypoint is Pharma Company's internal invoice assurance application. It checks what was billed against what was contracted, authorized, delivered, released, and approved.

This version of the story is organized around three simple ideas: Build, Observe, and Tune. Start with the business problem and why invoice assurance has become harder to trust. Then show how the agent system is built, observed, and tuned. End in Waypoint so the audience lands on the application and the business outcome.

# Sketch 0 - Problem framing
Start with the business problem, not the app. Establish why CMO invoice review has become hard to manage by hand and why Pharma Company needs a more trustworthy way to make payment decisions.
- Frame the pressure clearly: more contract manufacturers, more contract terms, more milestone logic, and more approval context.
- Make the risk visible in business terms: payment leakage, slower decisions, and less confidence in what should be approved, disputed, or escalated.
- Introduce Waypoint as Pharma Company's internal invoice assurance application, but do not spend time in the product yet.
- Set up the story clearly: if this is the problem, how do we build the agent system, observe its behavior, tune it for production, and finally see the result in the app?

# Build - From local proof of concept to enterprise agent fleet
The Build section answers a basic question: how do we create an agent system that can actually do this work at enterprise scale?

## Sketch 1 - Build the first version in GitHub Copilot
Use the GitHub Copilot app to create a local proof of concept. The goal is to show that a local agent can approximate invoice review for Waypoint against local contracts and supporting records.
- Show the main surfaces briefly: Home, My Work, Automations, and Chat.
- Show the project-level working areas: chat, rubber duck, actions, agent merge, and canvas.
- Show the first agent being created and run in canvas with a local model and MXC.
- Be explicit that this stage is a proof of concept using local or simulated data, not the final enterprise operating model.
- Tie the agent back to the Waypoint task: reviewing invoice lines against contract and operating evidence.
- Keep the pacing brisk. The point is to show that the task is feasible before we expand and harden it.

## Sketch 2 - Build for enterprise use in Foundry and M365
Now move the same idea into an enterprise setting. We have proved the concept locally. This step connects the system to real data, adds guardrails, and turns one proof of concept into a governed fleet of agents that people can use where they already work.
- Move to VS Code and show how the agent system gets connected to the right IQs. The POC simulated the data. This step brings in real enterprise data and visible guardrails on tool calls.
- Name the key IQs clearly: Work IQ for email and Microsoft 365 context, Foundry IQ for indexed contracts in the knowledge base, Fabric IQ for structured invoice data, and Web IQ for current external financial context when needed.
- Show the toolbox and explain how those IQs let the fleet pull together contract terms, invoice records, approvals, correspondence, and outside signals in one review flow.
- Deploy hosted agents in Foundry. Show cloud isolation and a simple execution path.
- Move the agents into M365 as autopilots that can be used in Teams. Show a short interaction tied to invoice assurance work.
- Land the section with a simple point: we have moved from one local build to an enterprise agent fleet inside Pharma Company.

# Observe - First inspect performance, then zoom out to governance and cost
Observe should keep a single chapter shape, just like Build. That means separate sketches for the close-up view and the zoomed-out operating view.

## Sketch 3 - Observe performance in Foundry
Continue in Foundry and stay with the same invoice-review system. The goal here is to show how we inspect whether the agents are doing the work the right way.
- Show tracing so the audience can see the path through the evidence.
- Show rubrics.
- Show evals.
- Keep the examples grounded in the actual job: contract reasoning, evidence use, and recommendation quality.
- Make the point that this is how we inspect agent quality in production.

## Sketch 4 - Observe governance and cost in A365
Now widen the frame from one run to the broader operating view in A365.
- Show all agents in 365.
- Show the list view.
- Show approvals.
- Show access and auditability.
- Show cost.
- Make the point that Observe is not only about model behavior inside one run. It is also about how the fleet is governed and what it costs once it is deployed across the business.

# Tune - Improve quality and lower cost
The Tune section starts from what we just observed. We have evidence about performance in Foundry, and we have visibility into governance and cost in A365. Now we use both to improve the system.

## Sketch 5 - Tune the agent and model in Foundry
Start with the impetus of performance plus cost.
- Use Foundry and show how traces can help auto-optimize the agents.
- Show how the evaluation signals from the Observe section feed into agent optimization.
- Keep the examples tied to the invoice-review task so the improvement feels concrete.
- When we want a smaller model with the right behavior, that is when we tune.
- Go through fine-tuning plus RLE in Foundry.
- Show the hill-climbing motion of carrying what we learned into a smaller model.
- Tie the result back to the final app outcome: the same invoice-review task, better quality where it matters, and lower run cost at scale.

# Sketch 6 - End in Waypoint
Close in the app. Return to Waypoint and show the business outcome now that the agent system has been built, observed, and tuned.
- Start in the invoices tab and show several invoices with decisions already made: matched, variance, and disputed.
- Put real dollars on the screen so the audience sees recovery opportunity and risk, not just status labels.
- Show the evidence behind a few decisions: contract terms, PO or receipt context, batch records, QA release, milestone status, and invoice lines.
- If useful, show a batch reconciliation result with the relevant IQs enabled so the audience sees scale, not just a single invoice.
- Keep the framing on Pharma Company's internal invoice assurance process, not routine invoice processing.
- Land the final point clearly: this is what the full build, observe, and tune loop delivers inside the business.

# Suggested Close
Close by returning to the business outcome in Waypoint. Waypoint gives Pharma Company a way to review complex CMO invoices against the full operating record, surface issues with evidence, and scale that review with governed agents. The story starts with the business problem, then shows how the agent system is built, how its behavior is observed in production, and how it is tuned to improve quality and run cost. It ends in the application, where those improvements show up in real invoice decisions. The result is better payment decisions, less leakage, and more confidence in a process that has become harder to manage by hand.

# Optional framing notes
- Use Build, Observe, and Tune as section labels in narration and slide titles, even if the underlying product names change by segment.
- Start with the problem. End with the app.
- Keep Waypoint as the anchor at the end so the story lands on a business decision, not a tooling tour.
- In Build, start with one local proof of concept, then widen to a fleet of governed agents.
- In Observe, keep the two-sketch flow simple: first performance in Foundry, then governance and cost in A365.
- In Tune, make sure the audience feels the handoff from Observe: we saw what happened, now we improve it.
- If marketing wants softer labels, alternatives could be Build, Measure, Improve or Build, Evaluate, Optimize.
