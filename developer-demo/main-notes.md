# Importan Pieces of the demo
This is main notes for the demos.

## Carissa Notes
3. on copilot studio - we know the underlying product truth/toolchain to connect the low code --> pro dev handoff is evolving very quickly. Judson's guidance was to harden the *scenario* that connects the two parts of that story, and let the product that's demoed to pay off that scenario evolve over the course of the year. so for now, if that's some kind of export button to get the spec output over to github, that's fine - if there's eventually a single app, we can shift to that. but the human scenario of business leaders who vibe code and pro devs who harden the same will be real, regardless of the toolchain. Ryan Martin and Seth Juarez, i think this might adjust how you build something for Start and then we'll just need to evolve it in the fall.

4. for the build scenario, Elijah's Build demo is a great foundation - Judson especially liked how Fabric IQ showed up in that one. Seth Juarez and Mike Hulme that's the starting blueprint for the next rev!

5. holistically though, we are missing one really important piece - closing the loop with Agent 365. it's not just observe and govern, it's also feeding into a loop of continuous improvement and performance evaluation. that element of performance/token efficiency keeps getting removed from the last chapter and it needs to be part of the flow. Erin Friedman and Ward Starbird i'm not sure if this is you or a different team - if we need to add someone else from Agent 365 who can cover the FinOps element of its value, please let me know who.

## Important Pieces
Things to have

- Copilot app +1 other surface (CLI, VS Code)
- rubber duck (show multi-model) - stretch to include different reasoning levels for different use case (general CI vs. bigger security issue)
- **something** that shows larger GHE platform (CI/CD in an agent-development flow)
- MDASH, Defender
- Foundry (foundry agent service)
- Foundry IQ, Work IQ, Web IQ
- Horizon DB

## From Mike Hulme
Updated to bring in Frontier Tuning. Let me know if I missed anything Seth.

# Build Chapter B

Build a fleet of agents to improve supply chain operations - inventory, out-of-stock, availability-to-promise

Starting in GitHub Copilot App, I bring in an existing app from Copilot Studio (TBD)

In GitHub Copilot App, I run multiple agent sessions, all in parallel, with each session working in its own isolated work tree, getting 2nd opinions from other models with Rubber Duck, and managing their own review cycles in draft pull requests. Beyond productivity this is AI native development with agents orchestrating the entire software lifecycle

Security isn’t something we manage in isolation. MDASH plays an active role in the SDLC loop. Code is scanned, exploits are proven in a sandbox, and findings flow back to the developer as a Copilot PR with proof and regression tests attached: Found, Proven, Fixed before the agent ever ships.

Using Foundry, I choose a model trained to my specific business (Frontier Tuning), and connect to my knowledge base and deploy to production

My supply chain agents are now operating as a production system, with live telemetry returning insights grounded internal knowledge and external context, giving me a single model of the business

Reveal backend grounding of agents using Microsoft IQ

My agents operate as an extension of our teams, fully integrated into our processes and our flow of work, actively engaging in Microsoft Teams and M365.

what do these fleet of agents do?

Judson keeps citing individual agents that work together but do specific tasks:

- inventory
- out-of-stock
- availability-to-promise