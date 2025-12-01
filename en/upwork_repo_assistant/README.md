# Upwork Funnel Job Repo Assistant

This pack contains advanced prompts that instruct your IDE AI (Cursor, Jules, Stitch) to **create a structured workspace directly in your repository** for each Upwork job.

Unlike the standard "Prompt Pack" which outputs text in the chat, this "Repo Assistant" builds a folder structure with markdown artifacts (`requirements`, `plan`, `proposal`, etc.) ready for you to work on.

## How to Use

1.  **Open your IDE AI chat.**
2.  **Copy & Paste the Universal Header:**
    - Open `00_UNIVERSAL_HEADER.md` and copy the entire content.
    - Paste it into the chat.
3.  **Copy & Paste the Job-Specific Add-On (Optional):**
    - If you have a specific scenario (e.g., GHL 20 Funnels), open the matching file (e.g., `01_JOB_GHL_20_FUNNELS.md`).
    - Copy and paste it immediately after the header.
4.  **Paste the Upwork Job Description:**
    - Copy the full text of the Upwork job posting.
    - Paste it at the very end.
5.  **Run the Prompt:**
    - Tell the AI: "Run the workflow and write all outputs into the repo as files."
    - The AI will create a folder in `upwork_jobs/` with all the necessary files.

## Files

- `00_UNIVERSAL_HEADER.md`: The core instructions for the repo-building agent. **Use this for every job.**
- `01_JOB_GHL_20_FUNNELS.md`: Add-on for "Setup GoHighLevel Domain + Connect It With 20 Funnels".
