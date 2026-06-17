Setup: The business is already under pressure to move faster and rely more heavily on contract manufacturers. We pick up where that increased CMO activity starts to create risk: more supplier invoices, more contract terms, more approval context, and more chances for payment leakage or compliance-sensitive mistakes. In this demo, Waypoint is the internal name of Pharma Company's invoice assurance application. "Pharma Company" is the placeholder company name. Waypoint represents the internal software that validates what was billed against what was contracted, authorized, delivered, released, and approved.

# Sketch 0 - Waypoint Invoice Reconciliation
Start with the outcome. Show the invoice assurance problem clearly, then show how Waypoint resolves it inside Pharma Company. If the company name appears on screen or in notes, treat "Pharma Company" as a stand-in name that marketing can replace later.
- Start in the invoices tab and show several invoices with decisions already made: matched, variance, and disputed.
- Attach real dollars to the findings so the audience sees recovery opportunity and risk, not just flags.
- Show the evidence behind a few decisions: contract terms, PO or receipt context, batch records, QA release, milestone status, and invoice lines.
- Run a batch reconciliation with all relevant IQs enabled. If helpful, kick this off at the start of the demo and return to the results here.
- Keep the framing on Pharma Company's internal invoice assurance process, not routine invoice processing.

# Sketch 1 - GitHub Copilot App - Our First Agent POC
Use the GitHub Copilot app to create a local proof of concept. The goal is to show that a local agent can approximate invoice review for Waypoint against local contracts and supporting records.
- Show the main surfaces briefly: Home, My Work, Automations, and Chat.
- Show the project-level working areas: chat, rubber duck, actions, agent merge, and canvas.
- Show the agent being created and run in canvas with a local model and MXC.
- Be explicit that this stage is a proof of concept using local or simulated data, not the final enterprise operating model.
- Tie the agent back to the Waypoint task: reviewing invoice lines against contract and operating evidence.

# Sketch 2 - Microsoft Foundry, M365, and A365 - Our Agents Grow Up
Use Microsoft Foundry to make the agent enterprise-ready and available at scale. We have proved the concept locally. Now we move it into an environment with the security, governance, and observability needed for production use inside Pharma Company.
- Move to VS Code and show how the agent gets connected to the right IQs. The POC simulated the data. This step brings in real enterprise data and visible guardrails on tool calls.
- Show the toolbox and explain what evidence the agent can now access: contracts, invoice records, receipts, batch records, quality status, milestone approvals, materials, and capacity context.
- Deploy the agent as a hosted agent in Foundry. Show cloud isolation and a simple execution.
- Move the agent into M365 or A365 as an autopilot that can be used in Teams. Show a short interaction tied to invoice assurance work.
- Show governance in A365: approvals, listing, access, and auditability.
- Optional close: email an invoice to the autopilot agent near the beginning, then complete the reconciliation back in Waypoint here.

# Sketch 3 - Hill Climbing
Now that the agents are working, the next goal is to improve quality and lower cost.

## Part 1 - Better at their jobs
- Show Foundry rubric evaluators and how rubrics can be generated from traces.
- Show the generated rubrics and how evaluations are run against them.
- Show how those rubrics and tests help improve the invoice-review agent using Foundry Agent Optimizer.
- Keep the examples grounded in the actual task: better contract reasoning, better evidence use, and better recommendation quality.

## Part 2 - More cost effective
- Show cost in the new A365 window.
- Show the hill-climbing exercise for carrying what we learned in Part 1 into a smaller model.
- Explain how the RLE helps the smaller model approach the larger model's quality at a lower operating cost.
- Tie the savings back to a production deployment where many invoice reviews may run every day.

# Suggested Close
Close by returning to the business outcome. Waypoint gives Pharma Company a way to review complex CMO invoices against the full operating record, surface issues with evidence, and scale that review with governed agents. The story starts with a real invoice decision in Waypoint, shows how the agent is built and hardened for production, then ends with a path to keep quality high while lowering run cost. The result is better payment decisions, less leakage, and more confidence in a process that has become harder to manage by hand.