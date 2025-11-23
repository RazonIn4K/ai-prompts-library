# AI Receptionist Dialogue Blocks

## Purpose
Reusable conversation flows and dialogue templates for AI-powered phone and chat receptionists across high-volume service industries. Designed for use with voice AI platforms (Bland.ai, Vapi, Retell) and ElevenLabs voice synthesis.

## Industries Covered
- **Roofing** – Storm damage, inspections, estimates
- **HVAC** – Repairs, maintenance, installations
- **Dental** – Cleanings, procedures, emergencies
- **MedSpa** – Aesthetic treatments, consultations
- **Legal** – Case intake, consultations, document requests

## Voice Configuration Notes

### ElevenLabs Voice Slots
| Industry | Recommended Voice Style | ElevenLabs Model | Notes |
|----------|------------------------|------------------|-------|
| Roofing | Warm, confident male/female | `eleven_turbo_v2` | Professional but approachable |
| HVAC | Calm, reassuring | `eleven_turbo_v2` | Emphasize urgency understanding |
| Dental | Friendly, gentle | `eleven_multilingual_v2` | Soft tone for anxious callers |
| MedSpa | Sophisticated, warm | `eleven_multilingual_v2` | Upscale, consultative feel |
| Legal | Professional, empathetic | `eleven_turbo_v2` | Authoritative yet compassionate |

**Stability:** 0.5–0.7 (balanced natural variation)
**Similarity Boost:** 0.75+ (consistent voice identity)
**Style:** 0.3–0.5 (subtle expressiveness)

---

## Intent 1: Greeting

### Universal Greeting Framework
```
[PAUSE 0.3s]
"Thank you for calling {business_name}, this is {agent_name}. How can I help you today?"
```

### Industry-Specific Greetings

#### Roofing
```
"Thank you for calling {business_name}, your local roofing experts. This is {agent_name}.
Are you calling about storm damage, a roof inspection, or something else I can help with?"
```

**Variables:** `{business_name}`, `{agent_name}`, `{service_area}`

#### HVAC
```
"Thanks for calling {business_name}. This is {agent_name}.
Is your call about a repair, maintenance, or a new system? I'm here to help."
```

**After-hours variant:**
```
"Thank you for calling {business_name} after hours. This is {agent_name}, our virtual assistant.
If this is a heating or cooling emergency, I can help get a technician dispatched right away.
What's going on with your system?"
```

#### Dental
```
"Good {time_of_day}, thank you for calling {practice_name}. This is {agent_name}.
Are you an existing patient or is this your first time calling us?"
```

**Emergency branch:**
```
"I understand dental emergencies can be stressful. Let me help you right away.
Can you describe what's happening?"
```

#### MedSpa
```
"Thank you for calling {spa_name}, where beauty meets wellness. This is {agent_name}.
Are you calling to book a treatment, ask about our services, or check on an existing appointment?"
```

#### Legal
```
"Thank you for calling the Law Offices of {firm_name}. This is {agent_name}.
How may I direct your call today?"
```

**New client variant:**
```
"Thank you for calling {firm_name}. This is {agent_name}.
Are you calling about a new legal matter, or are you an existing client?"
```

---

## Intent 2: Qualification

### Universal Qualification Framework
```
"To make sure I connect you with the right person and give you accurate information,
I have a few quick questions. This will only take a moment."
```

### Roofing Qualification

**Lead Scoring Questions:**
```
Q1: "Is this for your home or a commercial property?"
    → Residential = standard flow | Commercial = flag for commercial team

Q2: "What type of roofing issue are you experiencing?
     For example, a leak, storm damage, or are you looking for a new roof?"
    → Leak/Damage = urgent | New roof = project quote

Q3: "When did you first notice the issue?"
    → Within 48 hours = high priority | Older = standard

Q4: "Do you have homeowner's insurance, and have you filed a claim?"
    → Insurance = larger project potential

Q5: "What's your zip code so I can confirm we service your area?"
    → Validate service area
```

**Qualified Lead Response:**
```
"Great, we absolutely service {city/zip}. Based on what you've described,
one of our roofing specialists should take a look.
Would you prefer a morning or afternoon appointment?"
```

