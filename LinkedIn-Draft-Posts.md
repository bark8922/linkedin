# 10 Draft Posts

Ready to post, but read them in your own voice first and swap any `[bracket]` for the real detail only you know. A specific true number always beats a vague one. Each has a note on format and which idea-bank entry it came from.

---

## 1. The dashboard that deleted a $6K/month line item
*Territory: AI builds. Format: plain text + a screenshot of the dashboard. Idea #1.*

We were paying about $6K a month for an external analyst to keep our reporting alive.

A few weeks ago I finished a dashboard that does most of what that spend covered. Pulls the data, cleans it, updates itself. I'm an executive assistant, not a data engineer, and I built it mostly by figuring things out as I went.

The strange part wasn't the build. It was the quiet after. No launch, no announcement. A recurring cost just stopped making sense, and that was that.

I keep going back and forth on how to feel about it. On one hand, obviously good, the money stays in the business and the team gets the numbers faster. On the other, a chunk of someone's month of work now runs in the background without anyone thinking about it.

I don't have a tidy conclusion. Mostly I notice that the barrier to building this stuff has dropped further than most job descriptions have caught up to.

---

## 2. The bug that made me stop trusting my own dashboard
*Territory: AI builds. Format: plain text. Idea #2.*

For about [a week] I was reading numbers off a dashboard I built and quietly trusting them. They were wrong.

Not dramatically. Just enough that a total didn't reconcile with the source, and I only caught it because something felt slightly off on a figure I happened to know by heart. The cause was boring: [a join that silently dropped rows when a field was empty].

Here's what it taught me, and it wasn't "test your code." It was that the moment a tool looks polished, you stop questioning it. A messy spreadsheet keeps you skeptical. A clean dashboard invites you to switch your brain off.

Now I trust the ugly draft more than the pretty version, at least until I've tried to break it myself.

Still not sure that instinct scales. But it's saved me twice since.

---

## 3. I'm not a developer and I built it anyway
*Territory: AI builds. Format: plain text or short face-to-camera video. Idea #3.*

I don't have an engineering background. I've still shipped [a handful of] internal tools this year that the team actually uses every day.

I want to be careful here, because the internet's current favorite lie is "anyone can build anything now, no skills required." That's not what I found.

What I found: AI got me past the blank-page part and the syntax I'd never memorize. It did not get me past understanding the actual problem, knowing what "correct" looked like, or noticing when an output was quietly wrong. That part was still on me, and it was still hard.

So the honest version isn't "coding is dead." It's that the gap between an operations person with a clear problem and a working tool got a lot smaller. Not zero. Smaller.

That's a big deal, and it's also more boring than the hype. Both things are true.

---

## 4. The €96K number wasn't the point
*Territory: AI builds. Format: plain text + screenshot, or PDF carousel. Idea #4.*

A recruiting dashboard I built ended up saving roughly €96K a year in tooling. That's the number that gets people's attention.

It's not the part that mattered.

Before, seeing the state of the pipeline meant waiting on a report someone else assembled. Days of lag, sometimes a week. The real change wasn't the cost, it was that the team could open a tab and see the funnel, time-to-hire, and where candidates were actually getting stuck, that same morning.

The savings were a one-time headline. The daily visibility changed how people made decisions, quietly, every day.

I've started to think cost savings are the least interesting thing automation does. The speed at which people can see reality is the thing that actually moves work. The euros just get the meeting booked.

---

## 5. My job title says one thing. My work says another.
*Territory: EA-to-ops. Format: plain text. Idea #9.*

On paper I'm an executive assistant.

In practice, most of last month I was building data infrastructure and automations for a recruiting company.

I'm not saying that to complain, the opposite. It's one of the more interesting things I've watched happen to a role in real time. The assistant seat has always been the place with the widest view of where an org actually leaks time. What's new is that the person in that seat can now do something about it directly instead of just flagging it.

I don't think "executive assistant" describes what a lot of us in this seat now do. I also don't have a better title, and I'm not sure I need one.

Curious if anyone else's day-to-day has drifted this far from their title. What does yours actually say vs what you actually do?

