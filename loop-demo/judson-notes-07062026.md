# Build A
- Instead of calling out vs code, mention if I wanted to get my hands on the code, I can (make it more natural and honest)
- The path is moving from protoype > Foundry > production (don't say enterprise, say production)
- Change 4.1 to 5.5 to align with Seth, but if I do mention 4.1, be honest: it's fast and cheaper than 5.5
- Created by Jessica, hardened on Foundry
- Make sure Seth and my agent pieces align in terms of what makes an agent (model + instructions, context, memory, tools) vs Seth (model + instructions, skills, tools)

# Observe 1
- through line with Jess's agent
- need to have better trace output (this requires a `contract-policy-expert` correction)
- more romancing the rubrics
- spend more time with the evals on what matters and why
- Keep FCP but romance observability at the foundry layer

# Observe 2
- get more precise on the wording
- sort out why agents show up more than once
- show a tenant with multiple agents
- why is an agent suspicious? 
- number in the cost should be ugly
- use word "RISK" in the final mop-up

# Tune 1
-   Is there a way to see the actual changes in the assets? (likely fix inside of GHC App)
-   Not take as much time in this section
-   we should align on the main vernacular and stick to it

# Tune 2
- One of our assumptions is we can use a smaller model (explain why change the model)
- better bridge into RFT - talk about other models and maybe explain WHY fine tuning - model picker screen - why one would be better - is there an honest way to go from "I have this model" to "I want to fine tune"
- change JSON contract to "Shape"
- I made my agent do it (where did the grader come from)

# Overall
- Pump up numbers > those are rookie numbers
- Confidence numbers? Explain perhaps?
- Add in that before we had no visibility, now we do... but I still have to go validate
- From Anne: any reference to CMO needs to be changed to contract manufacturers (because CMO can == Chief Marketing Officer)
- before we didn't know - now we do
- run water through the business logic of all of this (numbers should make sense)
- (From Jessica Hawk) i'd add the point around repeated use --> better results as well. The world has been trained that FT is only for the elite, which is no longer true thanks to Foundry

Edits from Mike H. 
 
# 1\. Adjustments to Narrative

## A. Overall story and taxonomy
- Anchor the full demo on the journey from GitHub Copilot App canvas prototype to production in Microsoft Foundry.
- Use “prototype to production” consistently. Replace “enterprise-ready” with “production,” “production agent,” or “move to production.”
- Build a master context-setting slide that explains the terms the audience will hear throughout: instructions, context, memory, skills, tools, IQ, evals, rubrics, dimensions, runtime, and evidence.
- Create a simple well-architected-agent framework that shows how these concepts compose and how the IQ platform fits into the broader market vocabulary.
- Reduce jargon in the spoken narrative and use the same terms across Jessica, Seth, and Judson’s sections.

## B. GitHub Copilot App, VS Code, and Foundry handoff
- Explain that GitHub Copilot App and canvas are ideal for visualizing agent structure and building with prompts.
- Add a crisp developer rationale for VS Code: when a developer wants deeper iteration, more tactile control, and hands-on work in the code, they can open VS Code.
- Add a narrative nod that the local agent prototype eventually needs to move into a managed production environment in Foundry.
- Position Foundry as the place the same agent moves into production rather than being rebuilt.

## C. Anatomy of an agent and IQ platform
- Explain the value of the anatomy-of-an-agent visualization early, since the center column consumes real estate and otherwise looks static.
- Pay off the visualization during the demo as context, memory, and tools/IQ light up and the agent becomes smarter.
- Avoid describing IQ as simply “a tool.” Tell the higher-level story: IQ is the differentiated Microsoft platform layer for grounding and compounding intelligence.
- Clarify how context and IQ relate: context starts with provided data; IQ expands the agent’s ability to reason over enterprise knowledge and connected systems.

## D. Observe / performance / rubrics
- Clarify naming and lineage: Jessica builds the Contract Policy Expert; the Assurance Orchestrator calls it; Foundry observes and evaluates it.
- Explain rubrics in plain language before showing rubric detail. Then explain that rubric dimensions are the specific criteria being graded.
- Call out that good news: rubrics can be automatically generated, so the user does not need to handcraft every evaluation criterion from scratch.
- Explain the grades as repeated evaluation runs: same agent, same dataset, five runs, showing standard deviation in performance that needs to be tightened.
- Reinforce observability at every layer: agent-level performance in Foundry and fleet-level governance, access, risk, and cost through Agent 365.

## E. Agent 365 / governance narrative
- Shorten the Agent 365 tour and focus on what matters: govern, manage, secure, risk, and cost across the fleet.
- Explain why the suspicious agent is suspicious. If the product screen does not show rationale, the talk track needs to provide it.
- Frame rejection as pre-publish risk assessment before an agent reaches production.
- Add “risk” explicitly to the summary statement alongside governance, security, management, and FinOps.

## F. Tune and optimization narrative
- Shorten Tune A. Make the point fast: Foundry Optimizer improves the agent by tuning prompts, instructions, skill definitions, and tool descriptions.
- Standardize language between Jessica’s first section and Seth’s tuning section. Choose one vocabulary for instructions, context, memory, tools, skills, and assets.
- In Tune B, explain why cost is tied to the model. The current screen does not make that obvious to a general audience.
- Bridge from cost problem to solution: we hypothesized the large model drove cost, tried other options, and chose fine-tuning a smaller model because it preserved quality while reducing cost.
- Update the tuning improvement explanation so the audience understands what changed and why it matters.

## G. Caldova app and business outcome

- Remove or soften “more room for business-critical mistakes.” Use language that creates urgency without ending on a negative note.

- Shorten the front-end setup before showing the app value.

- Increase confidence scores into the 90s for executive readability if practical, or explicitly explain that lower confidence means “where to investigate first,” not “auto-approve.”

- Clarify the business value: before, Caldova had no visibility into a sea of contracts and invoices; now it has targeted visibility into where risk and overpayment may exist.

- Make the human-in-the-loop workflow explicit: an 83% confidence overpayment signal tells the user where to dig in and validate.

# 2\. Adjustments to Demo Screens and Videos

## A. Canvas and agent anatomy visuals
- Reduce distraction from the center column. If it remains visible, explain its value and make it actively useful.
- Zoom into Rubber Duck / red-box moments so the audience sees the active area instead of the full wall of UI.
- Use camera movement or callouts to direct attention to the canvas and agent state changes.
- If the anatomy component remains on screen, make sure it visibly changes as files, memory, context, IQ, and tools are added.

## B. Build / prototype screens
- Make the transition from local canvas prototype to Foundry production visually clear.
- Keep the VS Code moment short and explanatory: “I can open the code if I want deeper control.”
- Use GPT-5.5 as the initial model if that better supports the later model-swap / tuning story, and include a concise explanation for the choice.

## C. Observe performance screens
- Clean up confusing agent names and duplicate-looking agent instances.
- Improve visual lineage across Contract Policy Expert, Assurance Orchestrator, and observability views.
- Make rubric dimensions easier to read and connect to the spoken explanation.
- If telemetry shows the orchestrator talking to itself, adjust telemetry or visualization so sub-agent calls are obvious.

## D. Agent 365 / Observe B screens
- Shorten the volume of visible agents and avoid overwhelming the viewer.
- Show a more diverse inventory: Microsoft agents, customer-created agents, SAP, ServiceNow, partner agents, and agents from multiple sources.
- Improve owner, publisher, and source attribution so the audience can see why different categories matter.
- Make the suspicious / risky agent visually obvious, with clearer pre-publish rationale.
- Increase contract-agent overrun cost to make the before case materially worse and the after case more compelling.

## E. Tune A screens

- Make what changed in tuning visually obvious: highlight only the changed prompt, instruction, skill, or tool-description differences.

- Avoid asking the audience to compare long side-by-side text blocks where the visible lines appear identical.

- Shorten the section and focus on the result: better agent behavior through optimized assets.

## F. Tune B screens

- Show why cost points back to the model. If the product screen does not explain that, use a supplemental visual or narrative bridge.

- Add a simple model-comparison or model-selection moment before jumping into reinforcement fine-tuning.

- Rationalize dollar savings with a larger business problem so the payoff feels worth the effort.

- Make the cost reduction result visually crisp and easy to remember.

## G. Caldova app screens

- Increase or explain confidence scores so the business viewer does not interpret 73–83% as weak performance.

- Show overpayment detection, evidence, and human review workflow more explicitly.

- Show the before/after contrast: no visibility before; now a clear map of where to investigate.

- Keep the final app reveal strong and concise.

# 3\. Feedback for Product Teams

## A. Agent build experience

- The canvas center column takes substantial real estate and can appear inactive unless it visibly pays off during the demo.

- Product should better support focus/zoom/red-box style guidance so presenters can direct attention during agent-building workflows.

- Agent composition needs to be easier to explain visually, especially context, memory, instructions, tools, skills, and IQ.

## B. Foundry and IQ taxonomy

- Calling IQ a “tool” undersells the platform. Product and marketing need aligned nomenclature for IQ, tools, context, grounding, and harness/runtime ownership.

- Clarify how Foundry IQ, Work IQ, tools, and context appear in product surfaces and how they should be described externally.

- Need principled, uniform naming across IQ experiences so teams do not create confusion in keynote/demo narratives.

## C. Observability and evaluation

- Agent naming and lineage are confusing. Product needs clearer parent/child relationships and visible agent lineage.

- Observability should make it clear which agent was built, which orchestrator uses it, and how the evaluation maps back to that agent.

- Rubrics, dimensions, graders, and evals need clearer product explanations for non-expert audiences.

- Surface repeated-run variance / confidence / standard deviation in a more intuitive way for business and seller audiences.

## D. Agent 365 governance and risk

- Approval workflow should explain why an agent is risky or suspicious, especially before production/publish approval.

- Improve publisher, owner, and source attribution so admins can distinguish Microsoft, customer-built, partner, SAP, ServiceNow, Copilot Studio, and Foundry agents.

- Product should better represent ecosystems with agents from anywhere, not just one internal tenant or one source.

- Pre-publish risk assessment should be visible and actionable, not dependent on presenter explanation.

## E. Cost, model choice, and optimization

- Product should help users identify when model choice is driving cost.

- Surface recommendations for alternative models, fine-tuning opportunities, and optimization paths.

- Explain causality between model choice, quality, latency, cost, and tuning path more clearly.

- Connect Foundry cost/performance data with Agent 365 fleet-level cost and operational views.

## F. Cross-platform observability roadmap

- Continue roadmap alignment between Foundry observability and Agent 365 observability.

- Create a cleaner end-to-end story linking development, observability, governance, security, risk, and FinOps.

- Clarify whether eval data and operational data flow into Agent 365, and make that cross-platform story easier to tell.
