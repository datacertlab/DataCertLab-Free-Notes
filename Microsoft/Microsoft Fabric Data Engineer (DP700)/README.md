# Exam DP-700 — what you are sitting, and how to sit it

**Microsoft Certified: Fabric Data Engineer Associate** is earned by passing one exam,
**DP-700: Implementing Data Engineering Solutions Using Microsoft Fabric**. It is an
associate-level exam for people who already move data for a living, and it assumes you can
read and write Structured Query Language (SQL), PySpark and Kusto Query Language (KQL)
without looking every construct up.

Read this page once before you start studying and once the night before you sit. Everything
here comes from Microsoft's own published material for the current version of the exam.

---

## The figures

| | |
|---|---|
| Exam code | DP-700 |
| Exam guide version | Skills measured as of July 21, 2026 |
| Answering time | 100 minutes |
| Seat time to allow | 120 minutes |
| Passing score | 700, on a scale that runs from 0 to 1000 |
| Question count | Not published — see below |
| Skill areas | Three, each weighted 30–35% |
| Open book | Yes, Microsoft Learn is available during the exam |
| Delivery | Proctored, through Pearson VUE, online or at a test centre |
| Renewal | Free, annually, through an unproctored assessment on Microsoft Learn |

**Microsoft does not publish how many questions DP-700 carries**, and says the number can
vary between attempts. Two official ranges are in print and they do not agree: one Microsoft
page says most of its exams carry between 40 and 60 questions, and Microsoft's exam-readiness
material says most carry between 35 and 50. Neither is a statement about DP-700 specifically.
Prepare against the 100-minute clock rather than a question target, and work out your pace
from the count the exam itself shows you.

**A score of 700 is not the same as answering seven questions in ten correctly.** It is a
scaled score, and Microsoft publishes no mapping from raw answers to the scale. Treat any
readiness figure, here or anywhere else, as a rough guide rather than a predicted result.

There is **no per-domain minimum**. Only the total decides whether you pass, so a weak area
can be carried by strong ones — though with three skill areas of nearly equal weight, there
is not much room to write one off.

---

## What changed in this version

The current outline is dated 21 July 2026, and exactly one thing moved from the previous
edition. Under *Configure Microsoft Fabric workspace settings*:

> "Configure Dataflows Gen2 workspace settings" was replaced by **"Configure Apache Airflow
> workspace settings"**.

Microsoft's change log names that area as the one that moved and calls the change minor.
Setting the two published outlines side by side line by line, nothing else differs. That
single swap matters more than its size suggests, because most study material still tracks the
older outline: it will teach you Dataflow Gen2 workspace settings as an examinable objective,
and it will teach you nothing at all about Apache Airflow workspace settings. If you are
revising from anything written before August 2026, that is the hole in it.

Microsoft reviews its cloud exams quarterly, and Fabric ships features monthly. Where this
course and the live documentation disagree, the documentation is newer — but the exam is
written against the outline above, so answer what the objective asks.

Preview features are fair game. Microsoft's own guide says most questions cover generally
available features, and that preview features may appear where they are commonly used.

---

## The three skill areas

Each is weighted 30–35%, which in practice means roughly a third of the exam each. There is
no cheap area.

| Skill area | Weight | What it is really testing |
|---|---|---|
| Implement and manage an analytics solution | 30–35% | Workspace settings, source control and deployment, security and governance, orchestration |
| Ingest and transform data | 30–35% | Loading patterns, batch and streaming ingestion, and the transformations in between |
| Monitor and optimize an analytics solution | 30–35% | Finding out what broke or slowed down, and choosing the lever that fixes it |

Microsoft publishes no difficulty breakdown across the three, and what follows is how they
tend to feel rather than anything the exam guarantees. The first area often feels the most
structured, because its mechanisms have crisp boundaries and a question usually has one
defensible answer. The second tends to demand more judgement, because several approaches
genuinely work and only one is keyed. The third resists memorisation — you have to read the
symptom and reason from it.

---

## What the questions look like

Microsoft is explicit that it does not identify the formats on a particular exam in advance,
and it publishes no breakdown of how many of each you get. What it does do is name the
formats its role-based exams can use and demonstrate each one in its free exam sandbox. So
treat the table below as the range of things the interface can put in front of you, not as a
promise about your paper. The exam introduction screen tells you what is actually on yours —
read it before you start.

| Format | What you do | Watch for |
|---|---|---|
| Multiple-choice | Pick one answer | The constraint sentence usually decides it |
| Multiple-response | Pick several | Read how many are wanted |
| Build-list | Put steps in order | Order is the answer, not the steps |
| Drag-and-drop | Match items to targets | Every target must be filled |
| Hot-area | Click a region of a screen | Look at the whole screenshot first |
| Active-screen | Configure a settings dialog | Change only what the requirement asks |
| Case-study | Answer several questions from one scenario | You cannot return once you leave it |
| Problem-solution | Say whether a proposed solution meets a stated goal | 2 options, and you cannot go back |
| Labs | Perform real tasks in a live environment | Not on DP-700 at present |

Two of these deserve more than a table row.

**If your exam includes problem-solution sets, they are the format candidates find most
disorienting.** You are given a goal, then a proposed solution, and asked whether it meets
the goal. Then the same goal appears again with a different proposed solution. You see the
same problem several times, and **you cannot go back to an earlier one after answering**.
Answer each on its own merits and resist the urge to make them consistent with one another —
they are separate questions, and more than one of them can be right.

