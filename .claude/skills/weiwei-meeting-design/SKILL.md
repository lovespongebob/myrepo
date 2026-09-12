---
name: weiwei-meeting-design
description: >-
  Design meetings that produce measurable outcomes, using the methodology from
  Kevin M. Hoffman's "Meeting Design: For Managers, Makers, and Everyone." Use
  this skill whenever the user wants to plan, run, improve, or evaluate any
  meeting or workshop: kickoffs, brainstorms, stand-ups, check-ins, retros,
  postmortems, stakeholder interviews, pitch meetings, critiques, strategy/OKR
  sessions, presentations, workshops, and leadership meetings — 1:1s,
  skip-levels, staff meetings, all-hands, business reviews (QBR/MBR), and
  executive readouts. Also trigger when the user complains meetings are too
  long, frequent, or unproductive; asks for an agenda or facilitation plan;
  asks how many people to invite or how much time to book; asks how to handle
  conflict, tangents, or a dominating stakeholder; or asks whether something
  should be a meeting at all. Trigger even if "meeting" never appears — "plan
  our kickoff," "our standups feel useless," "I need to run a retro," and
  "prep me for my QBR" are all in scope.
---

# Meeting Design

Design meetings the way a designer approaches any product: define the job the
meeting must do, work within the real constraints (human memory, headcount,
time), and structure the conversation so it converges on decisions and actions.
Distilled from Kevin M. Hoffman, *Meeting Design: For Managers, Makers, and
Everyone* (Two Waves Books, 2018).

## Input

Collect these five facts before designing anything. If the user's request
already contains them, don't re-ask; if one or two are missing, make a
reasonable assumption and state it in the output. Ask questions only when the
answer would change the design significantly (e.g., headcount of 5 vs. 25).

1. **Desired outcome** — what should exist or be decided after the meeting that
   doesn't exist now? ("Discuss X" is not an outcome; "a prioritized list of X"
   is.)
2. **How the outcome will be measured** — count of decisions, action items,
   viable ideas, resolved questions, etc.
3. **People** — how many, their roles, and any power dynamics (execs present?
   client vs. vendor? strangers vs. an established team?).
4. **Time available** — and whether it's flexible.
5. **Stage of work** — beginning (starting something), middle (in-flight work),
   or end (closing/reflecting). This selects the template family. Recurring
   leadership meetings — 1:1s, skip-levels, staff meetings, business reviews,
   all-hands, executive readouts — are their own family regardless of project
   stage; use `references/leadership-meetings.md` for those.

Also useful when offered: remote vs. in person, organizational culture
(hierarchical vs. flat), and what has gone wrong in past meetings.

## Workflow

### Step 1: Confirm a meeting is the right tool

A meeting is a synchronous communication tool that costs everyone's combined
paycheck for the allotted time. Before designing one, apply the two-question
test:

- What outcome will this meeting enable that can't be achieved without it?
- How will that outcome be measured?

If the user can't answer the first question, or the job is pure information
transfer, recommend a cheaper asynchronous channel (a document, chat thread, or
email) instead — and say why. For an existing recurring meeting, also ask: why
was it established, and has that job already been done? If the job is done or
was never defined, the right design is to delete or decline the meeting.

### Step 2: Do the agenda math

Read `references/agenda-building.md` for the full method and worked examples.
The core numbers:

- One "just-complex-enough" concept = a sentence or two (fits on a sticky note).
- Cover **5 concepts per 10 minutes, then 10 minutes of review/discussion** —
  one 20-minute content section. About 15 concepts fit in an hour, and it's
  better to plan for fewer to leave room for tangents.
- Points of agreement between n people = n(n-1)/2. Cap discussions at **6–7
  people**; split larger groups into parallel subgroups of 5–7 that each
  converge on one idea, then share out.
- **The six-and-90 rule**: conversations don't get deep with more than six
  people, and they run out of gas after about 90 minutes. Schedule breaks at
  or before the 90-minute mark; break listening into 20–30 minute chunks.

If the requested content doesn't fit the requested time and headcount, show the
math and propose the trade-off (cut concepts, add time, or split into groups)
rather than silently producing an overstuffed agenda.

### Step 3: Pick and adapt a template

Match the stage of work to a template in `references/meeting-templates.md`,
which contains the goal, outcome measure, and sample agenda for each meeting
type in the book:

- **Beginning**: stakeholder interview, quick kickoff ("quickoff"), brainstorm
  (KJ method + dot voting), OKR/strategy session, full project kickoff workshop
  (ARCI, hypothesis design, design studio), and a pitch/proposal meeting for
  any two parties assessing fit (team↔sponsor, vendor↔client, partners).
