# Framing all in GitHub Copilot App
I want to talk to an agent to talk  about my contracts / policies. 
Open with the request. All in the GH Copilot App.
One line where we have the copilot app - you may have heard about *the others. They all use the same.... we have collapsed (almost) all of the things into the SDK (and they build on the same thing).

## Definition of Agent
An agent is a combination of:
- a model
- instructions (both context + procedural context)
- harness - runtime that processes model output (sometimes model output suggests a tool call - the harness runs it and puts it back on the thread)

## Part 1 - BUILD
Get it to work
1. Macro
  - home
  - *my work
  - automations
  - chat
2. Micro
  - rubber duck
  - canvas - simple, cheap, agent executes it, gets reponse
  - inter project talking

## Part 2 - DEPLOY
Get it working in Foundry with IQs. Now that I have a local thing working - lets move the _intelligence_ to the cloud (IQs + Agents)
1. Add IQs
2. Test
3. Deploy with IQs (implied Teams deploy as well)
4. Test
5. Deploy to Teams

## Process
1. Build a local agent (local model) with a file inside
2. Build a local agent with (cloud model) an IQ inside + Amanda
3. Move the local agent with both into Foundry