### HVAC Qualification

**Urgency Assessment:**
```
Q1: "Is your heating or air conditioning completely not working,
     or is it running but not performing correctly?"
    → Not working = emergency | Underperforming = standard

Q2: "Are there any vulnerable individuals in the home,
     like elderly family members or young children?"
    → Yes = priority dispatch

Q3: "What type of system do you have – central air, a heat pump, or a furnace?"
    → Routes to appropriate technician

Q4: "How old is your current system, if you know?"
    → 10+ years = replacement discussion opportunity

Q5: "Are you the homeowner or renting?"
    → Renter = may need landlord authorization
```

**Emergency Response:**
```
"I can hear this is urgent. Let me get a technician scheduled for you right away.
We have availability {next_available_slot}. Does that work for you?"
```

### Dental Qualification

**New Patient Intake:**
```
Q1: "Have you visited our office before?"
    → New = full intake | Existing = pull up record

Q2: "What brings you in today – is it a routine cleaning,
     a specific concern, or are you experiencing pain?"
    → Pain = same-day if possible

Q3: "Do you currently have dental insurance?"
    → Yes = collect carrier info | No = discuss payment options

Q4: "Is there a particular dentist you'd like to see,
     or would you like the next available appointment?"

Q5: "Any medical conditions or medications we should know about before your visit?"
```

**Pain/Emergency Branch:**
```
"I'm sorry you're in pain. Let me see what we can do to get you in quickly.
On a scale of 1 to 10, how would you rate your discomfort right now?"
```

### MedSpa Qualification

**Treatment Interest:**
```
Q1: "What treatment or service are you interested in learning about?"
    → Route to appropriate specialist

Q2: "Have you had this type of treatment before,
     or would this be your first time?"
    → First time = consultation recommended

Q3: "Are you hoping to address a specific concern,
     like fine lines, skin texture, or body contouring?"
    → Helps recommend treatment path

Q4: "Do you have any upcoming events you're preparing for?"
    → Timeline affects treatment plan

Q5: "How did you hear about us?"
    → Marketing attribution
```

**Consultation Offer:**
```
"Based on what you've shared, I'd recommend starting with a complimentary consultation.
Our specialists can create a personalized treatment plan just for you.
Would you prefer a weekday or weekend appointment?"
```

### Legal Qualification

**Case Intake:**
```
Q1: "What type of legal matter are you calling about?
     For example, personal injury, family law, criminal defense, or something else?"
    → Route to practice area

Q2: "When did this incident or situation occur?"
    → Statute of limitations check

Q3: "Have you spoken with any other attorneys about this matter?"
    → Competitive awareness

Q4: "Is this matter time-sensitive? For example,
     do you have a court date or deadline approaching?"
    → Urgency flag

Q5: "Briefly, can you share what happened?"
    → Open-ended for context
```

**Qualified Lead Response:**
```
"Thank you for sharing that with me. Based on what you've described,
one of our {practice_area} attorneys would be the right person to speak with.
They offer a free initial consultation. Can I schedule that for you?"
```

---

## Intent 3: Appointment Scheduling

### Universal Scheduling Framework
```
"Let me check our availability for you. Do you have a preference for
morning, afternoon, or a specific day of the week?"
```

### Scheduling Dialogue Blocks

**Offer Options (2-choice method):**
```
"I have availability on {day_1} at {time_1} or {day_2} at {time_2}.
Which works better for you?"
```

**Confirm Details:**
```
"Perfect. I have you down for {day} at {time} with {provider/technician}.
Can I confirm the best phone number to reach you at?
And what's a good email for the confirmation?"
```

**Address/Location Collection:**
```
"And what's the service address where we'll be coming out?"
[Repeat back] "Just to confirm, that's {address}?"
```

**Appointment Confirmation:**
```
"You're all set for {day}, {date} at {time}.
You'll receive a confirmation text and email shortly.
Is there anything else I can help you with today?"
```

### Industry-Specific Scheduling

#### Roofing
```
"Our inspector can come out to assess your roof on {day} at {time}.
The inspection takes about 30 to 45 minutes.
Does someone need to be home, or can we access the property?"
```

