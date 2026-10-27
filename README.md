# CrewAI Job-Search Agent: Design Note

Design note for the multi-agent job-search system built in the capstone's [Part 4](https://github.com/Geeka/Part_4_Agentic_AI_system). The agent reads a resume, searches live job listings, and emails the best match.

**Result:** good-match rate of **13 of 20 (65%)** across 10 synthetic resumes and two crews (sequential 8 of 10, hierarchical 5 of 10). A good match scores 4 or more out of 5 on a manual check of title, level and employer. The sequential process was chosen for the delivered system.

**Failed runs:** 2 of the 10 resumes needed one rerun (a run that stopped before searching, and a JSON parse error on the model's reply). Both completed on the rerun.

See `crewai_agent_design_note.md` for the requirements, architecture and design decisions.
