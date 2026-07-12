Now that we've validated our idea locally, the next step is moving it into Foundry so it can become a production-ready agent or fleet of agents.

One of my favorite features of the GitHub Copilot app is that I can hand my work directly into my preferred editor. With a single click, I can open the entire project in Visual Studio Code and continue building without losing any context.

Thanks to the magic of demo editing, I've already completed some of that work.

Here we're looking at the code that connects our application to Foundry. The setup is intentionally straightforward. We establish a connection to our Foundry project, authenticate using our credentials, choose the model we want to use, and we're ready to start building agents.

The real power comes from extending those agents with enterprise knowledge.

Rather than relying only on the language model, we can connect to services like WorkIQ, FabricIQ, SharePoint, and Microsoft Teams. Those integrations allow the agent to retrieve organizational knowledge and incorporate it into its reasoning, resulting in recommendations that are grounded in your business data rather than just the model's training.

As we're building, we don't have to leave Visual Studio Code to test any of this.

The Foundry Toolkit gives us direct access to our hosted models, playgrounds, session history, traces, and evaluations. I can interact with the agent, inspect how it's reasoning, review execution traces, and evaluate its performance, all from within the editor.

Once we're happy with the results, publishing the agent is straightforward.

Because it's hosted in Foundry, we can make it available through Microsoft Teams, allowing people to interact with it from a tool they already use every day.

Here's our invoice analysis agent running inside Teams.

I can mention the agent, ask it questions about an invoice, or request an analysis, and it responds with the same reasoning and capabilities we built throughout this workflow.

What started as a local prototype in the GitHub Copilot app has now become an enterprise-ready agent that securely connects to organizational data, runs in Foundry, and is available directly inside the collaboration tools your users already rely on.