#### HVAC
```
"I can get a technician out to you on {day} between {time_window}.
We'll give you a call about 30 minutes before arrival.
Will someone over 18 be home to let them in?"
```

**Same-Day Dispatch:**
```
"Good news – we have a technician who can be there today between {time_window}.
I'll need to collect a credit card to hold the appointment.
There's no charge unless you approve any work. Does that work for you?"
```

#### Dental
```
"I have an opening with Dr. {dentist_name} on {day} at {time}.
For new patients, we ask that you arrive 15 minutes early to complete paperwork.
Should I send you the forms ahead of time?"
```

**Recall/Hygiene Scheduling:**
```
"It looks like you're due for your 6-month cleaning.
I have availability with {hygienist} on {day} at {time}.
Would you like me to book that for you?"
```

#### MedSpa
```
"I can book your consultation with {specialist} on {day} at {time}.
The consultation takes about 30 minutes, and you'll have a chance to
discuss your goals and see what treatments might be right for you.
Should I reserve that for you?"
```

**Treatment Appointment:**
```
"For your {treatment} appointment, I have {day} at {time} available.
Just a reminder, we recommend avoiding sun exposure and retinol products
for 48 hours before your appointment. Does that date work for you?"
```

#### Legal
```
"Attorney {attorney_name} has a consultation opening on {day} at {time}.
The initial consultation is {free/fee_amount} and typically lasts about 30 minutes.
Would you like me to schedule that?"
```

**Document Reminder:**
```
"For your consultation, please bring any relevant documents –
police reports, medical records, contracts, or correspondence related to your case.
This helps the attorney give you the best guidance."
```

---

## Intent 4: Objection Handling

### Universal Objection Framework
```
"I completely understand. Let me see if I can address that for you..."
```

### Common Objections & Responses

#### "I'm just looking for a price."

**Roofing:**
```
"I completely understand wanting to know the cost upfront.
Every roof is different, so our inspections are free and come with a detailed,
no-obligation estimate. That way, you'll have exact numbers, not guesses.
Would you like me to schedule that complimentary inspection?"
```

**HVAC:**
```
"That's a fair question. For repairs, our diagnostic fee is {amount},
which gets applied to the repair if you move forward.
For replacements, we offer free in-home estimates. Which situation applies to you?"
```

**Dental:**
```
"Our pricing depends on the specific treatment and your insurance coverage.
We'd be happy to verify your benefits before your visit so there are no surprises.
Can I get your insurance information to check that for you?"
```

**MedSpa:**
```
"Our treatments range depending on the area and your goals.
The best way to get accurate pricing is a free consultation,
where we can also discuss any specials or packages.
Would you like to book one?"
```

**Legal:**
```
"Our fee structure depends on the type of case.
For {practice_area} matters, we typically work on {contingency/hourly/flat_fee}.
The initial consultation is {free/fee} and there's no obligation.
Would you like to schedule a time to discuss your specific situation?"
```

#### "I need to talk to my spouse/partner first."

```
"Absolutely, that makes sense. Would it help if I scheduled a time
when you could both be on the call, or would you prefer to call us back?
I can also send over some information so you have it ready when you discuss."
```

#### "I'm not ready to schedule yet."

```
"No problem at all. Can I get your contact information so we can
send you some helpful information, and you can reach out when you're ready?
We're here whenever you need us."
```

**Soft close variant:**
```
"I understand. Many of our clients felt the same way before their first appointment.
Would a no-pressure consultation help you decide?
You'd get all your questions answered with zero commitment."
```

#### "I've already called other companies."

```
"Smart move – it's always good to compare. What matters most to you
in making this decision? That way, I can make sure you have
the right information about what sets us apart."
```

#### "Your reviews/price/availability doesn't work."

**Negative Review Concern:**
```
"I appreciate you doing your research. We take all feedback seriously
and use it to improve. I can tell you that {social_proof_point}.
Would you like to speak with someone about your specific situation?"
```

**Price Objection:**
```
"I hear you – cost is an important factor. We focus on quality and standing behind our work.
Many clients find that our {warranty/guarantee/value_proposition}
makes the investment worthwhile. Would you like to learn more about our {financing/payment_options}?"
```

