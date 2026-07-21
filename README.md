# slf-1537 — MoneyPark MPRE Owner Activation Agent (microsite demo)

Single-file GitHub Pages prototype: an **inbound microsite** that embeds the ElevenLabs **MoneyPark Owner Activation** agent, in the same spirit and flow as the MoneyPark refinance microsite.

- **Live page:** https://charlesalzon-alt.github.io/slf-1537/
- **Agent (ElevenLabs, EU residency):** `agent_1101kw9w2jhjfk6tseg7hyqv997v`
- **Prompt source of truth:** `tries/MONEYPARK - FINOVO/onboarding agent/prompts/owner/` in the Solution Factory workspace (inbound microsite version).

## What it is

The activation flow modelled on the refinance one, to minimise legal friction: a MoneyPark automation emails the owner, the owner clicks through to this landing page (microsite), and chats with Anna. Anna delivers a fresh property estimate, captures a satisfaction signal (CSAT), and drives the owner to activate their MPRE cockpit by sending the one-tap login link by SMS. No outbound call: the owner opts in by starting the conversation here.

The widget is preloaded with a sample German owner profile (Herr Thomas Müller) so the conversation feels real.

## Architecture

Single `index.html`, no build step. The only external dependency is the ElevenLabs Convai widget embed. No secrets are stored client-side.

## Editing

Edit the canonical copy in the workspace (`tries/MONEYPARK - FINOVO/onboarding agent/owner-widget/index.html`), then copy to a temp clone of this repo and push.
