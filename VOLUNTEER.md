# The Museum of AI Safety is looking for volunteers

*Epistemic status: an early, rough project I've been building on and off. Posting to
get feedback and find people who'd like to help. Not sure yet how useful it is, and I'd
like to find out.*

I've been building **The Museum of AI Safety** — a first-person, walkable museum about
AI safety that runs as a single HTML file in the browser. No install, no account, no
network calls; you open it and walk around. There are currently 35 exhibits across
several halls (adversarial examples, jailbreaks, reward hacking, interpretability,
governance, AGI timelines, and the history from Wiener and Turing forward), plus a gift
shop that links out to the real on-ramps into the field (BlueDot, AISafety.info, Apart,
AI Safety Camp, 80,000 Hours, MATS, and others).

Repo: https://github.com/varchanaiyer/ai-safety-museum — open it in a browser, or run
`python3 -m http.server` and visit the page.

## Why it exists

Most good introductions to AI safety are text: reading lists, courses, wikis. Those are
the right tool for people who already want to sit down and study. I wanted to try a
lower-friction, more visual on-ramp — something you can wander through in a few minutes
that leaves you with the shape of the problem and a clear next step, and that points at
the existing communities rather than trying to replace them. Whether that actually works
on anyone is an open question. That's part of what I'm hoping to learn here.

## What works now, and what's rough

Honest state of the thing:

- **Works:** the raycasting engine, 35 exhibits with placard text, floor plan and
  wayfinding, the gift-shop links, progress saved in `localStorage`, resolution that
  auto-tunes for frame rate.
- **Rough / unfinished:** accessibility is thin (no screen-reader path, motion can't be
  reduced, colour contrast is untested). Mobile controls work but are fiddly. The exhibit
  text is my own summarising and has not been reviewed by anyone who works in these areas,
  so some of it is likely imprecise or out of date. It's English-only. Everything lives in
  one 1,800-line `index.html`, which is either charming or a liability depending on your
  taste.

I'd rather name these up front than have you find them.

## Where you could help

Any level of involvement is genuinely useful — a two-minute bug report is worth having.
Roughly from least to most time:

- **~2 min — try it and tell me what breaks.** Which browser/device, what went wrong.
  Open a GitHub issue or just leave a comment.
- **~15 min — walk through and note what's confusing or wrong.** Places where the framing
  is off, an exhibit doesn't land, or the path through the building doesn't make sense.
- **~1 hour — fact-check or improve an exhibit.** If you know a topic (interpretability,
  RLHF, evals, governance, timelines) well, tell me where a placard is imprecise, or draft
  a better version. Corrections from people closer to the work than I am are the single
  most valuable thing here.
- **Ongoing, if it suits you:**
  - *Developers* — accessibility is the biggest gap: a keyboard/screen-reader-navigable
    text mode, a reduced-motion option, contrast fixes. Also mobile controls and
    performance on low-end devices. It's plain HTML/Canvas/JS, no build step, no framework.
  - *Designers / writers* — exhibit copy, the visual language of the placards, the
    wayfinding.
  - *Translators* — it's English-only; the text is separable from the engine.
  - *Anyone* — suggest an exhibit that's missing, or a link the gift shop should carry.

If dev work appeals, I'll tag some starter issues as `good-first-issue`. If you'd like to
pick something up, comment on the issue so we don't collide.

## A request, not a pitch

Feedback is welcome, including the case that this shouldn't exist or that a museum is the
wrong shape for this — I'd genuinely rather hear that now than later. The goal is a small,
accurate, welcoming thing that sends people onward to the groups already doing the work,
not a destination in itself. If it's not serving that, tell me.

Best ways to reach me: open an issue or PR on the repo, or reply here. Thanks for reading,
and thanks to everyone whose writing the exhibits are built on.
