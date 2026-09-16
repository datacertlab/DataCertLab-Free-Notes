# Claude Certified Developer – Foundations (CCDV-F)

This is the exam, what it measures, and how to sit it. Everything below is taken from the official
Claude Certified Developer – Foundations Exam Guide, version 1.0, effective July 2026, read on
3 September 2026, plus a measurement of every sample item Anthropic has published for this
certification programme.

Read this page once before you plan your study, and once more the week you book.

## How to read this page

Four different kinds of statement appear below, and they are not equally certain. Each is labelled
where it could otherwise blur:

| Label | What it means |
|---|---|
| **Stated** | Written in the exam guide or in Anthropic's certification administration material |
| **Measured** | Counted from the sample items Anthropic has published. True of those samples, not a guarantee about your form |
| **Judgement** | Study advice derived from the two above. Ours, and argued rather than asserted |
| **Moved since** | Product behaviour that has changed since the guide took effect. Never the exam answer |

Where this page conflicts with the current exam guide, treat the exam guide as authoritative and
regard this page as needing correction. Where the guide and Anthropic's current documentation
disagree, the guide still decides the exam answer — that gap has its own section below.

---

## The exam at a glance

| | |
|---|---|
| Credential | Claude Certified Developer – Foundations |
| Exam code | CCDV-F |
| Items | 53 |
| Time limit | 120 minutes |
| Formats | Multiple-choice and multiple-response; each item states how many responses to select |
| Delivery | Proctored, online or at a Pearson VUE test centre |
| Scoring | Scaled score, 100–1,000 |
| Pass mark | 720 |
| Fee | $125 USD |
| Prerequisites | None. The recommended experience is recommended, not required |
| Who may register | Claude Partner Network organisations only, from a recognised company email domain. Minimum age 18 |
| Validity | 12 months |

Three things in that table are misread more often than the rest.

**Check that you can actually book this exam before you study for it.** Prerequisites and access are
different questions, and only the first is answered in the exam guide. The guide is accurate on its
own question: there is no course you must complete and no qualification you must hold. Access is
answered somewhere else. The Anthropic Partner Academy's certifications FAQ has a section headed
*Eligibility and access*, and it is unambiguous. Do you need to work at a partner organisation to
take an exam? Yes: certification is available to people at Claude Partner Network organisations.
Registration needs a partner email address on a recognised company domain, and a personal address
will not work. Can customers or non-partners get certified? Not currently — the FAQ says
certification is available only to organisations in the Claude Partner Network. There is also a
minimum age of 18, verified against your ID at check-in. Pearson VUE's programme page agrees that
certification is open to organisations in the network.

**That paragraph is the one on this page most likely to go out of date, so check it yourself.** It
was read on 3 September 2026, on the Partner Academy's own certifications FAQ and on Pearson VUE's
Anthropic programme page — both public, both linked from the certification page you would book from.
Access rules are programme policy rather than exam content, and Anthropic can change them without
touching a single objective. If you are not already inside a partner organisation, confirm the
current position before you plan any study around this exam.

**720 is not a percentage.** It is a scaled score on a 100–1,000 range, set by a standard-setting
study in which subject-matter experts judged what a minimally qualified candidate should be able to
do. There is no published mapping from scaled points to questions answered correctly, so anyone who
tells you the pass mark is a particular share of the exam is guessing. Study to the blueprint, not
to a percentage.

**Scoring is compensatory.** Your result comes from your total scaled score alone. The report shows
percent-correct by domain, but those per-domain figures are for your information and are not used to
decide pass or fail — there is no per-domain minimum you can fail on. A weak area can be carried by
a strong one, which changes how you should allocate the last week of study.

---

## What is new in version 1.0, and where the guide has already moved

Version 1.0 is the first edition of this guide, so there is no earlier version for older study
material to be stranded on. There are three gaps worth knowing anyway, and all three catch people.

**The blueprint has two levels, and most material only reads the first.** The guide publishes eight
domains *and* twenty-five individually weighted skills beneath them. The skill weights are the real
study map, and they do not follow the domain names — see the next section, which is the most useful
part of this page.

**The model lineup has moved, and so has one of the thinking modes.** The guide names the tiers as
Opus, Sonnet and Haiku, and the model options as fast mode, extended thinking, adaptive thinking and
effort levels. Two things have changed underneath that, and the second one will bite you at the
keyboard rather than in revision.

*Moved since — the count.* Anthropic's models overview page listed four current models on
3 September 2026, against the guide's three tiers. Anthropic does not present them as a ranking: its
own advice is to start with Opus for most workloads and reach for the fourth model when a task needs
demanding reasoning or runs long. So the honest statement is that there is one more model than the
guide names, not that there is a tier above Opus.