**Scheduling Conflict:**
```
"I'm sorry those times don't work. Let me see what else I can do.
What day and time would be ideal for you?
I'll do my best to make it happen or get you on our priority list."
```

#### "I don't have time right now."

```
"Totally understand – you're busy. This will just take another minute or two.
Or, if you prefer, I can call you back at a better time.
What works for your schedule?"
```

---

## Intent 5: Outbound Follow-Up

### Universal Follow-Up Framework
```
"Hi, this is {agent_name} from {business_name}.
I'm following up on {reason_for_call}. Do you have a moment?"
```

### Follow-Up Scenarios

#### Missed Appointment Follow-Up
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
I noticed we missed you for your appointment on {date}.
I wanted to reach out and see if everything is okay,
and help you reschedule when it's convenient.
Do you have a minute?"
```

**If they answer:**
```
"No worries at all – things come up. Would you like to reschedule now?
I have availability on {day_1} or {day_2}."
```

#### Quote/Estimate Follow-Up
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
I'm calling to follow up on the {estimate_type} we sent over on {date}.
Did you have a chance to review it, and do you have any questions I can answer?"
```

**Buying signals:**
```
"Great! If you're ready to move forward, I can get you on the schedule.
What timeframe were you thinking?"
```

**Not ready:**
```
"Understood. Is there anything holding you back that I might be able to help with?
We want to make sure you have all the information you need."
```

#### Lead Re-Engagement (30-60 days cold)
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
We spoke a while back about {original_inquiry}.
I wanted to check in and see if your situation has changed
or if there's anything we can help with now."
```

#### Post-Service Follow-Up
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
I'm calling to make sure everything went well with your {service} on {date}.
How was your experience?"
```

**If positive:**
```
"That's wonderful to hear! If you have a moment, we'd really appreciate
a quick review on Google. I can text you the link.
And of course, if you need anything in the future, we're here to help."
```

**If issue reported:**
```
"I'm sorry to hear that. Let me get the details so we can make this right.
Can you tell me what happened?"
```

### Industry-Specific Follow-Ups

#### Roofing – Storm Season
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
I'm reaching out because we had some severe weather in your area recently.
Many homeowners are finding damage they didn't notice at first.
Would you like us to do a free inspection to make sure your roof is okay?"
```

#### HVAC – Seasonal Maintenance
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
As we head into {season}, I wanted to remind you about scheduling
your preventive maintenance. This helps avoid breakdowns during {hot/cold} weather.
Would you like to get on the schedule?"
```

#### Dental – Recall/Hygiene Due
```
"Hi {patient_name}, this is {agent_name} from {practice_name}.
Our records show you're due for your 6-month cleaning and checkup.
I have some openings this week and next. Would you like to schedule?"
```

#### MedSpa – Treatment Series
```
"Hi {client_name}, this is {agent_name} from {spa_name}.
I'm calling about your {treatment} series.
You're due for your next session to maintain your results.
Would you like to book your next appointment?"
```

#### Legal – Case Status
```
"Hi {client_name}, this is {agent_name} from {firm_name}.
I'm calling with an update on your case.
Is now a good time, or would you prefer we schedule a call with Attorney {name}?"
```

---

## Intent 6: Voicemail Fallback

### Universal Voicemail Framework
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
I'm calling about {reason}. Please call us back at {phone_number}.
I'll also send you a text with our details. Thanks, and we look forward to speaking with you."
```

### Voicemail Scripts by Scenario

#### First Outreach – New Lead
```
"Hi {customer_name}, this is {agent_name} calling from {business_name}.
I received your request about {service/inquiry} and wanted to connect with you.
Please give us a call back at {phone_number} – that's {phone_number_spelled_out}.
I'll also send a quick text so you have our info handy.
Looking forward to helping you!"
```

#### Appointment Confirmation
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
I'm calling to confirm your appointment on {day} at {time}.
Please call us at {phone_number} to confirm, or reply to the text I'm sending now.
Thanks, and we'll see you soon!"
```

