# Project Instructions Template

The purpose of this project is to *{what do you want to accomplish? e.g. "Develop an SOP to X, following the specifications laid out in Y". Try to be specific and detailed in what you want the project to do.}*

This project will use a QC/QA testing and feedback framework using several separate 'agent' roles. These agents will be defined by chat-specific prompts. 

The main working document in this project is *{name of the file you will be working on}*
The specification(s) that this document must follow are: *{Name or names of the specifications and guidelines, if used}*

The framework is simple and mirrors code development, but for Quality documents and workflows. There is a main development loop consisting of a human and AI making changes to the document.

There is a QC spec tester agent that will test document output against its specification, following strict instructions for testing and reporting (the QC prompt). It will produce a report.

There is a QA agent that checks the evidence in the QC report, ensuring the evidence exists and supports the conclusions, again following strict instructions (the QA prompt). It will produce a report as well.