**Where an exam includes case studies, the questions hang off a scenario you can re-read as
often as you like** — but only while you are inside that case study. Once you move on, those
questions are closed. A review screen appears before you leave, so use it. The number of case
studies is shown on the introduction screen and is not published in advance.

**Labs are the one format worth reasoning about in advance.** Microsoft keeps no public list
of which exams contain them, says they can be added or withdrawn, and tells you on the
introduction screen. What is published is the timing: role-based exams without labs are given
100 minutes of answering time, and those that may contain labs are given longer. DP-700's
published answering time is 100 minutes, which points to a paper without labs — but that is
an inference from the timing, not something Microsoft states about this exam, and timing can
change. Read your introduction screen and prepare as though a lab is possible.

The practice questions in this course are multiple-choice and multiple-response, which is
what the platform they are delivered on can present. Where the exam uses another format, the
same knowledge is asked a different way — an ordering question becomes a choice between
complete sequences, a matching question becomes the single decision inside it. What you
cannot practise here is the clicking, so use Microsoft's free exam sandbox once before you
sit, purely to see the interface.

---

## Code on the screen

You will not be asked to write anything from scratch. You will be asked to complete a missing
piece of a snippet, or to choose which snippet does the job, across Transact-SQL (T-SQL),
PySpark and KQL. Answers are often separated by one operator, one clause, or the order of two
lines — so read the code, do not skim it.

You need working fluency in all three languages, not expertise in one. Filtering, grouping
and aggregating, joins, windowing functions, and the merge or upsert patterns are the
constructs that recur.

---

## The exam is open book, and that changes the questions

You have Microsoft Learn in a split screen for the whole exam. Everything on the site except
the questions-and-answers area, the practice assessments and your own profile. You can open
several tabs and search within a page.

Microsoft is direct about why this does not make the exam easier: the resource is there for
the occasional question where you need to look something up, and a candidate who leans on it
for everything runs out of time by design. The clock does not stop, and no extra time is
added.

What this really means for your preparation: **questions whose answer is one search away are
not what this exam is made of.** Most of it is choosing between approaches that all work,
where the stem names a constraint — least privilege, lowest cost, no data duplication, near
real time — and only one option satisfies it. In your job you might implement any of them. In
the exam, pick what Microsoft recommends.

Two habits that pay off:

- Microsoft documents that you can open several Microsoft Learn tabs during the exam. Use
  that: open your language syntax references at the start, before you need them, rather than
  searching from scratch each time.
- Do not open Learn until you have answered everything once. Then spend what is left on the
  questions you flagged.

---

## Time strategy

Microsoft's published ranges put most of its exams somewhere between 35 and 60 questions, so
on a 100-minute clock plan for roughly two minutes a question and check that against the
count the exam shows you. The average hides the shape of it. Recall questions take seconds. A
case study takes a large block, because the scenario has to be read before any of its
questions can be answered.

| Stage | What to do |
|---|---|
| First pass | Answer everything you know. Flag anything that needs thought and move on |
| Second pass | Return to what you flagged. Other questions may have jogged something loose |
| Case study | Keep 20 to 30 minutes for it. It is not timed separately and it eats time |
| Last | Use Microsoft Learn, if any time remains |

Read the problem before the question and the question before the options, and then go back
to the problem — but only the part the question actually needs.

You may take a break whenever you like except inside a lab or inside a problem-solution set,
and you do not have to arrange one in advance. Two things about it matter more than the
break: **the exam clock keeps running**, and every question you have already seen is closed
to you once you come back. Microsoft's exam-experience guidance says five minutes of break
time are built into the exam time, and that questions were removed to fund it — so if you do
not take a break, that time is yours to answer in. Follow whatever the break instructions in
your own exam interface say.

No marks are deducted for a wrong answer, so **never leave anything blank**. Some questions
are worth more than one mark, and Microsoft does not say which.

---

## Study strategy

Treat the outline as a checklist, and be honest about which lines you could actually perform
rather than recognise. That gap is what your study time is for.

**Build things.** This exam rewards having done the task. Connect a workspace to source
control, then do it again with the other provider. Create a deployment pipeline and watch how
items pair and rebind. Load a table incrementally and handle a duplicate. Break something and
find it in the monitoring surfaces.

**Learn the boundaries, not the catalogue.** Nearly every hard question is a choice between
neighbouring things: lakehouse or warehouse, shortcut or mirroring, Dataflow Gen2 or notebook
or pipeline, a workspace role or an item permission. Knowing what each one is will not
separate them. Knowing what each one is *not* will.

**Do the security area properly and early.** The concepts have crisp boundaries, which makes
it an area where a strong understanding pays off across many question scenarios.

**Do not stop at the free module knowledge checks.** They are the easiest questions you will
meet and they will leave you overconfident.

---

## The last 24 hours

- Re-read the outline and this page. Nothing new.
- If you are sitting remotely, run the hardware check the day before, not on the day.
- Have a second monitor if you can. The split screen is cramped on one.
- Know where the timer, the question count, the flag control and the break control are. The
  free exam sandbox shows you all four in the real interface.
- Read the introduction screen when it appears. It tells you how many case studies you have
  and whether there are labs, and it is the only place that information exists.

---

*This page describes the exam as Microsoft published it for the version dated 21 July 2026.
Fabric changes quickly. Where a documentation page you find during the exam disagrees with
something you learned here, the exam is written against the outline above — answer the
objective.*
