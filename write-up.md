# Design Rationale — Daily Reflection Tree

## What I Was Trying to Build

The brief asked for a wise colleague, not a therapist. That constraint shaped every question. A wise colleague doesn't moralize, doesn't keep score, and doesn't pretend they have the answer. They ask the question that makes you stop and think. That was the target.

---

## Why These Questions

**Axis I — Agency**

The opening "weather report" question is not about locus of control directly — it's a softening entry point. Asking "did you have internal or external locus of control today?" would trigger defensiveness. Asking "what was today like?" is how a real conversation starts.

The branching from "Sunny/Cloudy" vs "Stormy/Foggy" matters: people who had a hard day need a different first question than people who had a good one. Both groups end up examining agency, but from different angles. The "Sunny" path asks *what made it happen* (attribution). The "Stormy" path asks *where did your mind go* (response pattern).

The second question per branch was designed to find the edge of the axis — the moment where the person's habitual response becomes visible. For the "stuck" branch, the question "was there a moment — even a small one — where you had a choice?" is doing something specific: Rotter's research shows that people with external locus don't deny all agency, they just have a *lower threshold* for attributing outcomes to external factors. The question is calibrated to find that threshold, not accuse them of victimhood.

**Axis II — Orientation**

The opening interaction question was the hardest to design. The problem: an entitlement-oriented person will rarely recognize themselves in a question that uses the word "entitlement." The options needed to be honest descriptions of inner states, not labels. "I was thinking about what I would get" is how entitlement actually *feels from the inside* — not "I felt entitled."

The flip question on the entitlement branch ("did someone else give more than they received?") is borrowed from perspective-taking research. It doesn't shame — it redirects attention outward for a moment, which is the psychological move that entitlement makes impossible.

**Axis III — Radius**

The spectrum here runs from "no one came to mind besides me" to "a customer or end user." The options are ordered by radius width, and I deliberately put "A specific colleague" before "The team" — because naming a specific person is a more concrete cognitive act than thinking about an abstraction like "the team." Maslow's self-transcendence is a grand concept; the questions try to find its smallest operational unit.

---

## Branching Trade-offs

The tree makes one significant structural compromise: the bridge nodes auto-advance without confirmation. This means an employee at 11pm sees the transition happen quickly. The alternative — making bridges interactive — slows the conversation without adding information. I chose pace over ceremony.

The decision nodes are hidden from the employee. This was non-negotiable. If someone sees "your answer has been classified as EXTERNAL," the reflection collapses into a performance review. The intelligence is in the structure, invisible to the user.

One deliberate design choice: the reflection nodes on the "external" and "entitlement" paths are *invitations*, not verdicts. "Here's a question to sleep on" versus "you were in the driver's seat today." The asymmetry is intentional — it mirrors how a wise colleague would actually respond to someone having a bad day vs. a good day.

---

## Psychological Sources

- **Rotter (1954)** — Locus of Control. The internal/external branching and the "attribution" framing in Axis I questions comes directly from Rotter's I-E scale design. His key insight: locus of control is a *generalized expectancy*, not a fixed trait — which is why the tree doesn't label anyone permanently.
- **Dweck (2006)** — Growth Mindset. The second-layer questions in Axis I ask about what you *did* rather than who you *are*. "I found a different path" is a behaviorally-framed growth-mindset response, not a personality claim.
- **Campbell et al. (2004)** — Psychological Entitlement Scale. The PES measures entitlement through items about deserving more than others. The Axis II questions translate this into situational language: "did you feel you deserved more credit?"
- **Organ (1988)** — OCB. The Axis II "contribution" branch is grounded in Organ's five OCB dimensions: altruism, conscientiousness, sportsmanship, courtesy, and civic virtue. "I helped with something that wasn't mine to do" = altruism. "I put in extra effort" = conscientiousness.
- **Maslow (1969)** — Self-Transcendence. Maslow's posthumous work argued that healthy humans move through a hierarchy that peaks not at self-actualization but at self-transcendence — orienting toward something beyond the self. The Axis III radius questions operationalize this as concentric circles: self → colleague → team → customer/world.
- **Batson (2011)** — Empathy. The distinction between perspective-*taking* (cognitive) and sympathy (emotional) informed the Axis III questions. The goal isn't to make someone feel bad for a colleague — it's to ask them to *model* the colleague's experience, which is the harder and more durable skill.

---

## What I'd Improve With More Time

1. **Temporal anchoring.** The current tree treats "today" as a uniform unit. A better version would ask "what time of day?" first and anchor the subsequent questions to a specific moment rather than an abstraction.

2. **Streak-awareness.** The tree has no memory. A real deployment would know "this is your 3rd 'stormy' day this week" and adjust the reflection accordingly — not by moralizing, but by making the pattern visible.

3. **The entitlement branch needs more texture.** There are many flavors of entitlement — comparative (I deserve more than others), transactional (I gave X so I should get Y), historical (I've paid my dues). The current tree treats them as one thing. They'd benefit from distinct branches.

4. **Closing ritual.** The "See you tomorrow" end node is abrupt. A better ending would ask one forward-looking micro-commitment — not a goal, but a tiny intention for tomorrow. Something small enough to actually keep.

---

*AI tools used: Claude (claude.ai). Approximate share of task: research framing (~30%), question drafting iteration (~40%), structural review (~20%). All final question text, branching logic, and design rationale written and verified by the author.*
