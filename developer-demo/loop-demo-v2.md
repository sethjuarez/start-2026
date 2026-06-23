# Loop Demo v2

## Setup
Pharma Company is under pressure to move faster while relying more heavily on contract manufacturing organizations, or CMOs. That increases the volume and complexity of CMO invoices. More suppliers, more contract terms, more milestone logic, and more approval context all make payment decisions harder to trust. Waypoint is Pharma Company's internal invoice assurance application. It checks what was billed against what was contracted, authorized, delivered, released, and approved.

This story is organized around three simple ideas: Build, Observe, and Tune. It starts with the business problem and why invoice assurance has become harder to trust. It then shows how the agent system is built, observed, and tuned. It ends in Waypoint so the audience lands on the application and the business outcome.

## Business Context
Start with the business problem, not the app. Establish why CMO invoice review has become hard to manage by hand and why Pharma Company needs a more trustworthy way to make payment decisions.
- The pressure is increasing: more contract manufacturers, more contract terms, more milestone logic, and more approval context.
- The business risk shows up as payment leakage, slower decisions, and less confidence in what should be approved, disputed, or escalated.
- Waypoint is introduced as Pharma Company's internal invoice assurance application, without spending time in the product yet.
- The story then follows a clear sequence: how the agent system is built, how its behavior is observed, how it is tuned for production, and how that work shows up in the app.

## Build - From local proof of concept to enterprise agent fleet
The Build section answers a basic question: how do we create an agent system that can actually do this work at enterprise scale?

### Build the first version in GitHub Copilot
This section uses the GitHub Copilot app to create a local proof of concept. The goal is to show that a local agent can approximate invoice review for Waypoint against local contracts and supporting records.
- Briefly show the main surfaces: Home, My Work, Automations, and Chat.
- Show the project-level working areas: chat, rubber duck, actions, agent merge, and canvas.
- Show the first agent being created and run in canvas with a local model and MXC.
- Make clear that this stage is a proof of concept using local or simulated data, not the final enterprise operating model.
- Tie the agent directly to the Waypoint task: reviewing invoice lines against contract and operating evidence.
- The purpose of this section is to establish that the task is feasible before the system is expanded and hardened.

### Build for enterprise use in Foundry and M365
This section moves the same idea into an enterprise setting. The concept has been proved locally. The next step is to connect the system to real data, add guardrails, and turn one proof of concept into a governed fleet of agents that people can use where they already work.
- Move to VS Code and show how the agent system connects to the right IQs. The proof of concept simulated the data. This step brings in real enterprise data and visible guardrails on tool calls.
- Name the key IQs clearly: Work IQ for email and Microsoft 365 context, Foundry IQ for indexed contracts in the knowledge base, Fabric IQ for structured invoice data, and Web IQ for current external financial context when needed.
- Show the toolbox and how those IQs bring together contract terms, invoice records, approvals, correspondence, and outside signals in one review flow.
- Deploy hosted agents in Foundry and show cloud isolation with a simple execution path.
- Move the agents into M365 as autopilots that can be used in Teams, with a short interaction tied to invoice assurance work.
- The section ends with a simple point: the system has moved from one local build to an enterprise agent fleet inside Pharma Company.

## Observe - From performance inspection to governance and cost
Observe keeps the same chapter shape as Build, with one close-up view and one operating view.

### Observe performance in Foundry
This section stays in Foundry and focuses on the same invoice-review system. The goal is to show how the team inspects whether the agents are doing the work the right way.
- Show tracing so the audience can see the path through the evidence.
- Show rubrics.
- Show evals.
- Keep the examples grounded in the actual job: contract reasoning, evidence use, and recommendation quality.
- The point of this section is that this is how agent quality is inspected in production.

### Observe governance and cost in A365
This section widens the frame from one run to the broader operating view in A365.
- Show all agents in 365.
- Show the list view.
- Show approvals.
- Show access and auditability.
- Show cost.
- The point of this section is that Observe is not only about model behavior inside one run. It also covers how the fleet is governed and what it costs once deployed across the business.

## Tune - Improve quality and lower cost
The Tune section starts from what was learned in Observe. Performance is visible in Foundry, and governance and cost are visible in A365. That information is then used to improve the system.

### Tune the agent and model in Foundry
This section begins with the combined pressure of performance and cost.
- Use Foundry and show how traces help auto-optimize the agents.
- Show how the evaluation signals from the Observe section feed into agent optimization.
- Keep the examples tied to the invoice-review task so the improvement feels concrete.
- When a smaller model is needed with the right behavior, this is where tuning comes in.
- Go through fine-tuning plus RLE in Foundry.
- Show the progression of carrying what was learned into a smaller model.
- Tie the result back to the final app outcome: the same invoice-review task, better quality where it matters, and lower run cost at scale.

## End in Waypoint
Close in the app. Return to Waypoint and show the business outcome now that the agent system has been built, observed, and tuned.
- Start in the invoices tab and show several invoices with decisions already made: matched, variance, and disputed.
- Put real dollars on the screen so the audience sees recovery opportunity and risk, not just status labels.
- Show the evidence behind a few decisions: contract terms, PO or receipt context, batch records, QA release, milestone status, and invoice lines.
- If useful, show a batch reconciliation result with the relevant IQs enabled so the audience sees scale, not just a single invoice.
- Keep the framing on Pharma Company's internal invoice assurance process, not routine invoice processing.
- The final point is clear: this is what the full Build, Observe, and Tune loop delivers inside the business.

## Closing Message
Close by returning to the business outcome in Waypoint.
- Waypoint gives Pharma Company a way to review complex CMO invoices against the full operating record.
- It surfaces issues with evidence and helps scale that review with governed agents.
- The story starts with the business problem, then shows how the agent system is built, how its behavior is observed in production, and how it is tuned to improve quality and run cost.
- It ends in the application, where those improvements show up in real invoice decisions.
- The result is better payment decisions, less leakage, and more confidence in a process that has become harder to manage by hand.