- **Middle**: daily scrum, weekly project check-in, lean coffee, deliverable
  presentation, design critique, and a build-your-own workshop structure
  (including Adam Connor's "work backward from the actions the team must take
  afterward" planning method).
- **End**: UAT defect log review, agile retrospective, blameless postmortem.
- **Leadership** (recurring organizational meetings, in
  `references/leadership-meetings.md`): 1:1 and skip-level, leadership staff
  meeting, key business review (QBR/MBR), all-hands broadcast, and executive
  readout (presenting up for a decision). These apply the book's method to
  executive contexts — status moves to writing, and past ~40 people the
  meeting becomes a broadcast where chunked content and upvoted Q&A replace
  discussion and dot voting.

Templates are starting points, not scripts. Adapt timings with the agenda math
and tailor activities to the user's culture and outcome. When the user's time
budget sits between two templates (e.g., a 2-hour kickoff vs. the 1-hour
quickoff and the 4–8-hour workshop), compress by moving alignment work into
asynchronous pre-work — stakeholder interviews, expectation scoring,
pre-reads — and spend the synchronous time only on what needs synchrony:
resolving conflict, generating ideas together, and deciding. A well-designed
agenda still works when it's "mostly broken" — prefer structures that survive
interruptions and derailment over brittle minute-by-minute scripts.

### Step 4: Design the facilitation

Read `references/facilitation.md` before writing any facilitation plan — the
four roles, question classes, and style guidance below are summarized from it,
and the full detail matters most when the meeting involves conflict, senior
stakeholders, prioritization, workshops, or remote attendees. Always cover the
basics in the output:

- **Assign the four roles**: facilitator (neutral process guide), public
  recorder (visible group memory — never a private note-taker), leader (states
  the intent, then behaves as a group member or stays away), group members.
  Flag when the requester is too invested in the outcome to facilitate
  neutrally, and suggest a neutral facilitator plus a subject-matter-expert
  seat instead.
- **Shape the conversation as divergence then convergence**: open up options
  before narrowing to decisions. Divergence-only is pointless brainstorming;
  convergence-only shuts people down.
- **Design 3–5 facilitation questions** using humble inquiry: questions that
  surface feelings, motivations, actions, or systems — with the asker's own
  preferred answer removed.
- **Plan capture**: visible real-time recording (whiteboard/stickies/shared
  doc), a parking lot for valuable tangents (with a commitment to revisit it),
  and voting methods (e.g., dot voting) that let people prioritize without
  talking over each other.

### Step 5: Produce the output

Assemble everything from steps 1–4 into the Meeting Design Brief below. When
the user described past meeting failures while asking for a new design, open
the brief with a short diagnosis that maps each failure to the specific design
choice that fixes it — it shows the design is a response to their situation
rather than a generic template.

## Output format

Deliver a **Meeting Design Brief** in markdown using exactly this structure
(omit a section only when it genuinely doesn't apply, e.g., no recurring-meeting
review for a one-off interview):

```markdown
# Meeting Design Brief: [meeting name]

## The job of this meeting
- **Outcome:** [what exists/is decided afterward]
- **Success measure:** [how to count/verify it]
- **Cost check:** [n people × duration; why a meeting beats async here]

## People ([n] total — [note if split into subgroups])
- [Name/role] — [why they're needed / ARCI role]
- **Facilitator:** [who, and why they can stay neutral]
- **Recorder:** [who; capture method]

## Preparation
- [what to send in advance, pre-meeting interviews, materials, room/tools]

## Agenda ([total duration])
| Time | Block | What happens | Mode |
|------|-------|--------------|------|
| 0:00–0:10 | ... | ... | [divergent/convergent; talk/visual/write] |

## Facilitation plan
- **Opening statement of purpose:** [one sentence to say verbatim]
- **Key questions:** [3–5 humble-inquiry questions]
- **The turn:** [when and how to switch from divergence to convergence]
- **Risks & recovery:** [likely derailments and the fallback move for each]

## After the meeting
- [action-item capture and distribution, e.g., photo of the wall/board]
- [follow-ups; when to check whether the meeting did its job]
- [for recurring meetings: the condition under which this meeting gets deleted]
```

For quick requests (e.g., "give me a 15-minute standup agenda"), compress the
brief to the sections that matter — job, agenda, facilitation notes — but never
omit the outcome and its measure: they are what make it a designed meeting
rather than a scheduled one.

When the user asks to **fix an existing meeting** rather than create one, run
the same workflow as a diagnosis: state the meeting's supposed job, identify
which constraint is being violated (undefined outcome, too many people, too
many concepts, no facilitation roles, no convergence, too long for memory),
and propose the smallest set of format changes to test next time — small
iterative changes over wholesale reinvention, and measure after each change.

## Principles to keep in view

- People's brains are the universal design constraint: working memory holds
  ~30 seconds, sessions over 90 minutes blur action items, and pairing
  complementary visuals with talk builds stronger memories than talk alone.
  Never design a meeting that is only listening.
- Conflict is material to work with, not a failure state. Surface it early
  (stakeholder interviews, priority scoring with standard deviations), give it
  structure (facilitated divergence/convergence), and keep it about the process
  rather than the people ("blameless" framing).
- Meetings both reveal and change organizational culture. When a user's meeting
  problem is really a culture problem (deference to executives, blame,
  knowledge silos), say so, and borrow patterns from
  `references/meeting-templates.md` §Culture notes.
- Every recurring meeting must eventually be deleted. Build the exit condition
  into the design.
