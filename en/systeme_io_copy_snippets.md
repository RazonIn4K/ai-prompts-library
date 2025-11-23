# Systeme.io Campaign Copy Snippets

**CATEGORY:** Email Marketing / Marketing Automation
**PURPOSE:** Reusable email copy for systeme.io campaigns including welcome sequences, nurture flows, discovery call CTAs, and drip reminders
**VARIABLES:** `{first_name}`, `{offer_name}`, `{bonus}`, `{deadline}`, `{calendar_link}`, `{sender_name}`, `{company_name}`
**TONE:** Warm professional, conversational mentor, encouraging without being pushy

---

## Segment Definitions

| Segment | Description | Email Approach |
|---------|-------------|----------------|
| **New Lead** | Just opted in, high curiosity, unfamiliar with you | Focus on building trust, delivering immediate value, setting expectations |
| **Warm Lead** | Engaged with content, opened emails, clicked links | Focus on deepening relationship, addressing objections, moving toward action |
| **Inactive** | No engagement in 14-30+ days | Focus on re-engagement, curiosity hooks, low-pressure value delivery |

---

## 1. Welcome Emails

### 1A. Welcome Email — New Lead

**Subject Lines (choose one):**
- Welcome aboard, {first_name} — here's what's next
- You're in! Let's get you started
- {first_name}, your first step starts here

**Email Body:**

```
Hey {first_name},

Welcome — I'm genuinely glad you're here.

You just made a smart decision by joining [community/list/program]. Most people stay stuck because they never take that first step. You did.

Here's what you can expect from me:
• Practical strategies you can use immediately (no fluff)
• Honest advice based on real experience
• Resources designed to help you [achieve specific outcome]

First things first — hit reply and tell me: what's your biggest challenge right now with [topic]?

I read every response. Seriously.

Talk soon,
{sender_name}

P.S. Keep an eye on your inbox. I've got something valuable coming your way in the next email.
```

**Systeme.io Tags:** `new_lead`, `welcome_sent`
**Automation Trigger:** Immediately after opt-in

---

### 1B. Welcome Email — Lead Magnet Delivery

**Subject Lines:**
- Here's your {bonus} — as promised
- Your download is ready, {first_name}
- Got it! Here's your {bonus}

**Email Body:**

```
Hey {first_name},

As promised, here's your copy of {bonus}:

[DOWNLOAD BUTTON: Get Your {bonus}]

This isn't just another PDF that sits on your desktop collecting dust. Inside, you'll discover:

• [Key benefit/insight #1]
• [Key benefit/insight #2]
• [Key benefit/insight #3]

My recommendation? Block 15 minutes today, grab a coffee, and go through it. Then pick ONE thing to implement this week.

That's how real progress happens — one action at a time.

Questions? Just hit reply.

{sender_name}

P.S. Tomorrow I'll share [preview of next email content] — you won't want to miss it.
```

**Systeme.io Tags:** `lead_magnet_delivered`
**Automation Trigger:** Immediately after opt-in (or 5-minute delay from welcome)

---

### 1C. Welcome Email — Warm Lead Returning

**Subject Lines:**
- Good to see you back, {first_name}
- {first_name}, welcome back — things have changed
- We missed you (and have something new)

**Email Body:**

```
Hey {first_name},

I noticed you're back — and I'm glad.

A lot has happened since we last connected. I've been working on some new things I think you're going to love.

Here's what's new:
• [New resource/update #1]
• [New resource/update #2]
• [New feature/improvement #3]

No need to catch up on everything. Just start here:

[CTA BUTTON: Check Out {offer_name}]

Welcome back. Let's make this count.

{sender_name}
```

**Systeme.io Tags:** `returning_subscriber`, `warm_lead`
**Automation Trigger:** Re-subscribe or tag-based segment entry

---

## 2. Nurture Touchpoints

### 2A. Value Email — Teaching Framework

