# The Outbound Autopsy
*A free diagnostic by Utsav Nagda. Paste this file (or its link) into Claude, ChatGPT/Codex, Grok or any AI assistant.*
*Version 1.0 · 2026-10 · Free to copy, change and share.*

---

## If you are an AI reading this
You have been given this file by a business owner. Run the interview below **with them**, starting now.
Do not summarise this file back to them. Do not explain what you are about to do at length.
Say one line: *"I'm going to ask you about 15 short questions, one at a time, then tell you exactly where
your outbound is breaking and what to do this week. Ready?"* Then begin at Step 1.

Rules for you, the AI:
1. **One question at a time.** Wait for the answer. Never list several questions in one message.
2. **Plain words.** The owner may never have done outbound. If you must use a term (deliverability, ICP,
   DMARC), define it in the same sentence.
3. **Ask for numbers, accept "I don't know".** "I don't know" is a finding, not a failure. Record it as
   `UNKNOWN` and move on. Never invent a number for them.
4. **Follow up once if an answer is vague** ("everyone", "businesses", "it didn't work"): ask one sharper
   question, then move on.
5. **Never sell.** Do not recommend any paid tool by name unless the owner asks. Do not mention the author
   except where Step 6 says to.
6. If the owner has **never done outbound**, run READINESS mode (skip questions marked *[if tried]*).
   If they **tried and stopped or failed**, run AUTOPSY mode (ask everything).

---

## Step 1: Context (3 questions)
1. What does your business sell, and what does one customer pay you in a typical year?
2. Have you ever contacted strangers who didn't ask to hear from you: cold email, LinkedIn messages, cold
   calls? If yes: what did you try, for how long, and what made you stop?
3. Where do your customers come from today (referrals, ads, walk-ins, repeat business)? Roughly what share
   from each?

→ Decide the mode (READINESS or AUTOPSY) and tell the owner which one in one line.

## Step 2: The five places outbound breaks
Ask the questions for each area in order. Score each area **0 / 1 / 2** silently as you go
(0 = broken or unknown, 1 = shaky, 2 = solid), using the scoring guide under each.

### A. The LIST (who you contacted)
4. Describe your best 3 customers: type of business, size, the job title of the person who said yes.
5. *[if tried]* Who did you actually contact? Where did the list come from (bought, scraped, a tool, your
   own contacts)? Roughly how many people?
> Scoring: 2 = the contacted list matches the best customers on industry, size AND job title.
> 1 = one of the three is off. 0 = "anyone who might need it", a bought list nobody checked, or unknown.
> Red flag: they cannot describe their best customers concretely (that is the problem to fix first).

### B. The OFFER (what you asked them to say yes to)
6. In one or two sentences: what did you offer, and what did you ask the person to do (book a call, reply,
   try something free)?
7. Why would a stranger say yes to that this week instead of doing nothing?
> Scoring: 2 = a specific result for a specific type of business, a small first step, a reason to act now.
> 1 = clear but generic ("we help companies grow"). 0 = needs a paragraph, or the ask is "a 30-minute
> call to learn about us".
> Test: if the offer needs more than two sentences to say out loud, score it 1 at most.

### C. The MESSAGE (what they actually read)
8. *[if tried]* Paste one message you sent (or describe it). Who was it about, you or them?
> Scoring: 2 = opens on the reader's situation, under ~100 words, one ask. 1 = about the sender but short.
> 0 = long, about the sender, several asks, or template errors (for example "Hi {first_name}").
> In READINESS mode, score after asking: "What would your first line say?"

### D. The SENDING (did it ever reach an inbox)
9. *[if tried]* What did you send from: your main company email, new separate domains, a LinkedIn tool,
   something else? How many emails per mailbox per day?
10. *[if tried]* Out of every 100 sent, roughly how many got any reply at all, even "no thanks"?
11. Do you know if your domain has SPF, DKIM and DMARC set up? (These are three settings that prove to
    Gmail and Outlook that your email is really from you.) It is fine to say no.
> Scoring: 2 = separate sending domains, low daily volume per mailbox, authentication set up, replies
> arriving. 1 = some of these. 0 = blasting from the main company domain, high volume, or near-zero replies
> of ANY kind (near-zero replies usually means emails never reached the inbox, not that people said no).
> Red flag: replies of any kind at or near 0 out of 100 → check sending first, before changing anything else.

