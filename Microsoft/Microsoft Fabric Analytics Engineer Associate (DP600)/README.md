# Exam DP-600 — what you are sitting, and how to sit it

This page is the map. It covers what the exam is made of, what the questions look like on screen,
how the clock works, and how to spend the weeks before it. Everything here tracks the current
edition of the exam, **Skills measured as of July 21, 2026**.

The certification is **Microsoft Certified: Fabric Analytics Engineer Associate**. The exam that
earns it is DP-600, *Implementing Analytics Solutions Using Microsoft Fabric*.

---

## The figures

| Fact | Value |
|---|---|
| Answering time | 100 minutes |
| Seat time | 120 minutes |
| Skill areas | 3 |
| Objectives | 7 groups, 41 bullets |
| Score range | 0 to 1000 |
| Passing score | 700 |
| Scoring model | Scaled |
| Per-domain minimum | None |
| Penalty for a wrong answer | None |
| Open book | Yes, Microsoft Learn |
| Renewal | Annually, free, online |

Two of those need a sentence each.

**700 is a scaled score, not 70% correct.** Microsoft says so plainly: as a scaled score, it "may
not equal 70% of the points". There is no published mapping from answers to the scale. So no
percentage on this course's mock exams converts into a predicted exam score, and anyone who tells
you it does is guessing. Treat the mocks as a readiness signal and nothing finer.

**Scoring is compensatory.** There is one cut score for the whole exam and no minimum score for any
individual skill area. A strong area can carry a weak one. Your score report will break performance
down by area afterwards, but that breakdown is feedback, not a set of separate hurdles.

Microsoft does not publish a question count for DP-600. Its two general statements disagree: one
support page says most exams contain between 40 and 60 questions, and its Director of Psychometrics
says most have between 35 and 50. The only band both agree on is 40 to 50, and treat that as a
planning assumption rather than a specification — the count can vary between sittings.

You do not have to guess on the day. **The welcome screen states the structure of your own sitting**
before you answer anything: the total number of questions, how many are standalone, how many case
studies there are and how many questions each holds, and the same for any labs. Read it. Some
questions are worth more than one point, and when that is true the question says so.

---

## What changed in this version

Two changes matter, and the one that matters most is not the recent one.

The July 2026 edition altered five strings. Two of them change what you are asked. *Choose between a
lakehouse, warehouse, or eventhouse* became **Choose between different data stores** — the objective
no longer names three options, so SQL database in Fabric, mirrored databases and shortcuts are all
in play. And *Direct Lake on SQL endpoints* became **Direct Lake on SQL analytics endpoint**,
singular, matching the product's current name. The other three changes are wording only.

The larger break is older, and most material written about this exam has not caught up with it. In
November 2024 DP-600 went from four skill areas to three, and from 57 measured skills to what is now
41. **PySpark and notebook authoring were removed from DP-600 and moved to DP-700.** *Explore and
analyze data* was folded into *Prepare data*. KQL and Eventhouse were added.

That removal is worth dwelling on, because it is the single most common way current DP-600 study
material is wrong. The words *Spark*, *PySpark*, *Python*, *notebook* and *Eventstream* do not
appear anywhere in the exam's skills-measured list. The query languages in scope are SQL, KQL and
DAX. If a practice question asks you to complete a PySpark snippet, it is testing DP-700.

The flip side is useful. Because those mechanisms are adjacent, plausible and out of scope, they
make excellent wrong answers. Expect to see notebooks and eventstreams offered as options. Knowing
they are not this exam's territory is itself a discriminator.

---

## What is not on this exam

Worth its own list, because this is where most people waste preparation time.

| Topic | Why it is not here |
|---|---|
| PySpark and Python | Moved to DP-700 in November 2024 |
| Notebook authoring | Moved with it |
| Spark pool configuration | Not in the skills-measured list |
| Fabric admin portal and tenant settings | Not in the skills-measured list |
| Shortcuts as an objective | Useful to know, but not a named skill here |

Two cautions about that table. It says these are not *named objectives*, not that they never appear
on screen: Spark and Eventstream are both listed as options in a Fabric ingestion decision guide the
objectives do point at, so recognising them is useful. And the guide itself says related topics may
be covered. The practical rule is that you should not be *studying* these to pass DP-600, and an
option built on one is far more often a distractor than a key.

