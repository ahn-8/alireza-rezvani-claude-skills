# Nodal Cold Email Series — B2B SaaS & B2C ($5M–$100M+ ARR)

**Brand:** Nodal (nodal.cx) — marketing operations and data enablement consultancy
**Target:** VP/Head of Marketing, Growth, RevOps, or Marketing Ops at B2B SaaS companies ($5M–$100M+ ARR) or B2C businesses running multiple martech platforms
**Built with:** `marketing-skill/skills/cold-email` — frameworks (`references/frameworks.md`), follow-up cadence and angle rotation (`references/follow-up-playbook.md`), deliverability guidance (`references/deliverability-guide.md`), voice-calibration table (VP/Director tier: 5–7 sentences, direct, metrics-conscious), scored with `scripts/email_sequence_analyzer.py` before delivery.
**Cadence:** Day 1 → Day 4 → Day 9 → Day 16 → Day 25 → Day 35 (the skill's standard 6-touch cadence, gaps increasing over time)
**Voice:** Succinct, confident, warm, methodologically precise. No false urgency. (Nodal brand voice)

---

## Email 1 — First Touch (Day 1)

**Framework:** Observation → Problem → Proof → Ask (OPPA)
**Subject line:** your data stack

**Body:**

{{First name}},

Most marketing teams now run more platforms than any one person can keep straight — CRM, enrichment, attribution, automation — and the data between them rarely reconciles cleanly.

That gap stays invisible until you try to trust a report or act on a lead score, and then it gets expensive.

We're Nodal, a marketing operations and data enablement consultancy. We build the integrations, CRM architecture, and tracking models that make the platforms you already pay for actually usable, without the overhead of a full agency engagement.

On a recent project, backtesting an existing lead-scoring model against closed revenue found the top-tier segment worth 30% more than random triage — same CRM, same leads, just an accurate model.

Worth a 20-minute call to see where your setup stands?

Shelby Ahern
Nodal
nodal.cx

---

## Email 2 — New Angle (Day 4)

**Framework:** Question → Value → Ask (QVA)
**Subject line:** your lead scoring

**Body:**

{{First name}},

Quick question: when was your lead-scoring model last checked against what actually closed?

Most aren't. We see it constantly — a model built once, personas never folded in, scores that quietly drift from reality. On one engagement, adding persona data to an existing model took its correlation with closed revenue from noise to 1.8x, using the same leads and the same CRM.

That's a data architecture fix, not a rebuild. We map what's actually flowing between your CRM and enrichment sources before touching the scoring logic, and we backtest every change against revenue before you commit to it.

If your model hasn't been checked this year, that's usually the first place worth looking.

Worth 15 minutes to walk through what that check looks like?

Shelby Ahern
Nodal
nodal.cx

---

## Email 3 — Value Add (Day 9)

**Framework:** lead with a benchmark before asking again (per the skill's "give something useful" rule — never "just checking in")
**Subject line:** a quick benchmark

**Body:**

{{First name}},

Sharing something useful rather than asking again.

On a recent SMS integration project, we rebuilt the data flow between the CRM and the messaging platform — no new campaign, just cleaner state tracking on who'd already been contacted. Connection rate lifted 60% and revenue per message rose 67%, from the data fix alone.

The pattern shows up often: the growth lever everyone's chasing is really a data-plumbing problem wearing a campaign costume.

Want the fuller breakdown, or a quick look at where a similar gap might be sitting in your own stack?

Shelby Ahern
Nodal
nodal.cx

---

## Email 4 — Direct Question (Day 16)

**Framework:** plain, standalone question — no setup, no callback to prior emails
**Subject line:** quick question

**Body:**

{{First name}},

Plain question: can your team trust the numbers in your marketing reporting today, or is there manual reconciliation happening behind the scenes to make it presentable?

If it's the latter, that's exactly what we fix — cleanly, without a rebuild.

Worth 15 minutes to compare notes?

Shelby Ahern
Nodal
nodal.cx

---

## Email 5 — Reverse (Day 25)

**Framework:** ask for a referral to the right person if this contact isn't the owner
**Subject line:** right contact

**Body:**

{{First name}},

If marketing data infrastructure — CRM configuration, lead scoring, tracking architecture — isn't something you own directly, is there someone on your team who does?

A name would help me stop guessing and start being useful to the right person.

If it is you, no worries at all — happy to pick this back up whenever the timing works.

Worth a quick reply either way?

Shelby Ahern
Nodal
nodal.cx

---

## Email 6 — Breakup (Day 35)

**Framework:** close the loop professionally; signal this is the last one
**Subject line:** last note

**Body:**

{{First name}},

I'll stop cluttering your inbox after this one.

I've sent a few notes about how Nodal fixes the data architecture underneath a marketing stack — CRM configuration, lead scoring backtested against revenue, tracking models that hold up under reporting. If any of that becomes a priority later, happy to reconnect — just reply here and I'll pick it up.

If there's someone else at your company worth looping in, a name goes a long way.

Worth a reply either way?

Shelby Ahern
Nodal
nodal.cx (hello@nodal.cx)

---

## Quality Check (`scripts/email_sequence_analyzer.py`)

Per the `cold-email` skill's own instruction ("Run it on every drafted sequence before delivering: any email scoring below 70 gets rewritten"), this sequence was scored before delivery:

| Email | Subject | Word count | CTA | Personalization | Score |
|---|---|---|---|---|---|
| 1 — First Touch | your data stack | 127 | ✅ clear | 3.9% | 93/100 🟢 |
| 2 — New Angle | your lead scoring | 124 | ✅ clear | 3.2% | 93/100 🟢 |
| 3 — Value Add | a quick benchmark | 92 | ✅ clear | 4.3% | 93/100 🟢 |
| 4 — Direct Question | quick question | 46 | ✅ clear | 8.7% | 100/100 🟢 |
| 5 — Reverse | right contact | 65 | ✅ clear | 6.2% | 100/100 🟢 |
| 6 — Breakup | last note | 79 | ✅ clear | 5.1% | 100/100 🟢 |

**Sequence overall: 96/100 🟢 Strong.** No email fell below the skill's 70-point rewrite threshold; no spam-trigger words, dead openers, or weak CTAs detected in any email. Emails 1–3 came in slightly under the skill's 5% personalization-density guideline (3.2–4.3%) — acceptable given this is unsegmented template copy rather than a 1:1 personalized send; see personalization guidance below for what to add per-send.

---

## Series Notes

**Personalization guidance:**
- Research the prospect's martech stack before sending — if you can identify their CRM (HubSpot vs. Salesforce), enrichment tools, or attribution setup, reference it directly in Email 1 or 2. It signals you understand their actual infrastructure, not a generic pitch, and lifts the personalization density the analyzer flagged as merely adequate.
- Where possible, reference a specific gap visible from the outside (e.g., inconsistent UTM tagging, a lead form that doesn't route to their CRM cleanly) — adds specificity and shows homework.

**Opt-out / compliance** (per `references/deliverability-guide.md` → Legal Requirements):
- CAN-SPAM (USA): honest subject line, physical mailing address, working unsubscribe mechanism — non-negotiable on every email.
- GDPR (EU/EEA): legitimate-interest basis required; no soft opt-in.
- CASL (Canada) / PECR (UK): stricter consent requirements — confirm applicability before sending into those markets.

**A/B testing candidates:**
- Email 1 subject: test "your data stack" vs. "quick question" (per skill guidance: shorter, more internal-looking subjects tend to win on B2B).
- Email 6 subject: test "last note" vs. "closing the loop."
- Email 1 CTA: test "20-minute call" vs. "quick diagnostic" framing.

**Sending infrastructure** (per `references/deliverability-guide.md` → Domain Setup, Domain Warmup, Sending Limits by Platform):
- Use a dedicated sending subdomain (e.g., `outreach.nodal.cx`), never the primary domain — protects `nodal.cx`'s core email reputation if the outreach domain gets flagged.
- Confirm SPF, DKIM, and DMARC are all passing before the first send (verify with mail-tester.com; target 9/10 or higher).
- 5-week warmup ramp: Week 1 at 5–10 emails/day (real conversations only), Week 2 at 20–30, Week 3 at 40–60 (watch for >30% open rate), Week 4 at 80–100, Week 5+ up to 200/day with daily monitoring.
- Plain text only — no HTML template, no logo, no embedded images. Cold email with heavy HTML both scores worse on deliverability and reads as a marketing blast rather than a person.
- Keep bounce rate under 2% (5%+ is dangerous) — verify the list before the first send; never buy a list.