*Moved since — how you ask Claude to think.* The guide names both extended thinking and adaptive
thinking. The balance between them has shifted since. Current models lean on adaptive thinking
steered by an effort setting, and the older mode where you set a thinking budget by hand is being
wound down. Anthropic's models overview described that mode as deprecated on the 4.6 generation and
not accepted on later models when we read it on 3 September 2026.

Which models still take it will have moved again by the time you read this, so check Anthropic's
current thinking documentation for whatever model you are using. What will not have moved is the
shape of the problem. The guide names a mode you may not be able to switch on while practising, and
it is examinable anyway.

**Neither of these changes the exam answer.** The exam is written against the objectives in this
guide. Answer from the lineup and the modes the guide names. Treat anything introduced or retired
after July 2026 as background — worth knowing as an engineer, and not an option you are being asked
to choose. A candidate who "corrects" for the newer product will mark a right option wrong.

**One product in scope has already been renamed.** The guide says Claude Agent SDK throughout. It
was previously called the Claude Code SDK, and documentation still exists under both names. If your
study material says Claude Code SDK, it predates the rename; the capability is the same one.

---

## Where the marks actually are

The eight domains, in the guide's own order:

| Domain | Weight | What it rewards |
|---|---|---|
| D1 Agents and Workflows | 14.7% | Choosing between a workflow and an agent, and knowing what makes an agent reliable |
| D2 Applications and Integration | 33.1% | Ordinary software engineering, done around a model |
| D3 Claude Code | 3.1% | Knowing where configuration lives and what each surface does |
| D4 Eval, Testing, and Debugging | 2.6% | Localising a failure before changing anything |
| D5 Model Selection and Optimization | 16.8% | Tokens, tiers, thinking, caching, and what each costs |
| D6 Prompt and Context Engineering | 11% | Controlling behaviour without enlarging the prompt |
| D7 Security and Safety | 8.1% | Separating untrusted input from trusted instructions |
| D8 Tools and MCPs | 10.6% | Deciding where a capability should live |

**These weights are approximate, and the guide says so.** It describes them as the approximate
proportion of scored items drawn from each domain. Use them to divide your study time, not to
predict your paper: multiplying a weight by 53 gives a planning figure, and nothing commits Anthropic
to that exact count on the form you sit. A domain worth a couple of percent may hand you two items
or none.

**Domain names mislead here, and the twenty-five skill weights fix that.** Claude Code is the most
famous thing in the syllabus and it is one skill worth 3.1%. Applications and Integration sounds
like preamble and is a third of the exam. Study against this table, sorted heaviest first:

| Skill | Domain | Share |
|---|---|---|
| Claude Application Design | D2 Applications and Integration | 8.6% |
| Software Engineering Foundations | D2 Applications and Integration | 7.4% |
| Claude API Mechanics | D2 Applications and Integration | 6.8% |
| Technical Fundamentals | D5 Model Selection and Optimization | 6.1% |
| Agent Construction with Claude | D1 Agents and Workflows | 5.3% |
| LLM Fundamentals | D5 Model Selection and Optimization | 5.2% |
| Agent Patterns and Frameworks | D1 Agents and Workflows | 4.9% |
| Prompt Engineering | D6 Prompt and Context Engineering | 4.6% |
| Agent Architecture | D1 Agents and Workflows | 4.5% |
| Tool Implementation | D8 Tools and MCPs | 4.4% |
| Configuration Management | D2 Applications and Integration | 4.1% |
| Agentic Customization | D8 Tools and MCPs | 4.1% |
| Context Engineering | D6 Prompt and Context Engineering | 3.8% |
| Understanding Requirements | D2 Applications and Integration | 3.4% |
| AI Application Security | D7 Security and Safety | 3.2% |
| Claude Code Operation | D3 Claude Code | 3.1% |
| Systems Life Cycle | D2 Applications and Integration | 2.8% |
| Cost and Token Management | D5 Model Selection and Optimization | 2.8% |
| Model Selection and Tradeoffs | D5 Model Selection and Optimization | 2.7% |
| Debugging and Error Handling | D4 Eval, Testing, and Debugging | 2.6% |
| Output Handling | D6 Prompt and Context Engineering | 2.6% |
| Guardrails and Safe Deployment | D7 Security and Safety | 2.3% |
| MCP Server Development | D8 Tools and MCPs | 2.1% |
| Identity, Secrets, and Key Management | D7 Security and Safety | 1.6% |
| Claude Hooks | D7 Security and Safety | 1.0% |

Three readings of that table are worth making explicit.