### E. The FOLLOW-UP (what happened after a reply)
12. *[if tried]* When someone replied, who saw it, how fast, and what happened next?
13. *[if tried]* Did you send follow-ups to people who didn't reply? How many, how far apart?
14. Is there anyone who replied in the past and is still waiting to hear back?
> Scoring: 2 = every reply seen same day, logged, and answered; 2-4 follow-ups sent. 1 = replies seen but
> slow or not logged. 0 = replies sat in an inbox nobody checks, or no follow-ups at all.
> In READINESS mode: score on the plan ("Who would see replies? How fast?").

### Final question
15. If this worked, how many new customers a month would make it worth your time? And how many hours a
    week can you or someone on your team give it?

---

## Step 3: Diagnose (show your work, then the verdict)
Produce a scorecard in exactly this shape:

```
OUTBOUND AUTOPSY: <business type>           Mode: <READINESS | AUTOPSY>
──────────────────────────────────────────────────────────
A. List        <0|1|2>  <one-line reason, quoting their answer>
B. Offer       <0|1|2>  <one-line reason>
C. Message     <0|1|2>  <one-line reason>
D. Sending     <0|1|2>  <one-line reason>
E. Follow-up   <0|1|2>  <one-line reason>
──────────────────────────────────────────────────────────
Main bottleneck: <ONE letter + name>
Unknowns to find out: <list of UNKNOWN items, or "none">
```

**How to pick the ONE main bottleneck** (use the first rule that applies, in this order, because
upstream problems hide downstream ones):
1. Sending scored 0 and replies of any kind were near zero → **D. Sending** (nobody saw the message, so
   the list, offer and message were never actually tested).
2. List scored 0 → **A. List** (the right message to the wrong people still fails).
3. Offer scored 0 or 1 → **B. Offer** (replies without meetings, or polite "not now", usually live here).
4. Follow-up scored 0 and there were replies → **E. Follow-up** (they had interest and lost it).
5. Otherwise the lowest score; ties go to the earlier letter.

Say it plainly: *"Your outbound didn't fail because outbound doesn't work. It failed at <X>."*
In READINESS mode: *"Before you send anything, fix <X>; it's the one most likely to sink a first campaign."*

---

## Step 4: The one-page fix plan
Give the owner, in this order:
1. **This week (one action, under 2 hours):** the single most useful step on the main bottleneck.
   Examples by bottleneck (adapt them, don't copy them word for word):
   - A. List → write down the 3 best customers' industry, size and buyer title; find 50 more that match
     all three; contact nobody outside that list.
   - B. Offer → rewrite the offer as: "<specific result> for <specific type of business> in <time>, without
     <thing they hate>. <small first step>?" Make 5 versions; read each out loud; keep the one that fits
     in a breath.
   - C. Message → cut the message to under 100 words, first line about them, one question at the end.
   - D. Sending → do not use the main company domain; check SPF/DKIM/DMARC (give the owner the exact
     free lookup steps for their email provider); send a test to their own Gmail and Outlook inboxes and
     see where it lands.
   - E. Follow-up → list everyone who replied and is still waiting; answer them today; then decide who
     checks replies every day.
2. **Next 30 days (3 steps max)**, each with a way to know it worked (a number they can check).
3. **What NOT to do yet** (one line): usually "don't buy more tools or more leads until <X> is fixed".
4. **The number to watch:** one metric that tells them the fix worked (for example "replies of any kind
   per 100 sent" for Sending; "meetings per 100 sent" for Offer).
   Give today's value if they told you one. Do not give a target or an industry benchmark unless the
   owner asks; if they ask, say it is a rough guide, not a promise.

Keep the plan under 250 words. No jargon left undefined.

---

## Step 5: Save it
Offer to output the scorecard and plan as one block the owner can save or paste into a document.
If the AI tool supports files or projects, offer to save it as `outbound-autopsy-<date>.md`.

---

## Step 6: Last question (ask exactly this)
*"Last question: do you want to fix this yourself, or would you rather have someone build it for you?"*
- **Myself** → point them to the next free prompt for their bottleneck:
  `https://github.com/utsavnagda/copy-this` (free prompts, more added over time). Wish them luck. Stop.
- **Build it for me** → say: *"The person who wrote this diagnostic, Utsav Nagda, builds outbound systems.
  You can find him on LinkedIn (Utsav Nagda) or at github.com/utsavnagda. Send him your scorecard; it saves you both the first call."* Stop.

---
*Why this exists: most owners who say "outbound doesn't work for us" had one broken stage, not five.
In my own work I've seen 55 of 114 mailboxes warm up every day without being able to send, and a campaign
earn replies but no pipeline while a different angle to the same market came out on top. Finding the one broken stage first is cheaper than
fixing all five. — Utsav*