---

## The three skill areas

Microsoft publishes a range for each area rather than a fixed number, because the count varies
between sittings. Our practice tests allocate a single figure inside each published range so the mock
exams have a fixed shape.

| Skill area | Microsoft's published share | Our practice tests allocate |
|---|---|---|
| Maintain a data analytics solution | 25–30 | 26% |
| Prepare data | 45–50 | 48% |
| Implement and manage semantic models | 25–30 | 26% |

**Prepare data is close to half the exam.** That is the single most useful fact on this page for
planning. It covers getting data in, transforming it, and querying it in four different surfaces:
the Visual Query Editor, SQL, KQL and DAX.

*Maintain a data analytics solution* is security, governance and the development lifecycle —
workspace and item access, row-level and column-level and object-level and file-level security,
sensitivity labels, endorsement, version control, deployment pipelines and the XMLA endpoint.

*Implement and manage semantic models* is modelling and performance — star schemas, relationships,
storage modes, calculation groups, composite models, Direct Lake behaviour, and making DAX fast.

---

## What the questions look like

Microsoft does not publish a format breakdown, but it does publish a sandbox that demonstrates every
format in the real exam interface. Twelve formats were observed there. You will not meet all of them
in one sitting.

| Format | What you do |
|---|---|
| multiple-choice | Pick 1 answer from a list of radio buttons |
| multiple-response | Pick several checkboxes; the stem says how many |
| build-list | Move actions into the answer area in the right order |
| drag-and-drop | Map items onto labelled targets |
| hot-area | Click regions of a screenshot |
| active-screen | Configure a simulated settings dialog |
| active-screen-dropdown | Complete a statement from two or more dropdowns |
| yes-no-statement-grid | Judge several statements Yes or No in one table |
| problem-solution-set | One problem, several proposed solutions, judged one at a time |
| case-study | A scenario document with several questions hanging off it |
| lab | Hands-on tasks in a live environment |
| interlinear-dropdown | Inline blanks, each with its own dropdown |

Six things about that list are worth knowing before exam day.

**A multiple-response stem always tells you how many answers to select.** You never have to guess
whether it wants two or three. The interface also warns you if you try to move on having selected
too few.

**A build-list gives you more actions than slots.** Some of the actions on offer do not belong in the
answer at all. Do not assume you must use every one.

**The problem-solution-set is the format people find most disorienting.** The same scenario appears
several times, each with a different proposed solution, and you answer Yes or No to each. Three
rules govern it. You cannot skip a question in it. You cannot go back to one once answered, and they
never appear on the review screen. And — the part that catches people — more than one solution in a
set may be correct, or none of them may be. Judge each solution on its own merits against the stated
goal. Do not reason that you have already used your one Yes.

**Multi-part questions can give partial credit.** Where a question has several components, Microsoft says you earn a point per
correct component and can score some of the marks without scoring all of them. The exceptions are
the single-answer formats: a multiple-choice question has exactly 1 correct answer and a
problem-solution-set question offers Yes and No. Exact scoring rules are not published per format, so treat partial credit as something multi-part questions may give rather than a guarantee. Answer
everything regardless, because nothing is deducted for a wrong answer.

**The exam is one-way across sections.** Questions are grouped into sections, and once you finish a
section you cannot return to it. Within a section you can flag questions and revisit them from a
review screen until you choose to finish. Read that review screen before you commit.

**The exam tells you its own shape before you start.** The welcome screen states the total number of
questions, how many are standalone, how many case studies there are and how many questions each
holds, and the same for labs. You will not be surprised by a case study; you will only be surprised
by how long it takes if you have not budgeted for it.

A note on labs: DP-600 is scheduled at 100 minutes, which is Microsoft's duration for exams without
labs. Exams that may contain labs are given 120. Microsoft deliberately refuses to confirm which
exams carry labs, so treat a lab as unlikely rather than impossible.

---

## Code on the screen

You will see SQL, KQL and DAX. The audience profile says so directly, and one whole objective group
is about querying data in four surfaces.

You are not asked to write code from scratch. The forms are completion and selection: finish a
snippet, or choose which of four snippets does the job. That means the difference between the right
answer and the best wrong answer is often a single function, a clause, or an argument order.

