# Play At Home

I believe the best way to learn about AI is to play with the tools that are available, become familiar with what’s possible, the strengths and weaknesses.

Included with this file are simple versions of the agent prompts I used for this experiment along with some instructions to use them in a feedback loop as described in my talk.

[!CAUTION] Remember: This isn’t meant for you to use at work and definitely not to replace the checks and balances that exist within your system. It not a finished product in any sense of the word, and it comes with no warrantee of fitness whatsoever.

1. Create a Project (isolate)

Create a project for working on your document. Both Claude and ChatGPT have projects now, which is one way to have several chats use the same source information. Upload the document that you want to work on, and the specifications you want to use as guardrails. You might want to change these documents to a format that works best for your choice of GPT. Remember, you can iterate on the specifications with AI.

2. Set up your 'Agents'
Set up at least 3 chats within the project: one for QC, one for QA, and one for you to iterate on the document. Paste the markdown files in their respective chat windows.

3. Create - Test - Fix - Interate

Work on your document with the main AI, and every once in a while ask the QC AI to test your work. The QC agent will publish a report as 'Requirements Testing Report' in markdown format. Make that report available to the whole project. Make fixes and iterate on your creation. Check the QC agent's work by asking the QA agent to evaluate the QC report.

## Disclaimer

**THESE MATERIALS ARE PROVIDED "AS-IS" FOR EDUCATIONAL PURPOSES ONLY.**

These prompts and instructions are demonstration materials from a conference presentation. They are:
- **NOT intended for production use** in regulated environments
- **NOT a substitute** for validated quality systems or compliance processes
- **NOT warranted** to be fit for any particular purpose
- **PROVIDED WITHOUT ANY WARRANTY**, express or implied, including but not limited to warranties of merchantability, fitness for a particular purpose, or non-infringement

The author assumes **NO LIABILITY** for any damages, losses, or regulatory issues arising from the use or misuse of these materials. Users assume all risks associated with their use.

If you work in a regulated industry (GLP, pharmaceutical, medical device, etc.), consult your quality and regulatory teams before adapting any of these concepts for your environment.

## License

This work is licensed under the Creative Commons Attribution 4.0 International License (CC-BY-4.0). You are free to share and adapt this material for any purpose, including commercially, as long as you provide attribution. See [LICENSE](LICENSE) for full details.