---

## 6. What I stopped doing when I started building
*Territory: EA-to-ops. Format: plain text. Idea #10.*

A year ago, a real slice of my week was moving numbers between systems by hand. Copy from here, paste there, reconcile, repeat. [Rough estimate: X hours a week.]

Almost none of that is on my plate now. I wired the systems together and the copy-paste just stopped existing.

The interesting question was never "how do I do this faster." It was "what do I do with the hours that opened up." Honestly it took me a while to answer well. For a bit I just filled the time with more small tasks, which defeats the point.

What actually helped was using the freed time on the problems that don't automate: the judgment calls, the messy human stuff, the things worth thinking slowly about.

The automation was the easy part. Not wasting what it gave back turned out to be the harder skill.

---

## 7. The thing I automated that I shouldn't have
*Territory: AI builds / taste. Format: plain text. Idea #8.*

I automated a [process] a while back that, in hindsight, I should have left alone.

It worked fine, technically. The problem was that the manual version quietly included a judgment step, someone glancing at the thing and going "that looks off." When I automated it, I automated away the glance too. Nothing broke loudly. It just meant a small human check disappeared, and a few weeks later that missing check cost more than the time I'd saved.

I unwound part of it and put the human back in the loop on purpose.

I think the reflex right now is to automate anything that repeats. But some things repeat because a person is quietly making a call each time. Automating the steps is easy. Noticing which step was actually a judgment is the harder part, and I got it wrong here.

---

## 8. What hiring looks like from the ops seat, not the recruiter seat
*Territory: Recruiting from the inside. Format: plain text. Idea #14.*

I'm not a recruiter. I want to say that clearly before I say anything about hiring.

But I work inside a recruiting company and I build the systems that track the pipeline, so I spend my days looking at the data underneath the process rather than running the process itself. It's a strange, useful angle.

The thing I keep noticing from here: the stage everyone assumes is the bottleneck usually isn't. [In our data, the drop-off that hurt most was at ___, not where people expected.] It's easy to believe a story about where things get stuck. It's harder, and more uncomfortable, to look at where they actually get stuck.

I don't have recommendations. I'm not in a position to give them. Just an observation from someone who sees the numbers but doesn't own the outcome: the funnel rarely leaks where the meeting says it does.

---

## 9. The metric everyone watches vs the one that actually predicts
*Territory: Recruiting from the inside. Format: plain text + screenshot. Idea #15.*

Building a dashboard forces you to notice which numbers people stare at.

In hiring, a lot of eyes go to the top-of-funnel count, how many candidates came in. It's visible, it feels like progress, and it's mostly a vanity number.

The one that actually seemed to predict whether a role closed was less obvious: [time-in-stage at ___ / speed of the first response / whatever your data showed]. Not how many entered, but how fast the ones who mattered moved through.

I'm hedging on purpose here, this is one company's data and I build the reports, I don't run the hires. So take it as an observation, not a law.

But it's made me suspicious of any single headline metric. The number that's easy to see and the number that's actually doing the predicting are rarely the same one.

---

## 10. The question I can't answer yet
*Territory: Cross-cutting / open. Format: plain text. Idea #20.*

Here's something I build with every week and still haven't resolved: how much to trust an automated output before a human looks at it.

Too much oversight and you've just made a slower version of the manual process, now with extra steps. Too little and you're one silent failure away from a number nobody caught being wrong for a month.

I don't have a rule for it. Right now I go case by case, mostly on gut: how bad is it if this is wrong, and how loudly would it fail. Which is not a satisfying answer for someone who likes systems.

I don't think "keep a human in the loop" is wrong, exactly. It's just not specific enough to actually use. Which loop. Which human. Checking what, how often.

Genuinely asking, if you've automated real work: how do you decide where the human has to stay?

---

## Posting order suggestion
If you want a gentle on-ramp: start with **#5** (job title vs work) or **#2** (the bug) — both are humble, low-exposure, and very you. Save **#1** and **#4** for when you're ready for a bigger one, they're your strongest but also the most visible. **#10** is the safest "high-value" post because it's literally just an honest question.
