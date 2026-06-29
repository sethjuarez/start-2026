Now let's look at the application we've built and published. This is where everything we've been working on comes together.

Here we're looking at our invoices. The agents have already analyzed each one and categorized them based on the evidence they found.

Let's start with an invoice that was approved.

At a glance, we can see the agent's decision, the confidence behind it, and, most importantly, the evidence that supports that decision. We can drill into the supporting documents, review the evidence trai€l, and even see every tool the agent used to reach its conclusion.

That evidence trail is really the key. Instead of asking us to simply trust the AI, the application shows exactly *why* it believes this invoice should be paid.

Now let's compare that to a recovery recommendation.

Here, the agent determined the invoice shouldn't be paid as submitted. Once again, we can inspect the supporting documents, review the evidence that led to the recommendation, and follow the complete reasoning behind the decision.

One capability I particularly like is that we aren't limited to a single agent run. As we're experimenting with different models or prompts, we can compare multiple runs side by side to understand how different approaches affect the outcome.

In this case, the application has even generated a reviewer draft that helps prepare a response for disputing the invoice, giving the reviewer a strong starting point instead of beginning from scratch.

Now let's switch over to the run history.

Here we can see every execution across the system. We can filter by date range, decision type, confidence level, or even sort by the amount of money at risk to quickly identify the highest priority cases.

If we open one of these runs, we get a complete view of how that decision was made.

In this example, the invoice represents $920 of potential risk. We can see each service involved in the workflow, including FoundryIQ and FabricIQ, along with an aggregator agent that combines those results into a single recommendation that our Waypoint application ultimately presents to the reviewer.

Because every step is captured, the entire process is fully traceable from the original documents all the way to the final recommendation.

We also have operational telemetry built into the application.

On the right, we can monitor expert and tool usage, understand which capabilities are contributing the most value, and even measure how much money each one has helped recover. We can also track trends over time, such as whether overall financial risk is increasing or decreasing.

What I like about this entire workflow is how naturally it evolves.

We started with an idea running locally in the GitHub Copilot app. We refined it inside Visual Studio Code, published the agents into Foundry, connected them through Teams, and ultimately delivered a web application that anyone in the organization can use.

The same idea that started as a local proof of concept is now a production-ready workflow that provides transparency, governance, and measurable business value.