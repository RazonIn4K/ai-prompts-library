# ManyChat Conversational Copy Snippets

**CATEGORY:** Marketing Automation / Chatbot Copy
**PURPOSE:** Ready-to-use conversational copy snippets for ManyChat flows with CTA buttons and tags
**VARIABLES:** `{lead_name}`, `{product_name}`, `{price}`, `{bonus_name}`, `{deadline}`, `{whatsapp_link}`, `{testimonial_name}`, `{result_achieved}`
**TONE:** Friendly mentor, warm, encouraging, conversational, no pressure

---

## 1. Keyword Response (Entry Point)

### Trigger: User types keyword (e.g., "READY", "START", "INFO")

```
Hey {lead_name}!

So glad you reached out. You're in the right place.

I'm here to help you [achieve specific outcome] without the overwhelm.

Quick question before we dive in...
```

**Button Options:**
- `[Yes, tell me more!]` → Tag: `interested_lead`
- `[Just browsing]` → Tag: `cold_lead`

---

### Alternative Keyword Response (High Energy)

```
{lead_name}! You just made a great decision.

Most people scroll past opportunities like this... but not you.

Ready to see what's possible?
```

**Button:**
- `[Show me!]` → Tag: `engaged_lead`

---

## 2. Welcome Message (New Subscriber Flow)

### First Contact Welcome

```
Welcome to the family, {lead_name}!

I'm genuinely excited you're here. This is where your [transformation journey] begins.

Here's what you can expect from me:
 Tips that actually work (no fluff)
 Real strategies you can use TODAY
 Support when you get stuck

One quick thing — what's your biggest challenge right now with [topic]?
```

**Button Options:**
- `[Getting started]` → Tag: `beginner`
- `[Staying consistent]` → Tag: `intermediate`
- `[Scaling up]` → Tag: `advanced`

---

### Warm Welcome (After Opt-in)

```
Hey {lead_name}, welcome aboard!

You're now officially part of a community of [X] people committed to [outcome].

Here's your first win: I've got a free resource that's helped hundreds of people [specific result].

Want me to send it over?
```

**Button Options:**
- `[Yes please!]` → Send freebie → Tag: `lead_magnet_received`
- `[Maybe later]` → Tag: `delayed_interest`

---

## 3. Waitlist Pitch

### Building Anticipation

```
{lead_name}, something big is coming...

I've been working on {product_name} — and honestly? It's my best work yet.

This is for you if:
 You're tired of [pain point 1]
 You want [desired outcome] without [common frustration]
 You're ready to finally [transformation]

Spots will be limited when doors open.

Want first dibs + an exclusive bonus only for waitlist members?
```

**Button Options:**
- `[Yes, save my spot!]` → Tag: `waitlist_member`, `vip_lead`
- `[Tell me more first]` → Tag: `waitlist_curious`

---

### Waitlist Confirmation

```
You're on the list, {lead_name}!

Here's what happens next:
1. I'll message you FIRST when doors open
2. You'll get the waitlist-only bonus ({bonus_name})
3. You'll have early access before everyone else

Keep an eye on your messages — I don't want you to miss this!
```

**Button:**
- `[Got it!]` → Tag: `waitlist_confirmed`

---

## 4. Nurture Sequence

### 4A. Quick Tips

```
Hey {lead_name}! Quick tip for you today...

Most people think [common misconception].

But here's what actually works:

**[Actionable tip in 1-2 sentences]**

Try this today and let me know how it goes!
```

**Button Options:**
- `[Great tip!]` → Tag: `engaged`
- `[Need more help]` → Trigger support flow

---

### 4B. Testimonial Share

```
{lead_name}, I wanted to share something with you...

{testimonial_name} was exactly where you are right now.

They said: "[Short testimonial quote about struggle → transformation]"

And now? {result_achieved}.

This is possible for you too.

What's holding you back right now?
```

**Button Options:**
- `[Time]` → Tag: `objection_time`
- `[Money]` → Tag: `objection_money`
- `[Not sure it'll work for me]` → Tag: `objection_doubt`
- `[Nothing, I'm ready!]` → Tag: `hot_lead`

---

### 4C. Mini Lesson

```
{lead_name}, let's talk about [topic]...

Here's the 3-step framework I use with every client:

**Step 1:** [First action]
**Step 2:** [Second action]
**Step 3:** [Third action]

Most people skip Step 2 — and that's why they stay stuck.

Want me to break down Step 2 in more detail?
```

**Button Options:**
- `[Yes, tell me more]` → Send detailed content → Tag: `high_engagement`
- `[I've got this]` → Tag: `self_sufficient`

---

### 4D. Mindset Nudge

```
Quick mindset check, {lead_name}...

I know sometimes it feels like everyone else has it figured out.

Truth? They don't. They just started before they felt ready.

You've already taken the first step by being here.

What's one small action you can take TODAY toward [goal]?
```