DAX carries the most weight of the three, because it appears in both *Prepare data* and *Implement
and manage semantic models*. Iterators, table filtering, windowing and information functions are
named in the objectives by name. So is improving DAX performance, which is a different skill from
writing DAX that works.

---

## The exam is open book, and that changes the questions

You get Microsoft Learn in a split screen for the whole 100 minutes. You can open multiple tabs,
search within a page, and resize the split. You cannot reach Q&A, practice assessments, or your own
profile, and you cannot leave the Learn domain.

Microsoft is explicit about why. Learn is there "for those questions that describe problems where
you may need to look something up". It is not there to answer every question, and if you use it that
way you will run out of time. That is deliberate.

So the exam is built to defeat lookup. Questions that could be answered by typing one product name
into a search box do not discriminate between candidates, so there are fewer of them. What is left
is judgement between several options that are all defensible. Two objectives literally begin *Choose
between*.

The practical consequence: rehearse decisions, not definitions. Knowing what a calculation group is
will not be enough. Knowing when a calculation group beats a field parameter is the exam.

Know where to find the documentation you are most likely to need. Good candidates are: the DAX function reference, Direct Lake
documentation, and the security pages. Then leave them alone unless you are genuinely stuck.

---

## Time strategy

100 minutes across roughly 40 to 50 questions is about two minutes each. That is comfortable if you
do not squander it, and tight if you do.

A workable plan:

1. **Answer every question once, in order, without agonising.** Flag anything you are unsure of and
   move on. Most people finish this pass with 25 to 35 minutes left.
2. **Budget the case study separately.** If the welcome screen says there is one, set aside 20 to 25
   minutes for it. It is not timed separately and it will eat your buffer if you let it.
3. **Read case study questions before reading the whole scenario.** The scenario contains far more
   material than the questions need. Knowing what is being asked tells you which sections to read
   properly.
4. **Spend the remaining time on flagged questions**, using Learn on the few where a specific fact
   would settle it.
5. **Never leave a question blank.** There is no penalty for a wrong answer, so a guess is free.

Two clock traps. Breaks do not pause the exam — five minutes are built into the time, but the clock
keeps running, and once you start a break you cannot return to any question you had already seen.
And the section boundary is final, so do not finish a section expecting to come back.

---

## Study strategy

Roughly five to seven weeks at eight to ten hours a week is a realistic plan if you already work
with analytics data. Add time if T-SQL or DAX is new, because *Prepare data* is nearly half the exam
and it assumes both.

The order that works:

**Start with the skills-measured list, not with a course.** All 41 bullets are on one page. Read
each one and ask whether you could do it on a Monday morning. That list is the specification, and
everything else is commentary on it.

**Learn the decisions, not the feature tours.** For each area, the exam wants a choice: which store,
which storage mode, which security boundary, which lifecycle mechanism, which modelling construct,
where the performance cost actually is. Write the comparison out yourself before reading ours.

**Get hands on OneLake, lakehouses, warehouses and semantic models.** A Fabric trial is free.
Building a small star schema end to end teaches more than any amount of reading, because most of
this exam is about things that only become confusable once you have touched them.

**Do the official practice assessment, more than once.** It is free on Microsoft Learn, it draws
from a pool larger than a single sitting shows, and it is the closest published match to the real
wording. Note that it renders only single-answer and multiple-answer questions, so it will not
prepare you for the other formats. That is what the sandbox and this course's mocks are for.

**Check currency on anything that feels recent.** Fabric changes fast. Preview features can appear
if they are commonly used, and some exam questions lag the product. When two sources disagree,
believe Microsoft Learn.

**Answer what Microsoft recommends, not what you built.** The most common way experienced people
lose marks is choosing the option they would actually implement over the one the documentation
endorses. Only one option is keyed, and it is the documented one.

---

## The last 24 hours

Do not learn anything new. Re-read the 41 objective bullets and your own comparison tables. Skim the
traps at the end of each domain file in this course.

Check the practical things. If you are sitting online, clear your desk, confirm your ID, and check
in 30 minutes early. Nobody can be in the room with you.

On the day, read the welcome screen properly before you start. It tells you how many questions you
face and whether a case study is coming. That is thirty seconds that shapes the next hundred
minutes.
