# slf-1537 — MoneyPark MPRE Owner Activation Agent (widget demo)

Single-file GitHub Pages prototype that embeds the ElevenLabs **MoneyPark Owner Activation** voice agent as a click-to-talk widget.

- **Live page:** https://charlesalzon-alt.github.io/slf-1537/
- **Agent (ElevenLabs, EU residency):** `agent_1101kw9w2jhjfk6tseg7hyqv997v`
- **Prompt source of truth:** `tries/MONEYPARK - FINOVO/onboarding agent/prompts/owner/` in the Solution Factory workspace.

## What it is

A hypothesis demo of the outbound Owner-activation agent: deliver a fresh property estimate, capture a satisfaction signal (CSAT), and drive the owner to activate their MPRE cockpit. In production the agent runs as an outbound call; this page exposes it as an inbound widget so stakeholders can experience it in the browser.

The widget is preloaded with a sample German owner profile (Herr Thomas Müller) so the conversation feels real.

## Architecture

Single `index.html`, no build step. The only external dependency is the ElevenLabs Convai widget embed. No secrets are stored client-side.

## Editing

Edit the canonical copy in the workspace (`tries/MONEYPARK - FINOVO/onboarding agent/owner-widget/index.html`), then copy to a temp clone of this repo and push.
