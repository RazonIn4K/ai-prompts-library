# AI Prompts Library

A curated collection of reusable AI prompt templates for outreach, chatbot tone, and content generation, available in both English and Spanish. This library provides ready-to-use prompt snippets with detailed voice and style guidelines to help you get the best results from AI models.

## 📚 Available Prompts

### Outreach First Line
Generate compelling opening lines for outreach messages that capture attention and establish genuine connection.

- **English**: [en/outreach_first_line.md](en/outreach_first_line.md)
- **Spanish**: [es/outreach_first_line.md](es/outreach_first_line.md)

### Chatbot Tone
Define consistent voice and style characteristics for AI chatbot interactions to ensure engaging and effective communication.

- **English**: [en/chatbot_tone.md](en/chatbot_tone.md)
- **Spanish**: [es/chatbot_tone.md](es/chatbot_tone.md)

### Quick-Start Income Prompts
Ready-to-use prompts designed to help generate monetizable content and streamline your sales workflow:

#### Podcast to Blog
Transform podcast transcripts into multi-format content: a 600–800 word blog post with headings, concise show notes, and five shareable social media posts—all in one go.

- **English**: [en/podcast_to_blog.txt](en/podcast_to_blog.txt)
- **Spanish**: [es/podcast_to_blog.txt](es/podcast_to_blog.txt)

**Quick Example:**
```
Copy the prompt from en/podcast_to_blog.txt, replace {transcript} with your podcast transcript,
and paste into your preferred AI model. You'll get formatted blog content, show notes, and
five social posts ready to publish.
```

#### Lead Research to Email Intro
Generate personalized, human-sounding cold-email opening lines based on prospect research. 1–2 sentences that feel genuine and non-spammy, not templated.

- **English**: [en/lead_research_to_email_intro.txt](en/lead_research_to_email_intro.txt)
- **Spanish**: [es/lead_research_to_email_intro.txt](es/lead_research_to_email_intro.txt)

### Proposals & Discovery
Prompts and question templates for winning Upwork bids and scoping client projects effectively:

#### Upwork Proposal General
Draft compelling Upwork proposals that address client needs, outline a clear plan, and include a strong CTA. Input your client's job post and your capabilities to generate a personalized, concise proposal.

- **English**: [en/upwork_proposal_general.txt](en/upwork_proposal_general.txt)
- **Spanish**: [es/upwork_proposal_general.txt](es/upwork_proposal_general.txt)

**Quick Example:**
```
Replace {client_job_post} with the Upwork job description and {my_capabilities} with your
relevant skills/experience. The prompt generates a ready-to-submit proposal under 300 words
that demonstrates empathy, outlines numbered steps, and includes a strong CTA.
```

#### Automation Discovery Questions
Strategic questions to uncover a prospect's workflows, pain points, tools, and priorities. Use these before proposing any automation solution to ensure alignment with their actual needs.

- **English**: [en/automation_discovery_questions.txt](en/automation_discovery_questions.txt)
- **Spanish**: [es/automation_discovery_questions.txt](es/automation_discovery_questions.txt)

#### Chatbot Discovery Questions
Comprehensive discovery guide for scoping chatbot projects. Covers purpose, audience, functionality, languages, existing resources, integrations, and timeline—everything you need to propose the right solution.

- **English**: [en/chatbot_discovery_questions.txt](en/chatbot_discovery_questions.txt)
- **Spanish**: [es/chatbot_discovery_questions.txt](es/chatbot_discovery_questions.txt)

## 🌍 Supported Languages

- **English** (`en/`)
- **Spanish** (`es/`)

## 📖 How to Use Prompts

### Quick Start
1. **Browse the [PROMPT_INDEX.md](PROMPT_INDEX.md)** to find the right prompt for your use case
2. **Open the prompt file** in your preferred language (`en/` or `es/` folder)
3. **Copy the entire prompt content** into your AI model
4. **Replace placeholders** like `{name}`, `{transcript}`, etc. with your actual data
5. **Submit and review** the output, refining variables if needed

### Using Prompts with Different AI Platforms

