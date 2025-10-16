# CCSQA/NERCSQA Attendees Bonus: Play At Home

Thanks for attending "The power of a specification: Freeing your creative self to go beyond compliance"!

Here are the AI prompts I promised that demonstrate a fast feedback loop with layered QA/QC agents, as described in the talk.

## What's Included

This repository contains:
- **`project-instructions-template.md`** - A template where you can put instructions for what you want to accomplish in this project, e.g. modify an SOP. 
- **`qc-spec-tester.md`** - QC agent prompt that tests documents against specifications
- **`qa-evidence-verifier.md`** - QA agent prompt that verifies QC testing evidence and reports
- **`README.md`** - This file with setup instructions
- **`LICENSE`** - CC-BY-4.0 license details

## Downloading the Files

Each markdown file contains a complete prompt that you can use with AI tools like **Claude** or **ChatGPT**.

**To use them:**
- Click any `.md` file above to view it, then copy the contents
- Or download the entire repository: click the green "Code" button → "Download ZIP"

> [!Tip] When you open a .md file, copy everything (including the markdown headings). ChatGPT automatically interprets markdown when pasted into chat.

## How to Use These Agents

> [!CAUTION] **These materials are for learning and experimentation only.** They are not intended for production use in regulated environments or as a replacement for validated quality systems. See the Disclaimer section below.

### Step 1: Create an Isolated Project

Create a dedicated project/workspace in your AI tool. This keeps your experiment separate and allows multiple chats to share the same documents.

In the **project instructions** add the contents of `project-instructions-template.md` and complete the missing details for what your goals are for the project.

**Claude users:**
Use Projects to group related chats and documents. Upload your files (SOPs, specs, templates) to the project’s shared files section.

**ChatGPT users:**
If you have ChatGPT Projects (Pro/Team), create a new project and upload your files there.

If you don’t have Projects, you can simulate it by manually re-uploading the same files into each chat.

**Upload to your project (or each chat):**

- The document you want to work on (e.g., an SOP, protocol, or report).
- The specifications or requirements it must meet.
- Any templates or style guides.

> [!Tip] You can use AI to help refine your specifications before you begin.



### Step 2: Set Up Your Agent Chats

Create at least three separate chats within your project:

1. **Creator Chat** - Your working space for drafting and editing the document
2. **QC Chat** - In a new chat, say: "You are the QC specification tester. Follow the instructions I’ll paste below:". Now paste or upload the `qc-spec-tester.md` prompt here.
3. **QA Chat** - In a new chate, say: "You are the QA evidence verifier. Follow the instructions I'll paste below:". Paste or upload the `qa-evidence-verifier.md` prompt here.

Each chat has access to the same project documents but performs a different role. Make sure you restate the role clearly (“You are the QC tester…”) each time you start a new chat for consistent behavior.

> [!Tip] Optional (ChatGPT Projects): After pasting each agent prompt, click “Pin” to keep it visible at the top of the chat.


### Step 3: The Fast Feedback Loop

**Create → Test → Fix → Iterate:**

1. **Create:** Draft or edit your document in the Creator chat
2. **Test (QC):** Ask the QC chat to test your document against the specifications.
   - The QC agent will produce a "Requirements Testing Report" in markdown format
   - Save this report to your project files
3. **Fix:** Review the QC findings and make corrections in your Creator chat
4. **Verify (QA):** Ask the QA chat to review the QC report
   - The QA agent checks that testing evidence is properly documented and valid
   - This adds a second layer of quality checking
5. **Iterate:** Repeat the cycle as you refine your document

> [!Tip] In **ChatGPT**: To save a report, click the '...' (three dots) next to the message → “Copy message” and paste it into your markdown editor or back into the project files. In **Claude**, click on the generated report and look for the "Copy" button above to copy the report to the project. If you don't see that option, just ask Claude to save it to the project.

**The key benefit:** You get rapid feedback on compliance issues while you work, rather than discovering problems during formal review.

### Further Exploration

What I've described so far is a rather manual process - you need to upload, convert and move documents between the 'agents' and ask them to do their thing. 

Once you get familiar with the workflow you can start playing with various agentic tools to orchestrate and automate between the roles. For example, you could automate sending files between the QA/QC agents when changes are detected, trigger re-testing when changes are detected, and generate dashboards or summary reports of quality metrics. 

These require more setup but can mirror an automated QA/QC pipeline.

If you're interested in a workshop that explores these and other topics for building multi-agent QA/QC workflows for quality, let me know by [joining the waitlist](https://daily.haiqu.ca/ffl-workshop) and I'll notify you when workshop dates are available.

---

### Compatibility Notes

| Feature              | Claude                      | ChatGPT                                   |
| -------------------- | --------------------------- | ----------------------------------------- |
| Shared context       | Built-in via *Projects*     | Available via *Projects* (Pro/Team only)  |
| Markdown handling    | Previews markdown visually  | Renders markdown text directly            |
| Upload & reuse files | Native file panel           | File panel (Pro/Team) or manual re-upload |
| Role consistency     | Retained across long chats  | Reinforce role each session for stability |
| Output saving        | “Download” or copy directly | “... → Copy message”            |

---

## Disclaimer

**THESE MATERIALS ARE PROVIDED "AS-IS" FOR EDUCATIONAL PURPOSES ONLY.**

These prompts and instructions are demonstration materials from a conference presentation. They are:
- **NOT intended for production use** in regulated environments
- **NOT a substitute** for validated quality systems or compliance processes
- **NOT warranted** to be fit for any particular purpose
- **PROVIDED WITHOUT ANY WARRANTY**, express or implied, including but not limited to warranties of merchantability, fitness for a particular purpose, or non-infringement

The author assumes **NO LIABILITY** for any damages, losses, or regulatory issues arising from the use or misuse of these materials. Users assume all risks associated with their use.

**If you work in a regulated industry** (GLP, pharmaceutical, medical device, etc.), consult your quality and regulatory teams before adapting any of these concepts for your environment.

## License

This work is licensed under the Creative Commons Attribution 4.0 International License (CC-BY-4.0). You are free to share and adapt this material for any purpose, including commercially, as long as you provide attribution. See [LICENSE](LICENSE) for full details.
