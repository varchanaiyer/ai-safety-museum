# The Museum of AI Safety is looking for volunteers

*Epistemic status: an early project with a big long-term goal and a small working
prototype. Posting to get feedback and find people who'd like to help build it out. I'm
not certain the in-person vision is the right bet, and I'd like to pressure-test it with
people who know more than I do.*

The goal is a **real, in-person Museum of AI Safety** — a free, public space you can walk
into and leave understanding, roughly, what the field is worried about and how to get
involved. Somewhere between a science-museum exhibit and an art installation: interactive,
honest, welcoming to people who've never heard the phrase "alignment," and pointed firmly
at the groups already doing the work.

**Right now it's virtual.** What exists today is a browser prototype: a first-person,
walkable museum that runs as a single HTML file, with 35 exhibits across several halls
(adversarial examples, jailbreaks, reward hacking, interpretability, governance, AGI
timelines, and the history from Wiener and Turing forward) and a gift shop that links out
to the real on-ramps (BlueDot, AISafety.info, Apart, AI Safety Camp, 80,000 Hours, MATS,
and others). Think of it as a proof of concept and a design sketch for the physical thing
— a way to test what an exhibit should say and how a visitor should move through it,
cheaply, before anyone pours a floor.

Try it: https://github.com/varchanaiyer/ai-safety-museum — open it in a browser, or run
`python3 -m http.server` and visit the page.

## Why in person, and why now

There are excellent text introductions to AI safety — reading lists, courses, wikis — and
they work well for people who already want to study. There's much less for the person who
walks past. A couple of physical AI exhibits exist (the Misalignment Museum in San
Francisco showed that a free, public, slightly funny space about this can draw a real
crowd; several science museums now run general AI shows), but there isn't a permanent,
dedicated place focused on the safety question specifically. The virtual museum is how I'm
testing whether that space is worth building, and what it should contain, before asking
anyone to fund a room.

I could easily be wrong that a museum is the right shape for this. That's one of the things
I'm hoping to find out here.

## What works now, and what's rough

Honest state of the prototype:

- **Works:** the walkable engine, 35 exhibits with placard text, floor plan and wayfinding,
  the gift-shop links, progress saved locally.
- **Rough / unfinished:** accessibility is thin (no screen-reader path, no reduced-motion,
  contrast untested). Mobile controls are fiddly. The exhibit text is my own summarising
  and hasn't been reviewed by anyone who works in these areas, so some of it is likely
  imprecise. It's English-only. And the in-person plan is, so far, just a plan — no venue,
  no budget, no curatorial partner yet.

I'd rather name these than have you find them.

## Where you could help

Any level of involvement is genuinely useful — a two-minute bug report is worth having.
Roughly from least to most time:

- **~2 min — try it and tell me what breaks.** Which browser/device, what went wrong.
- **~15 min — walk through and tell me what's confusing, wrong, or missing.** Especially
  as someone imagining a first-time visitor.
- **~1 hour — fact-check or improve an exhibit.** If you know a topic (interpretability,
  RLHF, evals, governance, timelines) well, tell me where a placard is imprecise or draft a
  better one. Corrections from people closer to the work than I am are the most valuable
  thing here.
- **Ongoing, if it suits you — the digital museum:**
  - *Developers* — accessibility is the biggest gap (keyboard/screen-reader mode,
    reduced-motion, contrast), plus mobile and performance. Plain HTML/Canvas/JS, no build
    step.
  - *Designers / writers* — exhibit copy, the visual language, wayfinding.
  - *Translators* — it's English-only; the text is separable from the engine.
- **Ongoing, if it suits you — the in-person museum** (this is where I most need people who
  know things I don't):
  - *Curators / exhibit designers* — how a physical exhibit teaches one idea well, what to
    cut, how visitors actually move through a room.
  - *Educators / docents* — what a general-public visitor needs, and could-be programming:
    school groups, talks, a walkthrough script.
  - *AI-safety researchers* — a standing "is this accurate?" check on any exhibit that
    would go on a real wall, and a sanity check on the whole premise.
  - *People with museum / gallery / space / partnership experience* — venues, hosting a
    pop-up, what it actually takes to put this in a room, and whether a temporary
    installation is a smarter first step than a permanent one.
  - *Fundraising / operations* — if this becomes real, it needs a sustainable, transparent
    way to run.
  - *Anyone* — suggest an exhibit that's missing, or an org the gift shop should link to.

## A request, not a pitch

Feedback is welcome, including the case that this shouldn't exist, or that a museum is the
wrong shape, or that the effort is better spent on the existing programs the gift shop
already points to. I'd rather hear that now. The aim is a small, accurate, welcoming thing
that sends people onward to the people already doing the work — not a monument, and not a
destination in itself.

Best ways to reach me: open an issue or PR on the repo, or reply here. Thanks for reading,
and thanks to everyone whose writing these exhibits are built on.