#### ChatGPT / ChatGPT Plus
1. Open [ChatGPT](https://chat.openai.com)
2. Start a new conversation
3. Copy the entire prompt file into the message box
4. Hit Enter and wait for the response
5. **Pro tip:** For longer prompts, paste the prompt first, then provide your variables in a follow-up message

#### Claude (Web, Desktop, or API)
1. Open [Claude](https://claude.ai) or your Claude interface
2. Paste the complete prompt into the chat
3. Claude's large context window handles long prompts exceptionally well
4. **Pro tip:** Claude excels with discovery questions and multi-step outputs (like podcast-to-blog)

#### Google Gemini
1. Go to [Google Gemini](https://gemini.google.com)
2. Paste the prompt into the chat box
3. For longer prompts, you may need to break them into 2–3 messages
4. **Pro tip:** Gemini is great for quick generation tasks like email openings

#### Microsoft Copilot (Windows/Bing)
1. Open [Copilot](https://copilot.microsoft.com)
2. Paste the prompt into the chat
3. Provide your variables and submit
4. **Pro tip:** Good for quick iterations and refinements

### Prompt Structure

Each prompt file in this library includes:

```
CATEGORY: [Type of prompt]
PURPOSE: [What it does]
VARIABLES: [Required placeholders]
TONE: [Voice and style characteristics]

[Prompt instructions and content]

EXAMPLE USAGE:
[Sample input and output]
```

### Best Practices for Variable Substitution

1. **Replace all placeholders** – Look for variables in curly braces: `{variable_name}`
2. **Be specific** – Vague inputs lead to vague outputs
3. **Maintain consistency** – If a variable appears multiple times, use the same value throughout
4. **Test first** – Try with sample data before using real information
5. **Iterate** – Refine outputs by adjusting your input variables

**Example:**
```
Original: "Hi {name}, I noticed {personalized_fact}..."
Your input: "Hi Sarah, I noticed you just launched a podcast on startup culture..."
```

### Customization Tips

- **Adjust tone**: Modify phrases like "friendly" to "formal" or "enthusiastic" to "straightforward"
- **Change length**: Specify word counts or duration for outputs (e.g., "under 200 words")
- **Focus on specifics**: Add industry details, product names, or company context
- **Combine prompts**: Use discovery questions first, then feed answers into a proposal prompt
- **Create variations**: Save custom versions of prompts with your preferred tweaks

---

## 🔍 Find the Right Prompt

- **Quick reference**: [PROMPT_INDEX.md](PROMPT_INDEX.md) – Organized by use case, category, and tags
- **By category**: Outreach, Discovery, Chatbot, Content, Proposals
- **By complexity**: Quick (< 2 min), Standard (2–5 min), Advanced (5+ min)

## 🤝 Contributing

Contributions are welcome! If you have a prompt to add or improvements to existing ones:

1. **Follow the standardized format**:
   ```
   CATEGORY: [Outreach/Discovery/Chatbot/Content/Proposals]
   PURPOSE: [One-line description of what the prompt does]
   VARIABLES: [List all {placeholders} used in the prompt]
   TONE: [Describe voice and style characteristics]

   [Prompt instructions and content]

   EXAMPLE USAGE:
   [Show sample input and expected output]
   ```

2. **Create both English and Spanish versions** (save in `en/` and `es/` folders with matching names)
3. **Update [PROMPT_INDEX.md](PROMPT_INDEX.md)** with entries in appropriate use case and category sections
4. **Test the prompt** with multiple AI models to ensure quality output
5. **Submit a pull request** with a clear description of the new prompt and its use case

## 📝 License

This project is open source and available for use in your AI applications and workflows.

## 🔗 Related Resources

- [PROMPT_INDEX.md](PROMPT_INDEX.md) – Complete reference guide for all prompts
- [Prompt Engineering Guide](https://www.promptingguide.ai/)
- [OpenAI Best Practices](https://platform.openai.com/docs/guides/prompt-engineering)
- [Anthropic Claude Prompt Guide](https://docs.anthropic.com/en/docs/build-a-chatbot-with-claude)

---

## ✨ Key Features

- **Standardized format** across all prompts for consistency and discoverability
- **14 bilingual prompts** covering outreach, discovery, chatbot, content, and proposals
- **Platform-agnostic** – Use with ChatGPT, Claude, Gemini, Copilot, and more
- **Production-ready** – Each prompt has been tested and refined for real-world use
- **Easy customization** – Clear variables and tone guidance for your specific needs
- **Growing library** – Submit new prompts and improvements via pull requests

---

**Note**: These prompts are designed to work with various AI models (GPT-4, Claude 3, Gemini Pro, etc.). Results vary by model and parameters. Test with your preferred AI platform and adjust variables for optimal results.

**Last Updated:** November 14, 2024