#### Missed Appointment
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
We missed you today for your {appointment_type} appointment.
We hope everything is okay. Please give us a call at {phone_number}
to reschedule. We're happy to find a time that works better for you."
```

#### Quote Follow-Up
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
I'm following up on the {estimate/quote} we provided for {service}.
If you have any questions or are ready to move forward,
please call us at {phone_number}. We'd love to help you get this done."
```

#### Urgent/Emergency
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
I have an important message regarding {urgent_topic}.
Please call us back as soon as possible at {phone_number}.
Again, that's {phone_number}. Thank you."
```

### Industry-Specific Voicemails

#### Roofing
```
"Hi, this is {agent_name} from {business_name}.
We received your inquiry about your roof.
With the recent weather in {area}, we're seeing a lot of hidden damage,
so I'd love to get you scheduled for a free inspection.
Call me back at {phone_number}. Talk soon!"
```

#### HVAC (Emergency Context)
```
"Hi {customer_name}, this is {agent_name} from {business_name}.
I know it's {hot/cold} right now, and I want to get your {AC/heater}
working as quickly as possible. Call us back at {phone_number}
and we'll prioritize getting a technician out to you."
```

#### Dental
```
"Hi {patient_name}, this is {agent_name} from {practice_name}.
I'm calling because you're due for your dental checkup.
Regular cleanings help prevent bigger issues down the road.
Call us at {phone_number} to schedule. We look forward to seeing you!"
```

#### MedSpa
```
"Hi {client_name}, this is {agent_name} from {spa_name}.
I'm reaching out about the {treatment} you were interested in.
We have some availability coming up and would love to get you scheduled.
Call us at {phone_number} or reply to my text. Talk soon!"
```

#### Legal
```
"Hello {caller_name}, this is {agent_name} from the Law Offices of {firm_name}.
We received your inquiry and would like to discuss your case.
Please call us back at {phone_number}. Consultations are {free/confidential}.
We're here to help."
```

---

## Implementation Notes

### Voice AI Platform Integration

**Bland.ai / Vapi / Retell Variables:**
```json
{
  "business_name": "string",
  "agent_name": "string",
  "customer_name": "string",
  "phone_number": "string",
  "service_area": "string",
  "next_available_slot": "datetime",
  "appointment_date": "date",
  "appointment_time": "time"
}
```

### ElevenLabs Voice Integration

**API Configuration:**
```json
{
  "voice_id": "{selected_voice_id}",
  "model_id": "eleven_turbo_v2",
  "voice_settings": {
    "stability": 0.6,
    "similarity_boost": 0.8,
    "style": 0.4,
    "use_speaker_boost": true
  }
}
```

**SSML for Natural Pauses:**
```
<speak>
  Thank you for calling <break time="200ms"/> {business_name}.
  This is {agent_name}. <break time="300ms"/>
  How can I help you today?
</speak>
```

### Handoff Triggers

**When to transfer to human:**
- Caller explicitly requests human agent
- Complex legal/medical advice needed
- Caller expresses frustration (sentiment detection)
- High-value opportunity identified
- Complaint or escalation scenario

**Handoff script:**
```
"I want to make sure you get the best help possible.
Let me transfer you to {role} who can assist you directly.
Please hold for just a moment."
```

---

## Metrics & Optimization

### Key Performance Indicators
| Metric | Target | Measurement |
|--------|--------|-------------|
| Answer Rate | 95%+ | Calls answered vs. total calls |
| Qualification Rate | 60%+ | Qualified leads vs. total calls |
| Appointment Set Rate | 40%+ | Appointments booked vs. qualified |
| No-Show Rate | <15% | Missed appointments vs. booked |
| Customer Satisfaction | 4.5+/5 | Post-call survey |

### A/B Testing Recommendations
- Test 2-choice vs. 3-choice appointment offers
- Compare direct scheduling vs. callback scheduling
- Test different objection handling phrases
- Experiment with voice personality variations

---

## Tags
`voice-ai`, `ai-receptionist`, `dialogue-blocks`, `elevenlabs`, `bland-ai`, `vapi`, `retell`, `roofing`, `hvac`, `dental`, `medspa`, `legal`, `conversation-flows`, `appointment-scheduling`, `lead-qualification`

---

**Last Updated:** November 2023
**Version:** 1.0
