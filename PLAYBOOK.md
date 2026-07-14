# LinkedIn Playbook

Written 14 Jul 2026, after throwing out three earlier versions that were all wrong.
Read this before generating anything. It is the spec, not a suggestion.

---

## The one rule that outranks everything else

**It has to be true.**

Not "true-ish." Not "true if you squint." Not a real fact with a flattering frame bolted on.

Things that have already been caught and must never happen again:
- Inventing a detail because it sounded good (a screenshot of "greyed-out nodes" that don't exist).
- Inflating Blake's role (claiming he designed the dashboard logic from scratch — he didn't; a data analyst built the logic, Blake rebuilt the system around it and has built a lot on top of it since).
- Rhetorically neat claims that aren't accurate ("nothing I've built has ever stopped running" — plenty has).
- Framing something as a deliberate choice when it was a constraint (the 12-second payment gap is a Revolut API rate limit, not a philosophy).

If a fact can't be verified in n8n, the repos, Slack, the Cowork session history, or Blake's own words: **don't write it.** Ask instead. A missing post is fine. A post with a lie in it is not, because his boss, his colleagues, and possibly the former analyst all read this.

---

## The second rule

**Stakes, or don't bother.**

The failed drafts were all technically accurate, well-mannered, and completely skippable. They were boring because nothing was at risk and nobody was in them.

