Setup: The business has already identified pressure to move faster and rely more heavily on contract manufacturers. We pick up at the point where increased contract manufacturing activity creates risk: more supplier invoices, more contract terms, more approval context, and more chances for leakage or compliance-sensitive mistakes (like over billing, under billing, or general contract or policy violations which could cause legal risk). Our solution is to use our company intelligence coupled with agents to make it all work!

# Sketch 0 - Waypoint Invoice Reconciliation
Start with the end in mind! Walk through the actual problem and solution!
- start in the invoices tab, show several invoices and agentic decisions that have been made
- attach actual dollars to the agentic solutions
- show a batch run of the process (with all the IQ's enabled) - perhaps start this at the beginning of the demo to get back to at the end.

# Sketch 1 - GitHub Copilot App - Our First Agent POC
Use the GitHub Copilot app to create a POC locally. This POC should prove out if a local agent can approximate our invoice reviews against local contracts
- show macro level things like Home, My Work, Automations and Chat
- show project level things like chat, rubber duck, actions, agent merge, and canvas
- show agent creation and running in a canvas using local model and MXC

# Sketch 2 - Microsoft Foundry, M365, and A365 - Our Agents Grow Up
Use Microsoft Foundry to make our agents enterprise ready and available at scale. Now that we've proved out our agent locally, we need to move it an enterprise environment that has all of the security, governance, and observability controls we need to deploy at scale in our enterprise.
- move to VSCode and show adding a toolbox with the appropriate IQs - our POC only _simulated_ our data, now its time to add real data via IQs. Show safety and guard rails for the tool calls
- deploy as hosted agent to Foundry, show isolation (similar to MXC but in the cloud) and execution of simple agent
- move agent to M365/A365 as an autopilot we can chat with in teams (show interaction)
- show agentic governance in A365 (approvals, listing, etc)
- [BONUS] Finish by emailing an invoice to the autopilot agent at the beggining and pay of the reconciliation in the app

# Sketch 3 - Hill Climbing
Now that we've been able to create and use these agents, our goal is to make them:
1. Better at their respective jobs,
2. and more cost effective
## Part 1 - Better at their jobs
- Show Foundry's rubric evaluators and how it can auto-generate rubrics based on traces
- Show the generated rubrics and how evaluations can be used against the rubrics to test
- Show how we can optimize our agent using the generated rubrics and tests using the new Foundry Agent Optimizer
## Part 2 - More Cost Effective
- Show cost in new A365 window
- Show hill climbing exercise for moving all of our learnings from *Part 1* into a smaller model and how the RLE helps us achieve near parity with a larger model with a more cost effective result

