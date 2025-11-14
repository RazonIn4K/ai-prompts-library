# Prompt Index

A comprehensive guide to finding and using prompts in the AI Prompts Library. All prompts follow a standardized format with clear categories, variables, tone, and usage examples.

---

## Quick Navigation

- **[By Use Case](#by-use-case)** – Find prompts by what you're trying to accomplish
- **[By Category](#by-category)** – Browse prompts organized by type
- **[By Tags](#by-tags)** – Filter by common themes and industries
- **[All Prompts](#all-prompts-reference)** – Complete reference with file paths

---

## By Use Case

### 🎯 Sales & Outreach
Generate leads and warm prospects with personalized messaging.

| Prompt | Purpose | Files | Complexity |
|--------|---------|-------|------------|
| **Outreach First Line** | Generate personalized opening lines for cold emails | [en](en/outreach_first_line.txt) / [es](es/outreach_first_line.txt) | Quick |
| **Lead Research to Email Intro** | Create 1–2 sentence cold-email openings from research | [en](en/lead_research_to_email_intro.txt) / [es](es/lead_research_to_email_intro.txt) | Quick |
| **Upwork Proposal General** | Draft compelling proposals for Upwork projects | [en](en/upwork_proposal_general.txt) / [es](es/upwork_proposal_general.txt) | Standard |

### 💼 Discovery & Scoping
Ask the right questions to understand client needs before proposing solutions.

| Prompt | Purpose | Files | Complexity |
|--------|---------|-------|------------|
| **Automation Discovery Questions** | 16 questions to scope automation projects | [en](en/automation_discovery_questions.txt) / [es](es/automation_discovery_questions.txt) | Standard |
| **Chatbot Discovery Questions** | 22 questions to scope chatbot projects | [en](en/chatbot_discovery_questions.txt) / [es](es/chatbot_discovery_questions.txt) | Standard |

### 📱 Chatbot Development
Configure and train AI chatbots with consistent voice and behavior.

| Prompt | Purpose | Files | Complexity |
|--------|---------|-------|------------|
| **Chatbot Tone** | Define chatbot voice, style, and interaction patterns | [en](en/chatbot_tone.md) / [es](es/chatbot_tone.md) | Quick |

### 📚 Content Creation
Transform raw content into multi-format, publishable material.

| Prompt | Purpose | Files | Complexity |
|--------|---------|-------|------------|
| **Podcast to Blog** | Generate blog post, show notes, and 5 social posts from podcast transcripts | [en](en/podcast_to_blog.txt) / [es](es/podcast_to_blog.txt) | Standard |

---

## By Category

### Outreach (3 prompts)
- Outreach First Line
- Lead Research to Email Intro
- Upwork Proposal General

### Discovery (2 prompts)
- Automation Discovery Questions
- Chatbot Discovery Questions

### Chatbot Configuration (1 prompt)
- Chatbot Tone

### Content Generation (1 prompt)
- Podcast to Blog

### Proposals & Sales (1 prompt)
- Upwork Proposal General

---

## By Tags

### Tags Explained
Each prompt is tagged with labels to help you filter by:
- **Use Case**: Outreach, Sales, Content, Discovery, Chatbot, Proposals
- **Complexity**: Quick (< 2 min setup), Standard (2–5 min), Advanced (5+ min)
- **Output Type**: Single-sentence, Multi-sentence, List, Structured Document
- **Industry**: General, SaaS, Freelance, E-commerce, Agency

### All Tagged Prompts

#### 🎯 Outreach
- **Outreach First Line** — Sales, Quick, Single-sentence, General
- **Lead Research to Email Intro** — Sales, Quick, Single-sentence, General

#### 💡 Discovery
- **Automation Discovery Questions** — Discovery, Standard, List, General / SaaS / Freelance
- **Chatbot Discovery Questions** — Discovery, Standard, List, General / SaaS

#### 📱 Chatbot
- **Chatbot Tone** — Chatbot, Quick, Reference Guide, General

#### 📝 Content
- **Podcast to Blog** — Content, Standard, Structured Document, General

#### 💼 Proposals
- **Upwork Proposal General** — Proposals, Sales, Standard, Multi-paragraph, Freelance / Agency

---

## All Prompts Reference

### 1. Outreach First Line
**Category:** Outreach
**Purpose:** Generate personalized opening lines for cold emails
**Variables:** `{name}`, `{personalized_fact}`
**Tone:** Friendly, genuine, conversational
**Complexity:** Quick
**Files:** [English](en/outreach_first_line.txt) | [Spanish](es/outreach_first_line.txt)

**Use When:**
- You need to warm up a prospect with a personalized message
- You want to avoid generic "hope this finds you well" phrases
- You have researched the person and found a relevant connection point

**Expected Output:** 1–2 sentence opening line ready to copy into an email

---

### 2. Lead Research to Email Intro
**Category:** Outreach
**Purpose:** Create personalized cold-email opening lines from prospect research
**Variables:** `{prospect_name}`, `{company}`, `{research_snippets}`
**Tone:** Genuine, conversational, research-backed, non-salesy
**Complexity:** Quick
**Files:** [English](en/lead_research_to_email_intro.txt) | [Spanish](es/lead_research_to_email_intro.txt)

**Use When:**
- You've done research on a prospect and want to write a personalized first line
- You want to establish credibility and genuine interest before pitching
- You need an opening that doesn't feel templated

**Expected Output:** 1–2 sentence opening line, ready to copy-paste

---

### 3. Chatbot Tone
**Category:** Chatbot Configuration
**Purpose:** Define voice and tone characteristics for AI chatbots
**Variables:** None (reference guide)
**Tone:** Instructional, clear, professional
**Complexity:** Quick
**Files:** [English](en/chatbot_tone.md) | [Spanish](es/chatbot_tone.md)

**Use When:**
- Building a new chatbot and want consistent voice across all interactions
- Training a team on how your chatbot should sound
- Reviewing chatbot responses for alignment with brand voice

**Expected Output:** Guidelines to train your chatbot's voice, plus example interactions

---

### 4. Podcast to Blog
**Category:** Content Generation
**Purpose:** Transform podcast transcripts into blog, show notes, and social posts
**Variables:** `{transcript}`
**Tone:** Friendly, engaging, conversational, professional
**Complexity:** Standard
**Files:** [English](en/podcast_to_blog.txt) | [Spanish](es/podcast_to_blog.txt)

**Use When:**
- You have a podcast episode transcript and want to repurpose it
- You need blog content, show notes, and social media posts from one source
- You want to maximize reach by publishing across multiple formats

**Expected Output:**
- 600–800 word blog post with headings
- 8–10 bullet-point show notes
- 5 standalone social media posts

---

### 5. Lead Research to Email Intro
**Category:** Outreach
**Purpose:** Generate personalized cold-email opening lines from prospect research
**Variables:** `{prospect_name}`, `{company}`, `{research_snippets}`
**Tone:** Genuine, conversational, research-backed, non-salesy
**Complexity:** Quick
**Files:** [English](en/lead_research_to_email_intro.txt) | [Spanish](es/lead_research_to_email_intro.txt)

**Use When:**
- You need to write a cold email with a personalized first line
- You've done research and want to show genuine interest
- You want to stand out from generic outreach

**Expected Output:** 1–2 sentence opening line

---

### 6. Upwork Proposal General
**Category:** Proposals & Sales
**Purpose:** Draft compelling Upwork proposals from client job posts and your capabilities
**Variables:** `{client_job_post}`, `{my_capabilities}`
**Tone:** Professional, empathetic, confident, action-oriented
**Complexity:** Standard
**Files:** [English](en/upwork_proposal_general.txt) | [Spanish](es/upwork_proposal_general.txt)

**Use When:**
- You're applying for an Upwork project and need a strong proposal
- You want to customize your response to specific client needs
- You need to include your value proposition in under 300 words

**Expected Output:** Ready-to-submit Upwork proposal (under 300 words) with empathy, plan, and CTA

---

### 7. Automation Discovery Questions
**Category:** Discovery
**Purpose:** Strategic questions to understand workflows and pain points for automation projects
**Variables:** None (reference guide)
**Tone:** Consultative, open-ended, discovery-focused
**Complexity:** Standard
**Files:** [English](en/automation_discovery_questions.txt) | [Spanish](es/automation_discovery_questions.txt)

**Use When:**
- You're in early conversations with an automation prospect
- You need to understand their current processes before proposing solutions
- You want to ensure alignment with real business needs

**Expected Output:** 16 discovery questions organized by topic (workflows, pain points, tools, goals)

---

### 8. Chatbot Discovery Questions
**Category:** Discovery
**Purpose:** Comprehensive questions to scope chatbot project requirements
**Variables:** None (reference guide)
**Tone:** Consultative, thorough, technical and business-focused
**Complexity:** Standard
**Files:** [English](en/chatbot_discovery_questions.txt) | [Spanish](es/chatbot_discovery_questions.txt)

**Use When:**
- A prospect wants a chatbot solution and you need to understand their needs
- You want to scope the project before writing a proposal
- You need to cover all dimensions (purpose, audience, functionality, integrations, budget)

**Expected Output:** 22 discovery questions organized by topic (purpose, audience, functionality, languages, resources, integrations, timeline/budget)

---

## How to Use the Index

1. **Start with "By Use Case"** if you know what you're trying to accomplish
2. **Check "By Tags"** if you want to filter by complexity, industry, or output type
3. **Reference "All Prompts"** for detailed info about specific prompts
4. **Open the file** in your preferred AI model (see main README for platform-specific guidance)

---

## Contributing New Prompts

When adding new prompts to the library:

1. Follow the standardized format (CATEGORY, PURPOSE, VARIABLES, TONE, PROMPT, EXAMPLE USAGE)
2. Create both English and Spanish versions
3. Add entries to this index under the appropriate use case and category
4. Assign relevant tags
5. Update the main README if creating a new category

---

**Last Updated:** November 2024
**Total Prompts:** 14 (7 English + 7 Spanish)