A post needs at least one of:
- Something that could go wrong and matters (money, someone's pay, a number people are judged on).
- A real position that someone could disagree with.
- A person other than Blake, and the effect the thing had on them.
- A question Blake actually can't answer.

"Interesting observation about data" is not stakes. It is the thing to avoid.

---

## The third rule

**Having an opinion is not arrogance.**

Blake spent three rounds pushing back on anything that made him sound like a know-it-all, and the result was a man with no point of view, which is worse. He is allowed to think things. He is allowed to be wrong in public.

What he is not allowed to be:
- Preachy ("here's what you should do").
- The hero of the story.
- Ungenerous about colleagues, especially the analyst whose logic he inherited and respects.

The line is: **have a position, don't have a lesson.**

---

## Voice

- Lead with a specific fact, moment or object. Never a stat, never a moral.
- Report and argue. Never instruct.
- Include the friction: the cost, the doubt, the bit that didn't work, the thing he refuses to do.
- One idea per post. No listicles.
- End on a real position or a real open question. Never a tidy takeaway.
- Sound like someone talking to a coworker.
- Generous to named or implied colleagues. Never "we used to pay someone a lot of money."

**Banned:** em dashes. "Thrilled to announce." "Humbled." "Hot take." "Unpopular opinion." Broetry. Engagement bait. "Here's what I learned." Anything that opens with a statistic and then pivots to Blake's CV.

**Self-check before shipping any angle:**
1. Is every factual claim in it verifiable?
2. Could someone disagree with it? (If no: it's boring.)
3. Would a colleague reading it feel respected?
4. Could only Blake have written it?

---

## Pillars

**1. What actually got replaced.** His sharpest lane. The AI conversation says the analysis got automated. What actually got removed was the scaffolding around the analysis: pipelines, licences, tooling. The thinking was never the expensive part. He has receipts and a genuine argument.

**2. What the automation can't catch.** Everything he runs has an error handler or a watchdog. They catch failure. They do not catch a number being quietly, plausibly wrong within tolerance. Nothing fires. Nobody knows. This is the richest and most unresolved thing he owns.

**3. What he refuses to automate.** The human step. The confirm-before-money-moves click. Not a technical decision. The stakes pillar.

**4. What automation does to the people downstream.** He builds things that chase, nudge and DM his actual colleagues, and then has to see them. The bot never forgets, so the pressure went up and nobody decided that. Almost nobody writing about AI has to look these people in the eye.

**5. Small true things from the machine room.** The 0.85 confidence threshold. The compression that renamed a file and silently served stale numbers. Cheap to produce, high hit rate, but cannot be the whole diet.

**6. Recruiting from the data seat.** Occasional. Max one in five. He works in recruiting, he is not a recruiter, and he never pretends otherwise.

---

## Cadence

- 1 to 2 posts a week. No streaks, no daily grind.
- Never two posts on the same underlying story.
- Rotate pillars. If the last three were all pillar 5, stop.
- No introduction post. He has never posted; the first one just starts. The work is the introduction.

---

## Generation process (this is the bit the scheduled task kept getting wrong)

**Wrong order (what was happening):** find a trend → bolt Blake's CV to it → sprinkle humility on top.

**Right order:**
1. **Dig his actual systems first.** n8n workflows and execution history. The repos (bark8922/tribe-dashboard, tribe-recruiting, daily-pulse). Cowork session history. Slack (his own messages, public channels, watchdog alerts). Gmail. Look for: something that broke, something that surprised him, something he decided not to do, something a colleague said.
2. **Find the felt thing.** The test is whether Blake would recognise it as something he has actually thought about. Posts assembled from search results read as assembled.
3. **Only then** check what's being discussed publicly, and only to see if it opens a door for a thing he already believes. The news is the doorway, never the source.
4. Draft with stakes. Check against the four self-check questions.
5. Flag anything unverified rather than writing around it.

---

## Ready to post

**A. The one to open with.**

> Every automation I run has something watching it. If a workflow fails, I get a message. If a number swings hard from last month, I get a message.
>
> None of that catches a number being slightly wrong.
>
> If a figure on the dashboard is off by two percent, nothing fires. No error, no alert, no red flag. It just sits there looking exactly as confident as the right number would have looked.
>
> That's the part I actually think about. Breaking is fine. Breaking is loud. The thing that worries me is an automation working perfectly and being quietly, plausibly wrong, in a way that's within tolerance for every check I've written.
>
> I don't have a good answer for it. I'm not sure the industry does either, and it's rushing ahead anyway.

Pillar 2. Post this first. It needs no introduction and it tells a stranger everything.

**B.**

> Our reporting used to run on a setup built by a data analyst. The logic in it was good. I've barely changed it, because it was right.
>
> When I rebuilt the whole thing this year, what actually disappeared wasn't his thinking. It was everything around his thinking. The pipeline, the licences, the tooling that existed purely to carry the logic from one place to another.
>
> I kept the logic. Understanding it was most of the job. And once I understood it, I could build things on top that weren't possible before, and build them fast, because I finally knew what every number meant.
>
> That's where I'd push back on the AI conversation. It didn't replace the analysis. It removed the scaffolding around the analysis.
>
> Those are very different things, and only one of them was ever the expensive part.

Pillar 1.

**C.**

> Paying contractors used to take me the best part of a day. Open each invoice. Write the number on a sheet. Compare it to what that person was supposed to get. Chase the difference if there was one. Repeat for everybody. Send the pile to the accountants. Then set up every single payment in the bank by hand, one at a time.
>
> Now the comparing happens automatically and the payments go out automatically.
>
> There's exactly one step I kept: I have to look at the numbers and confirm they're right before anything moves.
>
> I could automate that too. It would work. It would probably keep working for months.
>
> I'm not going to. It's not a technical decision. It's the one step where being wrong means a person doesn't get paid, and I want a human name attached to that.

Pillar 3.

---

## Idea bank (verified, not yet drafted)

- **The 0.85 threshold.** Every AI system has a number where somebody decided to stop trusting the machine. His is 0.85, in the categorisation approval queue. He picked it because it felt about right. So did everyone else who picked theirs. (Pillar 5)
- **The optimisation that was the bug.** A data file got big, so it got compressed. The compression renamed it. The dashboard kept looking for the old name and silently served stale numbers to everyone. Nothing failed. That was the problem. (Pillar 5)
- **The refresh gap.** Someone added two candidates at 14:26. The 14:40 refresh had already pulled its copy of the data at 13:51. To them, the system was broken. It was working exactly as designed. Nobody experiences a refresh schedule; they experience doing a thing and the computer not noticing. (Pillar 4)
- **The chase bot never forgets.** A human chaser forgets, gets busy, lets it slide. The bot doesn't. Pressure on people went up and nobody decided that. (Pillar 4)
- **The monthly false alarm.** On the 1st of every month the "current month has revenue" check fails, correctly, because revenue isn't booked yet. Once a month the system teaches him not to quite believe it. Monitoring is paid for in attention. (Pillar 2)
- **Two systems, two headcounts.** BambooHR says one number of active employees, the pipeline's own file says another. Neither is broken. They define "works here" differently and nobody ever had to reconcile them. (Pillar 1 or 5)
- **The manual fallback never leaves.** "If it's not fixed quickly I'll just do it manually." There is always a person standing behind the automation with a mop. (Pillar 3)
- **Backfilled stage dates.** If someone was hired they must have had an offer, an interview, a screen. Missing dates get filled in backwards from the hire. A good chunk of every time-in-stage chart is inferred, not recorded. (Pillar 6)
- **Four guesses at identity.** LinkedIn URL, then internal ID, then nickname, then email. Every conversion rate sits on top of that guess. (Pillar 6)

---

## Graveyard (do not resurrect)

- Any post that opens with a Gartner or MIT statistic.
- "I'm the single point of failure and it's a risk to the company." He hates it. It centres him and it whines.
- The greyed-out n8n nodes. They don't exist.
- Token cost / CLI comparisons. Not his lane, not his problem, and he had to ask what a CLI was.
- "The tools are selling you the ability to skip the setup." He doesn't believe it.
- Anything framing the 12-second payment gap as a deliberate design choice. It's a rate limit.
- An introduction post.
