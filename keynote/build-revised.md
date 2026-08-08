# BUILD revised - local Canvas to grounded operations

## Goal
Start with a real finance request in GitHub Copilot, build and test an invoice-audit agent locally in Canvas, then move the same idea into Microsoft Foundry for approved contract grounding, traces, monitoring, and evals.

The throughline is simple: **work context shapes a local agent, Canvas proves its behavior, and Foundry makes that behavior inspectable and improvable at scale.**

Target runtime: **9:35**. This leaves about **25 seconds of buffer** for live navigation and loading while keeping BUILD under 10 minutes.

## Important terminology for the presenter

- The current `pharmashield-foundry-demo` GitHub Copilot skill is a demo launcher. It opens the checked-in live Canvas and does not itself contain the invoice-audit policy.
- A local Canvas is the place to shape and pressure-test the initial agent behavior before moving to the hosted version.
- A Foundry Skill is different. It is a centrally stored, versioned `SKILL.md` file that carries reusable behavioral guidance for agents.
- Frame the invoice-audit policy as a Foundry Skill only if it has actually been created and registered in Foundry for this demo.
- Foundry Skills are currently preview. If product status matters for this audience, state that briefly and move on.

## Part A - GitHub Copilot: from work request to a tested local agent (4:45)

### 1. Open with the finance scenario - 0:30
- Finance needs to review a supplier invoice against the terms it agreed to.
- The team needs a finding with evidence it can inspect, not a generic risk flag.
- Open GitHub Copilot at the work that prompted the request.

### 2. Show the work context, not a product tour - 0:40
- Use My Work, chats, and the project view as three views of the same request.
- Show the relevant issue, discussion, or project artifact that defines the invoice-audit need.
- Keep the point concrete: this is where the team captures the request and its shared context.

### 3. Introduce the shared audit guidance - 0:45
- Show the project-level audit skill or instruction artifact.
- Call out only the behavior that matters: review against evidence, separate confirmed findings from open questions, and cite supporting contract language.
- Explain that shared guidance keeps agents from drifting into different audit rules.

### 4. Build the first version in local Canvas - 0:55
- Open a local Canvas and create the initial invoice-audit agent.
- Show the essentials only: model, instructions, invoice input, and the output format for findings and open questions.
- State the purpose of this first pass: test the audit behavior before connecting it to production data or services.

### 5. Test the local agent in Canvas - 0:55
- Attach the Aster Ridge invoice and run the standard audit request.
- Show one clear local finding, such as the line-2 overstatement, and one question the agent cannot resolve without contract evidence.
- Emphasize restraint: the local agent identifies what needs verification rather than inventing a contract conclusion.

### 6. Connect the guidance to Foundry Skills - 0:30
- Show the invoice-audit `SKILL.md` or a prepared Foundry Skill view.
- Explain that Foundry stores the shared guidance separately from agent code, versions each update, and lets the team test a revision before making it the default.
- Do not imply that the GitHub Copilot launcher and Foundry Skill are the same artifact.

### 7. Transition to the hosted agent - 0:30
- Invoke `pharmashield-foundry-demo`.
- Describe it accurately: it opens the checked-in Canvas for the live Foundry-backed demo.
- Set up the contrast: local Canvas established the behavior. Foundry adds approved knowledge and operational controls.

**Part A subtotal: 4:45**

## Part B - Foundry: grounded audit, evidence, and continuous quality (4:50)

### 8. Show what changes in Foundry - 0:35
- In the live Canvas, identify the hosted model, the same audit guidance, and Foundry IQ or `contracts-kb` as the approved contract source.
- Briefly confirm that Azure authentication, the deployed agent, and contract retrieval are available.

### 9. Run the grounded invoice audit - 1:15
- Use the same Aster Ridge invoice and audit request from the local test.
- Show the priority findings, including the negotiated-rate discrepancy and any packaging charge that the retrieved contract evidence supports.
- Keep the language disciplined: the contract supports the finding. The model does not make the policy decision on its own.

### 10. Prove where the answer came from - 0:55
- Open Trace for the same run.
- Show the Foundry IQ retrieval call, the returned passages, and the contract clauses behind the findings.
- Land one message: finance can follow each claim back to its evidence.

### 11. Show what the team operates after deployment - 0:45
- Open monitoring for the agent.
- Highlight one representative signal, such as request volume, latency, failures, or retrieval quality.
- Keep it tied to the same audit run or agent. This is not a dashboard tour.

### 12. Evaluate changes before they become the default - 0:45
- Open the invoice-audit eval set or scorecard.
- Explain that a new Skill version can be tested for accurate findings, grounded citations, and restraint when evidence is missing.
- Show the quality checks that matter most: correct discrepancy detection, supporting citations, and no unsupported claims.

### 13. Close on the operating loop - 0:35
- Recap the arc: GitHub Copilot captures the work, local Canvas tests the behavior, and Foundry grounds, traces, monitors, and evaluates the agent.
- End on the eval or Skill version view, so the last image reinforces ongoing quality rather than a one-time deployment.

**Part B subtotal: 4:50**

## Total
- Planned content: **9:35**
- Demo and transition buffer: **0:25**
- Maximum session time: **10:00**

## Pacing and scope guardrails

- Treat My Work, chats, and project context as connected evidence of one request. Do not give each surface its own tour.
- The local Canvas test must have a visible purpose: prove the first version can find a concrete invoice issue and can admit what it does not know.
- Use the same invoice and core prompt in local Canvas and Foundry. That makes the value of contract grounding obvious without extra explanation.
- If the local agent starts slowly, use a prepared Canvas with the agent already configured. Keep the live test result and the unsupported-question moment visible.
- If the Foundry Skill is not configured in the demo environment, show the `SKILL.md` as the intended shared policy and say the live Canvas uses the deployed agent configuration. Do not claim a live attachment that is not present.
- Preserve the live readiness checks. A missing Azure login, deployed agent, permission, or `contracts-kb` connection should remain visible rather than being replaced with a fabricated result.
- Use one representative hosted agent run for Trace, monitoring, and evals where possible.
- If time slips, reduce the My Work overview and shorten the Foundry Skill explanation first. Protect the local Canvas test, grounded audit, Trace, and evals.
- Do not end with a Teams or multi-agent architecture tour unless it is visibly demonstrated. Save broader distribution and specialist-agent design for OBSERVE.

## Presenter closing line

"We started with the work itself, tested the audit behavior locally in Canvas, then used Foundry to ground, inspect, and evaluate that same agent against approved contract evidence."