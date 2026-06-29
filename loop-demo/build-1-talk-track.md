Let's take a look at the GitHub Copilot app. This is where I can work with Copilot without juggling multiple CLI sessions or SDKs. If I decide to go deeper, I can hand any of these sessions directly into VS Code and continue developing there.

Everything starts from the home screen. I get a high level view of everything I'm working on, including active work, open issues, pending reviews, and any automations I've configured. It's essentially my Copilot command center, and it's where I start every morning.

Let me show you how I kicked off a proof of concept for our internal project, Pharma Shield.

All I need to do is enter a prompt: *Start the contract reconciliation proof of concept.* From there, the Copilot app takes care of the setup.

The first thing you'll see is that it creates a worktree. If you're familiar with Git, a worktree gives me an isolated workspace so I can experiment freely without affecting my main branch or anyone else's work.

Next, it loads a custom skill I created specifically for this contract reconciliation scenario. That skill captures the domain knowledge and workflow so every session starts with the same context instead of me rebuilding it each time.

Before anything runs, the app performs a quick preflight check of the local language model using Ollama.

That's important because there are plenty of situations where I don't want to rely on cloud connectivity. Maybe I'm on an airplane, working from a coffee shop, or handling sensitive customer data. Running locally gives me lower latency, lets me work offline, and helps ensure that my data never leaves the device during development and testing.

Once everything is ready, here's the application.

On the left is the Copilot session that's driving the work. On the right is the Canvas, which gives me an interactive view of the application I'm building and testing.

Right now I'm using my local model, although I can switch to a cloud model at any time.

Let's start with a simple question about one of these invoices.

As soon as I submit the prompt, notice the live network monitor. Every request is staying on the local machine. The model is running entirely on device, and there's no outbound traffic. That gives me confidence that sensitive information isn't crossing any network boundary while I'm experimenting.

From there, I can continue working through the proof of concept. I can review flagged invoices, inspect the evidence trail behind each recommendation, approve recoveries, place items on hold, or escalate them for governance review.

Now let's compare that to using a cloud model.

I'll switch models, reload the Canvas, and run the exact same prompt.

This time, the network monitor tells a very different story. We can see traffic leaving the device, along with exactly which model was used, how many documents were sent, and how much data crossed the boundary. That visibility makes it much easier to understand and audit what information is leaving the local environment.

One final capability I want to highlight is sandboxing.

Everything in this proof of concept is running inside an isolated execution environment called Microsoft MXC. To demonstrate why that matters, let's simulate a poisoned invoice containing a prompt injection attack that tries to access proprietary data, like a master batch record.

With the MXC sandbox enabled, the attack is blocked. The Canvas explains exactly what happened. Outbound network access is denied, file access is restricted, and the malicious prompt never reaches sensitive data.

Now let's disable the sandbox and run the same attack again.

This time, the trade secret is successfully exfiltrated. The Canvas immediately identifies what happened, explains the impact, and the Copilot app automatically creates a GitHub issue documenting the incident.

I can open that issue immediately, assign it to the right engineer, or begin remediation myself. Instead of just detecting the problem, the workflow moves directly into action.

At this point, we've proven that our idea works. The next step is scaling it beyond a local proof of concept so the rest of the team can use it. That's where cloud infrastructure comes in.

In the next demo, we'll take this same application and move it into Microsoft Foundry.