**Subject Lines:**
- The [X]-step method that changed everything
- {first_name}, try this approach
- Most people get this wrong (here's the fix)

**Email Body:**

```
Hey {first_name},

Let me share something that took me years to figure out.

When it comes to [topic], most people [common mistake]. I used to do the same thing.

Then I discovered this simple framework:

**Step 1: [Action]**
[Brief explanation — 1-2 sentences]

**Step 2: [Action]**
[Brief explanation — 1-2 sentences]

**Step 3: [Action]**
[Brief explanation — 1-2 sentences]

The difference? [Specific result or transformation]

Try it this week and let me know how it goes.

{sender_name}

P.S. If you want to go deeper on this, I cover it extensively in {offer_name}. More on that soon.
```

**Systeme.io Tags:** `nurture_sequence`, `content_engaged`
**Segment Note — New Lead:** Use as email 3-4 in sequence
**Segment Note — Warm Lead:** Can be sent as standalone value email
**Segment Note — Inactive:** Include curiosity hook in subject line

---

### 2B. Story Email — Personal Experience

**Subject Lines:**
- The day I almost gave up
- I made this mistake so you don't have to
- Nobody tells you this part...

**Email Body:**

```
Hey {first_name},

I wasn't always where I am now.

[1-2 paragraphs about your journey, struggle, or turning point]

The lesson? [Core insight in one sentence]

I share this because I know what it's like to be where you are. The doubt, the overwhelm, the wondering if it's even possible.

It is possible. And you don't have to figure it out alone.

That's exactly why I created {offer_name} — so you have a clearer path than I did.

[CTA BUTTON: Learn About {offer_name}]

You've got this.

{sender_name}
```

**Systeme.io Tags:** `story_email_sent`, `nurture_sequence`
**Segment Note — All Segments:** Stories build trust. Use early for new leads, mid-sequence for warm leads.

---

### 2C. Social Proof Email — Testimonial Focus

**Subject Lines:**
- {first_name}, see what [Client Name] achieved
- "I didn't think it would work..." — here's what happened
- Real results from real people

**Email Body:**

```
Hey {first_name},

I want you to meet [Client/Customer Name].

When they first came to me, they were [struggling with specific problem]. Sound familiar?

Here's what they said:

> "[Testimonial quote — 2-3 sentences about transformation]"

Now? [Specific result they achieved]

The best part? They're not special. They just took action and followed the process.

{offer_name} gives you the same roadmap.

[CTA BUTTON: See How {offer_name} Works]

Your success story could be next.

{sender_name}
```

**Systeme.io Tags:** `social_proof_sent`
**Segment Note — Warm Lead:** Highly effective for leads considering purchase
**Segment Note — New Lead:** Introduce after initial value emails
**Segment Note — Inactive:** Lead with curiosity, e.g., "This success story might surprise you"

---

### 2D. FAQ / Objection Handler Email

**Subject Lines:**
- The #1 question I get about {offer_name}
- "But what if it doesn't work for me?"
- Let me address the elephant in the room

**Email Body:**

```
Hey {first_name},

I get this question a lot:

**"[Common objection or question]"**

Fair question. Here's my honest answer:

[2-3 paragraphs addressing the objection directly, with evidence or reasoning]

The truth is, [reframe or reassurance].

If you're on the fence, I get it. Big decisions deserve careful thought.

But here's what I'd ask yourself: what's the cost of staying where you are?

When you're ready, I'm here.

[CTA BUTTON: Explore {offer_name}]

{sender_name}

P.S. Still have questions? Hit reply — I answer every email personally.
```

**Systeme.io Tags:** `objection_email_sent`
**Segment Note — Warm Lead:** Critical email for leads showing interest but not converting

---

### 2E. Quick Tip Email — Micro Value

**Subject Lines:**
- 60-second tip for {first_name}
- Try this today (takes 5 minutes)
- Quick win inside

**Email Body:**

```
Hey {first_name},

Here's a quick tip you can use today:

**[Actionable tip in 1-2 sentences]**

Why it works: [Brief explanation]

That's it. No long lesson today — just something you can implement in the next 5 minutes.

Let me know if you try it.

{sender_name}

P.S. Want more strategies like this? {offer_name} is packed with them. [Learn more →]
```

**Systeme.io Tags:** `quick_tip_sent`
**Segment Note — All Segments:** Great for maintaining engagement without overwhelm

---

## 3. Discovery Call CTAs

### 3A. Discovery Call Invitation — Soft Approach

**Subject Lines:**
- Can we talk, {first_name}?
- Got 15 minutes this week?
- Let's figure out your next step together

**Email Body:**

```
Hey {first_name},

I've noticed you've been engaging with my content, and I'd love to connect with you directly.

I'm opening up a few spots this week for a quick discovery call — no pitch, no pressure, just a real conversation about where you are and where you want to be.

In 15-20 minutes, we'll:
• Identify your biggest roadblock right now
• Map out a clear next step (regardless of whether we work together)
• Answer any questions you have about [topic or offer]

These spots fill up fast, so grab one while they're available:

[CTA BUTTON: Book Your Free Discovery Call]

Looking forward to meeting you.

{sender_name}

P.S. Even if now isn't the right time, I encourage you to book a slot. A little clarity can go a long way.
```

**Systeme.io Tags:** `discovery_invite_sent`, `warm_lead`
**Calendar Integration:** Link to systeme.io calendar or Calendly
**Segment Note — Warm Lead:** Ideal timing after 3-5 nurture emails

---

### 3B. Discovery Call Invitation — Direct Approach

**Subject Lines:**
- {first_name}, let's talk about {offer_name}
- Ready to take the next step?
- Your invitation to work together

**Email Body:**

```
{first_name},

I'll keep this short.

You've been following along for a while now. You've seen the strategies, the results, the testimonials.

At some point, information isn't the problem — implementation is.

That's where I come in.

I'm offering a free discovery call to see if {offer_name} is the right fit for you. No obligation, no hard sell — just an honest conversation.

On the call, we'll:
• Review where you are now vs. where you want to be
• Identify what's actually holding you back
• Determine if {offer_name} is the right solution (and if it's not, I'll tell you)

[CTA BUTTON: Schedule Your Discovery Call]

Spots are limited to [X] calls this week.

Talk soon,
{sender_name}
```

**Systeme.io Tags:** `discovery_invite_direct`, `high_intent`
**Segment Note — Warm Lead:** Use for highly engaged leads ready for conversion

---

### 3C. Discovery Call Reminder — Pre-Call

**Subject Lines:**
- See you tomorrow, {first_name}
- Quick reminder: Our call is coming up
- Don't forget: We're meeting soon

**Email Body:**

```
Hey {first_name},

Just a quick reminder that we have a discovery call scheduled:

**Date:** [Date]
**Time:** [Time + Timezone]
**Link:** [Meeting link]

To make the most of our time, come prepared to share:
• Your current situation and challenges
• Your goals for the next 90 days
• Any specific questions you want answered

I'm looking forward to connecting with you.

See you soon,
{sender_name}

P.S. Need to reschedule? No worries — reply to this email and we'll find a new time.
```

**Systeme.io Tags:** `call_reminder_sent`
**Automation Trigger:** 24 hours before scheduled call

---

### 3D. Discovery Call — No-Show Follow-Up

**Subject Lines:**
- We missed you, {first_name}
- Everything okay?
- Let's reschedule

**Email Body:**

```
Hey {first_name},

I had our call on the calendar but didn't see you — hope everything is alright!

Life happens, I completely understand.

If you still want to connect, I'm happy to reschedule. Just pick a new time that works:

[CTA BUTTON: Reschedule Your Call]

And if something has changed and you're no longer interested, that's okay too — just let me know so I can update my records.

Either way, I'm here when you're ready.

{sender_name}
```

**Systeme.io Tags:** `no_show`, `reschedule_sent`
**Automation Trigger:** 1 hour after missed call

---

## 4. Drip Reminders

### 4A. Offer Announcement — Launch Email

**Subject Lines:**
- {first_name}, it's finally here
- Doors are now open: {offer_name}
- You've been waiting for this...

**Email Body:**

```
{first_name},

The wait is over.

{offer_name} is officially open — and I couldn't be more excited to share it with you.

**Here's what you get:**

✓ [Key component/module #1]
✓ [Key component/module #2]
✓ [Key component/module #3]
✓ [Key component/module #4]

**Plus these bonuses:**
🎁 {bonus} (valued at $[X])
🎁 [Additional bonus #2]

**But here's the thing:**

This offer is only available until {deadline}. After that, [consequence: price increases / doors close / bonuses expire].

[CTA BUTTON: Get {offer_name} Now]

I designed this specifically for people like you — people who are ready to [achieve outcome].

Let's do this.

{sender_name}

P.S. Have questions? Reply to this email. I'm here to help you decide if this is right for you.
```

**Systeme.io Tags:** `launch_email_sent`, `offer_announced`
**Segment Note — New Lead:** Ensure they've received at least 2-3 nurture emails first
**Segment Note — Warm Lead:** Primary target for launch emails

---

### 4B. Deadline Reminder — 72 Hours Left

**Subject Lines:**
- {first_name}, 3 days left
- The clock is ticking on {offer_name}
- 72 hours — then it's gone

**Email Body:**

```
Hey {first_name},

Quick heads up: you have 72 hours left to join {offer_name}.

After {deadline}, [consequence — price increases, bonuses disappear, doors close].

If you've been thinking about it, now's the time to decide.

Here's what you'll miss if you wait:

❌ {bonus}
❌ [Exclusive component/access]
❌ [Current pricing/offer]

I don't want you to look back and wish you'd taken action.

[CTA BUTTON: Join {offer_name} Before It's Too Late]

Still have questions? Let's talk: [calendar_link]

{sender_name}
```

**Systeme.io Tags:** `72hr_reminder_sent`
**Automation Trigger:** 72 hours before deadline

---

### 4C. Deadline Reminder — 24 Hours Left

**Subject Lines:**
- {first_name}, this ends tomorrow
- FINAL DAY: {offer_name}
- 24 hours left — are you in?

**Email Body:**

```
{first_name},

This is your 24-hour warning.

Tomorrow at [specific time], {offer_name} closes — and with it, your chance to [achieve outcome] at this price.

I've loved having you on this journey. And I'd love even more to work with you directly inside {offer_name}.

Here's what's waiting for you:
• [Quick benefit recap #1]
• [Quick benefit recap #2]
• [Quick benefit recap #3]
• BONUS: {bonus}

[CTA BUTTON: Secure Your Spot Now]

If it's not the right time, no hard feelings. I'll still be here with free content and support.

But if you're ready to [transformation], this is your moment.

{sender_name}

P.S. Remember — after {deadline}, [consequence]. Don't let this slip away.
```

**Systeme.io Tags:** `24hr_reminder_sent`, `urgency_email`
**Automation Trigger:** 24 hours before deadline

---

### 4D. Deadline Reminder — Final Hours

**Subject Lines:**
- {first_name}, 3 HOURS LEFT
- Last chance: {offer_name} closes tonight
- This is it.

**Email Body:**

```
{first_name} —

This is it.

{offer_name} closes in just a few hours.

I'm not going to repeat everything — you know what's inside, you know the value, you know what's possible.

The only question left: are you ready to take action?

[CTA BUTTON: Join {offer_name} — Final Hours]

After {deadline}, this offer is gone. I can't make exceptions.

If you've been waiting for a sign, this is it.

{sender_name}
```

**Systeme.io Tags:** `final_hours_sent`, `closing_email`
**Automation Trigger:** 3-6 hours before deadline

---

### 4E. Post-Deadline — Doors Closed

**Subject Lines:**
- {offer_name} is now closed
- We've closed the doors (for now)
- What's next, {first_name}

**Email Body:**

```
Hey {first_name},

Just a quick note: {offer_name} is officially closed.

If you missed it, I understand — timing is everything, and sometimes it's just not the right moment.

Here's what you can do now:

1. **Stay on the list** — I'll let you know when doors open again (no guarantee on timing or price)
2. **Keep learning** — I'll continue sending valuable content your way
3. **Reach out** — If circumstances change, reply and let me know

I'm grateful you're here, whether you joined this round or not.

More good stuff coming soon.

{sender_name}

P.S. Want to be first in line next time? Reply with "WAITLIST" and I'll add you to the priority notification list.
```

**Systeme.io Tags:** `closed_email_sent`, `non_buyer`
**Segment Action:** Move non-buyers to nurture sequence or waitlist

---

## 5. Re-Engagement Emails (Inactive Segment)

### 5A. Re-Engagement — Check-In

**Subject Lines:**
- {first_name}, you still there?
- Did I do something wrong?
- Haven't heard from you in a while

**Email Body:**

```
Hey {first_name},

I noticed you haven't opened my emails in a while, and I wanted to check in.

No guilt trip — I get it. Inboxes are overwhelming and life gets busy.

But I'm curious: are you still interested in [topic/outcome]?

If yes, hit reply and let me know what you're struggling with. I'd love to help.

If no, that's okay too. You can unsubscribe below — no hard feelings.

But if you're still in, I've got some great stuff planned. Don't miss out.

{sender_name}

P.S. As a welcome back gift, here's [exclusive resource or tip]. Hope it helps.
```

**Systeme.io Tags:** `reengagement_sent`, `inactive_segment`
**Automation Trigger:** After 14-21 days of no opens/clicks

---

### 5B. Re-Engagement — Value Bomb

**Subject Lines:**
- {first_name}, I made this for you
- Free gift inside (no catch)
- Thought you might find this useful

**Email Body:**

```
Hey {first_name},

I know it's been a while, so I wanted to drop something valuable in your inbox — no pitch, no catch.

Here's [free resource/tip/template] that's been helping a lot of people with [specific problem]:

[CTA BUTTON: Get Your Free [Resource]]

Use it, share it, whatever helps.

If you ever want to dive deeper, you know where to find me.

{sender_name}
```

**Systeme.io Tags:** `value_bomb_sent`, `reengagement_attempt`
**Segment Note — Inactive:** Low-pressure approach to rebuild engagement

---

### 5C. Re-Engagement — Last Chance to Stay

**Subject Lines:**
- Should I remove you from the list?
- Last email from me (unless...)
- Time to say goodbye?

**Email Body:**

```
Hey {first_name},

I'll keep this simple.

I haven't heard from you in a while, and I don't want to clutter your inbox if you're no longer interested.

So here's the deal:

**Click below if you want to stay on the list:**

[CTA BUTTON: Yes, Keep Me Subscribed!]

If I don't hear from you in the next 48 hours, I'll remove you from the list. No hard feelings — I only want to email people who actually want to hear from me.

Thanks for being here, however long it's been.

{sender_name}
```

**Systeme.io Tags:** `final_reengagement`, `list_cleanup`
**Automation Trigger:** After 2 re-engagement attempts with no response
**Post-Action:** Remove from list if no click within 48 hours

---

## Systeme.io Implementation Guide

### Recommended Automation Structure

**Welcome Sequence (New Leads):**
```
Day 0: Welcome Email (1A or 1B)
Day 1: Value Email (2A or 2E)
Day 3: Story Email (2B)
Day 5: Social Proof (2C)
Day 7: Discovery Call Invite (3A) or Soft Pitch
```

**Nurture Sequence (Warm Leads):**
```
Weekly: Rotate between 2A, 2B, 2C, 2D, 2E
Monthly: Discovery Call Invitation (3A or 3B)
```

**Launch Sequence (Active Leads):**
```
Day 0: Offer Announcement (4A)
Day 2: Value + Testimonial
Day 4: FAQ/Objection (2D)
Day 5: 72-Hour Reminder (4B)
Day 6: 24-Hour Reminder (4C)
Day 7 (morning): Final Hours (4D)
Day 7 (post-deadline): Doors Closed (4E)
```

**Re-Engagement Sequence (Inactive):**
```
Day 0: Check-In (5A)
Day 3: Value Bomb (5B)
Day 7: Last Chance (5C)
Day 9: Remove if no engagement
```

### Tag Taxonomy

| Category | Tags |
|----------|------|
| **Lead Status** | `new_lead`, `warm_lead`, `hot_lead`, `inactive`, `non_buyer`, `customer` |
| **Engagement** | `email_opened`, `link_clicked`, `replied`, `highly_engaged` |
| **Interest** | `interested_{offer}`, `viewed_sales_page`, `abandoned_checkout` |
| **Objections** | `objection_price`, `objection_time`, `objection_doubt` |
| **Actions** | `discovery_booked`, `discovery_completed`, `no_show`, `purchased` |

### Custom Fields

- `first_name` — Contact's first name
- `lead_source` — Where they opted in
- `lead_magnet` — Which freebie they downloaded
- `interested_offer` — Which offer they've shown interest in
- `discovery_call_date` — Scheduled call date/time

---

## Variables Quick Reference

| Variable | Description | Example |
|----------|-------------|---------|
| `{first_name}` | Subscriber's first name | Sarah |
| `{offer_name}` | Product/program name | Digital Growth Academy |
| `{bonus}` | Bonus item name | Quick-Start Implementation Guide |
| `{deadline}` | Offer deadline | Friday at midnight EST |
| `{calendar_link}` | Booking page URL | https://calendly.com/yourname |
| `{sender_name}` | Your name/signature | Alex |
| `{company_name}` | Business name | GrowthLab Inc. |

---

## Usage Notes

- **Personalization:** Always use `{first_name}` in subject lines and greetings when possible
- **Testing:** A/B test subject lines — the options provided are starting points
- **Timing:** Send emails between 9-11 AM or 7-9 PM in subscriber's timezone for best open rates
- **Frequency:** New leads can handle daily emails for first week; warm leads prefer 2-3x weekly
- **Mobile:** 60%+ of emails are read on mobile — keep paragraphs short
- **Compliance:** Always include unsubscribe link and physical address per CAN-SPAM/GDPR

---

**Category:** Email Marketing / Funnel Copy
**Complexity:** Standard to Advanced
**Output Type:** Email Sequences, Automation Copy
**Platform:** Systeme.io (adaptable to other ESPs)