**The heaviest single skill is design, not API knowledge.** Claude Application Design at 8.6% is
about how Claude interprets instructions across interfaces, where content boundaries sit, how
schemas are shaped, and session hygiene. It is judgement, and it is the skill most people assume
they already have.

**The second heaviest skill is not about Claude at all.** Software Engineering Foundations at 7.4%
covers REST APIs, JSON, asynchronous programming, version control, code review and refactoring.
Reading it as a prerequisite rather than as content is the most expensive misreading available on
this exam.

**Small skills are cheap marks, and they cluster.** Security and Safety is 8.1% spread over four
skills, none of them above 3.2%. Each one looks skippable on its own, and together they outweigh
Domains 3 and 4 combined. The same is true of the smallest skills generally: they are narrow enough
to learn in an evening, and every item is worth the same as every other regardless of which skill it
came from.

---

## What the questions look like

Anthropic publishes three sample items for this exam and twelve for the sibling architect exam. We
counted every feature below across all fifteen, and they are consistent enough to describe as a
house style.

**Read this section as Measured, not as Stated.** Fifteen items is the entire published set, and it
is still fifteen items. Anthropic describes them as illustrating the style and cognitive level of
the exam, which is a strong signal and not a specification. Everything here tells you what to
prepare for; none of it is a promise about the form you sit.

**All fifteen published items are scenarios.** Two or three sentences set up a situation, then one
question closes it. Not one is a "which of the following statements is true". You are being asked to
choose an approach for a situation that has already been described.

**Four options in every published item, and every wrong one is a real technique.** The distractors
are things a competent engineer might actually propose. The published explanations reject them with
phrases like "over-engineered" and "solves a different problem entirely" — rarely because they are
false. If you take one thing from this page into the exam, take this.

**A multiple-choice item wants exactly 1 answer. A multiple-response item wants 2 or more, and the
item tells you how many.** That much is stated in the guide. Every published sample is
single-answer, so you will meet the multiple-response format for the first time in the exam itself;
read the instruction line before the options. The guide does not say whether multiple-response items
carry partial credit, so assume they do not and treat every response you select as load-bearing.

**No code appears in any published item.** Across all fifteen there is not one code block, request
body or log excerpt. Identifiers appear inline in ordinary prose instead — parameter names, file
paths, tool names, API names. Prepare to recognise them by name. Prepare for a listing anyway if you
have the time, because fifteen items cannot rule one out.

**The decisive word is never shouted in a published item.** They write "best fits" and "most
effective" in ordinary lower case. If your practice material capitalises BEST or LEAST, it has
borrowed a convention from a different vendor's exams.

**No published item uses an "all of the above" option or a negative stem.** None asks which option
would *not* work. Read the closing line of each stem anyway.

### The four questions to ask on every item

This is the reading procedure the published explanations reward, in order:

1. **What did the stem say is the primary concern?** It is usually stated outright, and it is often
   a business fact rather than a technical one — a deadline, a cost ceiling, a reuse requirement.
2. **Which options do not touch that concern?** Expect at least one option that is a genuinely good
   practice aimed at a different problem. Eliminate it without arguing with it.
3. **Of what is left, which is the smallest thing that fixes the cause?** When the stem says "first
   step", an option that requires new infrastructure is wrong even when it would work.
4. **Does any option overstate what a mechanism can reach?** The falsehood usually hides in a
   trailing clause that justifies the option, not in its main verb.

> **Trap.** A recurring distractor pattern in the published samples is "instruct the model to do it
> properly" offered against a problem the stem has already shown the model gets wrong some of the
> time. If a requirement is absolute — money moves, data leaves, a step must never be skipped — a
> prompt cannot enforce it and a programmatic control can. Reach for the deterministic option.

---

## Timing and pacing

53 items in 120 minutes is a little over two minutes each. **Judgement: the clock is unlikely to be
your binding constraint, and careful reading is worth more than speed.** Two things point that way.
The published items are short — the stems run to a few sentences and the options to a line or two —
so there is little to physically get through. And what separates the right option from the plausible
one is a distinction you either see or do not; re-reading helps, and hurrying does not.

One candidate report agrees, and one report is not a distribution: in a published first-hand account
of all four Claude certifications, Matthew Purcell describes finishing this one in 45 of the 120
minutes with the highest of his four scores. Take it as a hint that the margin exists, not as a
target. Plan for the full 120 minutes and spend whatever you save on the flagged items.

A workable plan:

- **First pass, roughly a minute an item.** Answer everything you know. Flag anything where you are
  choosing between two options you can both defend.
- **Second pass on the flags.** Run the four questions above in order. Most flagged items resolve at
  step 2 or step 3.