**Button Options:**
- `[I'll do it!]` → Tag: `action_taker`
- `[I need help deciding]` → Trigger support flow

---

## 5. Payment Nudges

### 5A. Soft Reminder

```
Hey {lead_name}! Just checking in...

I noticed you were interested in {product_name} but haven't joined yet.

No pressure at all — but I wanted to make sure you didn't miss anything.

Is there something I can help clarify?
```

**Button Options:**
- `[What's included?]` → Send benefits breakdown
- `[Is it right for me?]` → Trigger qualification questions
- `[What's the price?]` → Send pricing details → Tag: `price_aware`
- `[I'm ready to join!]` → Send payment link → Tag: `ready_to_buy`

---

### 5B. Value Stack Reminder

```
{lead_name}, quick recap of what you'll get with {product_name}:

 [Main deliverable 1] (Value: $X)
 [Main deliverable 2] (Value: $X)
 [Main deliverable 3] (Value: $X)
 BONUS: {bonus_name} (Value: $X)

Total value: $XXX

Your investment today: Only {price}

This is the lowest price I've ever offered.

Ready to lock it in?
```

**Button:**
- `[Yes, I'm in!]` → Send payment link → Tag: `converted`
- `[I have questions]` → Trigger FAQ flow

---

### 5C. Last Chance (Urgency)

```
{lead_name}, I wanted to give you a heads up...

{product_name} at this price closes in [X hours].

After that, the price goes up to [higher price] — no exceptions.

I really don't want you to miss this because [reason why it matters for them].

This is your last chance at this price.
```

**Button Options:**
- `[Secure my spot now]` → Send payment link → Tag: `converted_urgency`
- `[I'll wait for next time]` → Tag: `lost_lead_price`

---

### 5D. Post-Purchase Abandoned Cart

```
Hey {lead_name}! I noticed you started signing up for {product_name} but didn't finish.

Sometimes life gets in the way — totally get it!

Your spot is still saved, but I can only hold it for [X more hours].

Want me to send you the link to finish signing up?
```

**Button Options:**
- `[Yes, send the link]` → Send payment link → Tag: `cart_recovery`
- `[I changed my mind]` → Trigger objection flow → Tag: `cart_abandoned`

---

## 6. WhatsApp Invite

### Community Invitation

```
{lead_name}! Got something special for you...

I've created a private WhatsApp community where I share:

 Exclusive tips I don't post anywhere else
 Behind-the-scenes strategies
 Direct access to ask me questions
 First announcements about new offers

It's completely free and the vibes are amazing.

Want in?
```

**Button:**
- `[Join the Community]` → Open URL: `{whatsapp_link}` → Tag: `whatsapp_member`
- `[Not right now]` → Tag: `whatsapp_declined`

---

### VIP WhatsApp Group (Buyers Only)

```
Welcome to the inner circle, {lead_name}!

As a {product_name} member, you get access to our private WhatsApp group.

This is where:
 I answer questions personally
 Members share wins and support each other
 You get bonus content and early access

Click below to join — introduce yourself when you get there!
```

**Button:**
- `[Join VIP WhatsApp]` → Open URL: `{whatsapp_link}` → Tag: `vip_whatsapp_joined`

---

## 7. Countdown Reminders

### 48 Hours Left

```
{lead_name}, 48 hours left...

Doors to {product_name} close on {deadline}.

If you've been thinking about joining, now's the time to decide.

Here's what one member said: "[Quick testimonial]"

That could be you in a few weeks.

What's stopping you?
```

**Button Options:**
- `[Nothing — I'm ready!]` → Send payment link
- `[I still have questions]` → Trigger FAQ flow
- `[It's not the right time]` → Tag: `not_now`

---

### 24 Hours Left

```
FINAL DAY, {lead_name}!

{product_name} closes tomorrow at [time].

I've loved having you here, and I'd love even more to work with you inside.

But if it's not the right fit, no hard feelings — I'll still be here with free tips.

Last chance to join:
```

**Button:**
- `[Join {product_name}]` → Send payment link → Tag: `24hr_convert`

---

### 1 Hour Left

```
{lead_name} — 1 HOUR LEFT!

This is it. After [time], {product_name} closes and the price goes up.

No pressure, just want to make sure you don't regret missing this.

If you're ready, the link is below.

If not, I'll catch you next time!
```

**Button:**
- `[I'm in — let's go!]` → Send payment link → Tag: `last_hour_convert`

---

### Doors Closed

```
Hey {lead_name}...

{product_name} just closed.

If you missed it, don't worry — I'll let you know when doors open again.

In the meantime, stick around! I've got lots of free value coming your way.

What topic would you love me to cover next?
```

**Button Options:**
- `[Topic 1]` → Tag: `interest_topic1`
- `[Topic 2]` → Tag: `interest_topic2`
- `[Topic 3]` → Tag: `interest_topic3`

---

## 8. FAQ Responses

### FAQ: What's Included?

```
Great question, {lead_name}!

Here's everything you get with {product_name}:

**Core Content:**
 [Module/Feature 1]
 [Module/Feature 2]
 [Module/Feature 3]

**Bonuses:**
 {bonus_name}
 [Additional bonus]

**Support:**
 [Type of support offered]
 [Access duration]

Any other questions?
```

**Button Options:**
- `[How much is it?]` → Trigger pricing response
- `[Is it right for me?]` → Trigger fit assessment
- `[I'm ready to join!]` → Send payment link

---

### FAQ: How Much Does It Cost?

```
{lead_name}, here's the investment breakdown:

{product_name}: {price}

You can pay:
 In full (best value)
 [Payment plan option if available]

And remember, you're getting $XXX in value for just {price}.

Plus, there's a [guarantee type] guarantee — so there's zero risk.

Ready to get started?
```

**Button Options:**
- `[Yes, sign me up!]` → Send payment link
- `[Tell me about the guarantee]` → Trigger guarantee explanation
- `[I need to think about it]` → Tag: `price_hesitant`

---

### FAQ: Is This Right For Me?

```
Good question, {lead_name}. Let me help you figure that out!

{product_name} is PERFECT for you if:
 You're [ideal customer trait 1]
 You want [desired outcome]
 You're ready to [commitment required]

It's probably NOT for you if:
 You're looking for [wrong expectation]
 You're not willing to [required action]

Which sounds more like you?
```

**Button Options:**
- `[Sounds perfect for me!]` → Tag: `qualified_lead` → Send to payment
- `[I'm not sure yet]` → Trigger more questions
- `[Probably not for me]` → Tag: `unqualified` → Send to nurture

---

### FAQ: What If It Doesn't Work?

```
I hear you, {lead_name}. That's a valid concern.

Here's the thing:

1. **It's proven** — [X] people have gotten results with this
2. **It's supported** — You're not doing this alone
3. **It's guaranteed** — [Guarantee details]

If you show up and do the work, I'm confident you'll see results.

And if not? [Guarantee/refund policy].

What else can I help you with?
```

**Button Options:**
- `[I'm convinced — let's do this!]` → Send payment link
- `[Show me testimonials]` → Trigger testimonial flow
- `[I need more time]` → Tag: `needs_nurturing`

---

### FAQ: When Does It Start?

```
{lead_name}, here's the timeline:

**Access:** [Immediate / On specific date]
**Duration:** [How long they have access]
**Time commitment:** [Expected hours per week]

You can go at your own pace — no pressure to finish by a certain date.

Ready to get started?
```

**Button:**
- `[Let's go!]` → Send payment link
- `[More questions]` → Trigger main FAQ menu

---

## ManyChat Implementation Notes

### Recommended Tags to Create:
- `engaged_lead`, `hot_lead`, `cold_lead`
- `waitlist_member`, `waitlist_confirmed`
- `objection_time`, `objection_money`, `objection_doubt`
- `beginner`, `intermediate`, `advanced`
- `whatsapp_member`, `vip_whatsapp_joined`
- `converted`, `cart_abandoned`, `cart_recovery`
- `qualified_lead`, `unqualified`

### Recommended Custom Fields:
- `lead_name` (First Name)
- `lead_stage` (Awareness → Interest → Decision → Action)
- `product_interest` (Which product they're interested in)
- `last_engagement_date`

### Flow Structure Suggestions:
1. **Entry Flow:** Keyword → Welcome → Segmentation
2. **Nurture Flow:** 3-5 messages over 7-14 days
3. **Sales Flow:** Value → Objection handling → Urgency → Close
4. **Post-Purchase Flow:** Confirmation → Onboarding → WhatsApp invite

---

## Example Usage

**Input Variables:**
```
{lead_name} = "Sarah"
{product_name} = "Instagram Growth Accelerator"
{price} = "$197"
{bonus_name} = "Content Calendar Template Pack"
{deadline} = "Friday at midnight"
{whatsapp_link} = "https://chat.whatsapp.com/xyz123"
{testimonial_name} = "Marcus"
{result_achieved} = "grew from 500 to 10K followers in 90 days"
```

**Sample Welcome Output:**
```
Welcome to the family, Sarah!

I'm genuinely excited you're here. This is where your Instagram growth journey begins.

Here's what you can expect from me:
 Tips that actually work (no fluff)
 Real strategies you can use TODAY
 Support when you get stuck

One quick thing — what's your biggest challenge right now with Instagram?

[Getting started] [Staying consistent] [Scaling up]
```