- **Never leave an item blank.** The guide states no penalty for a wrong answer, so an unanswered
  item can only cost you. Guess anything still open with five minutes left.

---

## How to study

**Start in weight order, not in guide order.** The guide numbers its domains for its own reasons.
Your first three sessions belong to Claude Application Design, Software Engineering Foundations and
Claude API Mechanics, which together are close to a quarter of the exam.

**Start there; do not stop there.** Weight order tells you what to open first, not what to skip. The
small skills are narrow enough to learn in an evening each, and an item drawn from a 1.0% skill is
worth exactly as much as one drawn from an 8.6% skill. Front-load the heavy skills, then sweep the
light ones — that order costs nothing and the reverse order leaves free marks on the table.

**Build one application, and make it exercise the syllabus.** The guide's own preparation advice is
to build and operate at least one Claude application that exercises the API, integrates one or more
tools, applies basic prompt and context engineering, and includes simple security and evaluation
practices. That single project covers more of this blueprint than any amount of reading.

A checklist that maps onto the heavy skills:

- Make a synchronous request and a batch request, and be able to say in one sentence which situation
  each is for.
- Define a tool, then expose the same capability as an MCP server, and be able to say why you would
  choose one over the other.
- Write a project instruction file and a settings file, and know which one every teammate gets when
  they clone the repository and which one stays on your machine.
- Add a hook that blocks an action, so you have felt the difference between instructing the model
  and constraining it.
- Feed the application untrusted text that contains an instruction, and watch what your trust
  boundary does about it.
- Read a trace of a failed run and decide whether the fault is in your integration or in the model's
  output, before changing anything.
- Turn on prompt caching for a system prompt you send on every request, and look at the token
  counts before and after.

**In the last week, revisit the skills you have never used at work.** For most candidates that is
some combination of hooks, MCP server authoring, batch processing and evals. Each is small, each is
concrete, and each is worth about as much per item as the parts you already know.

---

## Booking, scoring and renewal

**Everything in this section can change without the blueprint changing, so check it the week you
book.** Fees, access rules, scheduling mechanics, retake intervals and renewal terms are run by the
certification programme rather than set by the exam guide, and they move on their own schedule. The
figures here were read on 3 September 2026.

Registration goes through the Anthropic Partner Academy, and the exam is delivered by Pearson VUE,
online-proctored or at a test centre. Access is the step people miss: the Partner Academy states
that certification is available only to organisations in the Claude Partner Network, so you need a
company email on a domain recognised on your organisation's partner record. You must also be at
least 18, which is checked against your ID at the door. Bring a valid government-issued photo ID
whose name matches your registration exactly.

**The two official sources disagree about the reschedule window, so plan on the longer one.** The
exam guide says you may cancel or reschedule up to 24 hours before your appointment. Pearson VUE's
Anthropic page says test centre appointments can be rescheduled or cancelled up to 48 hours before,
through your Pearson account. Both were read on 3 September 2026. Pearson VUE runs the scheduling,
and the tighter reading costs you nothing, so treat 48 hours as your deadline and check your own
booking confirmation, which is the only source that describes your actual appointment. Changes
inside the window forfeit the fee.

Results are reported as pass or fail with your scaled score, plus percent-correct by domain. If you
do not pass, the waiting period is 14 days after a first attempt, 30 days after a second and 90 days
after a third, with up to four attempts in a rolling twelve-month period. The fee applies each time.

The credential lasts 12 months. Renewing on time is a free, non-proctored assessment on the Partner
Academy; letting it lapse means sitting the full exam again at full price. The short validity is
deliberate — the guide says the credential is time-limited because the underlying technology moves
quickly, which is the same reason the model-lineup note above exists.

---

## Where these figures come from

Every number and quotation on this page is checkable. The blueprint, the counts, the scoring rules
and the policies all come from the Claude Certified Developer – Foundations Exam Guide, version 1.0,
effective July 2026, which you download from your certification page on the Anthropic Partner
Academy. Read it yourself before you book; it is short.

The question-style section was measured from the sample items in that guide and in the Claude
Certified Architect – Foundations guide. The access rules come from the Partner Academy's
certifications FAQ and from Pearson VUE's Anthropic programme page. Both "moved since" notes come
from Anthropic's current developer documentation. The models overview page carries the lineup and
the thinking modes; the Agent SDK migration guide carries the rename, and states in its own words
that the Claude Code SDK has been renamed to the Claude Agent SDK.

All of it was read on 3 September 2026. Where this page conflicts with the current exam guide, treat
the exam guide as authoritative and regard this page as needing correction.
