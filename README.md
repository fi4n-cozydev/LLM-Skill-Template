# LLM-Skill-Template:

## Google Antigravity Workshop Outline
   - Markdown Cheat Sheet --> [here](https://github.com/lifeparticle/Markdown-Cheatsheet)
   - Slide/Prompt/Tutorial --> [here](https://claude.ai/artifact/V4k8UXsE9qRm6AEEK8f8SL)
   - Agent Skills Marketplace --> [here](https://skillsmp.com/)
   - Agent Skills by Taweesak (Swimlane Diagram) --> [here](https://github.com/toche7/mySkills)

### AI Boost Bootcamp: How to Use Gemini at Work 101:
   - [Course Ref.](https://www.skills.google/course_templates/1674)

### CBTU AI Day : AI for Work:
   - [Course Ref.](https://cbtumu.net/coursenew/cbtu-ai-day-ai-for-work/)

### CBTU AI Day : AI for Research:
   - [Course Ref.](https://cbtumu.net/coursenew/cbtu-ai-day-ai-for-research/)

## Effective Prompt Engineer 
> **`Persona --> Task --> Context --> Format`**
```
(1) Persona 
I am a customer service representative.

(2) Task 
I need to write a letter responding to a customer complaint. 

(3) Context 
The customer ordered a pair of headphones that arrived damaged. They've already contacted us via email and provided pictures of the damage. I've offered a replacement, but they're requesting an expedited shipping option that isn't typically included in that order. Include a paragraph that acknowledges their frustration 

(4) Format 
three bulletpoints with potential resolutions.
```

# Skill Config:
**Workspace-Skill**
```
Antigravity Desktop: C:\Users\{yourUsername}\Desktop\ICCS-Skill-Workshop\.agents\skills\{skill-name}\
```

**Gloabal-Skill**
> folder `skills` system didn't create by default you must create it on you own.
```
(WIN)
Antigravity Desktop: C:\Users\{yourUsername}\.gemini\config\skills\{skill-name}\

(MAC)
Antigravity Desktop: ~/.gemini/config/skills/{skill-name}/
Antigravity CLI: ~/.gemini/antigravity-cli/skills/{skill-name}/
```

# Skill Element Structure:
| **SECTION** | **ROLE** |
|-:|:-|
|SKILL.md|Name, description, and instructions|
|references/|Criteria or reference documents|
|assets/|Templates used to generate outputs|
|scripts/|Programs for processing, as needed|

## `Skill Implementation Stage`
   1. Create Skills
      1. Target task
   2. Verification
      1. Create Test case using AI
      2. Testing Test case (*`.md files`*)
   4. Improvement
      1. Error logs


# Skill Template:
```
---
name: ชื่อ-skill-ภาษาอังกฤษ-ตัวเล็ก
description: Skill นี้ทำอะไร และควรเรียกใช้เมื่อใด (ใส่คำที่ผู้ใช้มักพิมพ์)
---
# Skill ชื่อภาษาไทย

## วัตถุประสงค์
สิ่งที่ Skill นี้ออกแบบมาเพื่อทำ

## เงื่อนไขการใช้งาน
เงื่อนไขที่ควรเรียกใช้ Skill นี้ และข้อมูลนำเข้า (Input) ที่ต้องมี

## คำแนะนำ
Workflow แบบเป็นขั้นตอน
1. ...
2. ..
3. ...

## กฎ
ข้อจำกัดและข้อกำหนดสำคัญ

## รูปแบบไฟล์ผลลัพธ์
ฟอนต์ ขนาด การจัดหน้า ตาราง และสคริปต์ที่ใช้สร้างไฟล์ (เช่น scripts/md_to_docx.py)

## ผลลัพธ์
ผลลัพธ์หรือชิ้นงานที่คาดหวัง (ชื่อไฟล์ รูปแบบ ที่เก็บ)

## Checklist คุณภาพ
- [ ] สิ่งที่ต้องตรวจก่อนส่งงาน

<!--
โฟลเดอร์ประกอบ (ไม่บังคับ)
references/        รูปแบบเอกสารที่สกัดจากไฟล์ต้นแบบ (format-*.md) และความรู้ประกอบ
assets/            แม่แบบที่มีช่องเติมข้อมูล (*-template.md / .html / .docx)
assets/examples/   ไฟล์ต้นแบบ (.docx/.pdf)
scripts/           สคริปต์ช่วยงาน เช่น md_to_docx.py
-->
```

## Build custom AI agents with Gemini Enterprise
> **`Brains > Context > Taskforce > Partners Ecosystem > Workbench > Governance`**

   - Brains and context set the foundation for your task force.
   - A library of AI agents, each dedicated to a single task to help you work. 
```
      1. setup agent's persona and goals
      2. divide its goals into subtask
      3. create instructions
      4. create a comparison to show different options
```

> <ins>TO CREAT AN AGENT :</ins>
```
Name: Scheduling agent
Description: Let's get scheduling!

Instruction: 
ROLE : AGENT PERSONA
You are an expert at staffing a store's shifts based on employee availability and preferences and policies. You will create an optimized work schedule, analyze it for conflicts, and present the final schedule and conflict report. You will use Gmail to send the schedule to staff if requested by the user.

OUTPUT EXPECTATIONS : GOALS
The final output will be a comprehensive, clearly formatted employee work schedule accompanied by a distinct conflict report.
1. The output table must present the daily shifts, assigned employees, and their designated backups, with each date, time/shift, and staffing recommendations clear and readable.
2. Each shift should have two people scheduled. Afternoon shifts should preferably have three employees. An available backup employbe must be noted for each shift. No employee should be scheduled for more than 40 hours per week unless it is unavoidable.
3. The conflict report must be presented in a distinct section following the schedule table.
4. The conflict report should clearly list any identified issues, the affected employee(s) or shift(s), and the reason for requiring user attention.
5. Before outputting your results, check them again for any errors. If conflicts persist, consider whether any alternate schedules are possible that could satisfy these conflicts without introducing new ones. Only when you have optimized and checked your work should you output.
6. The entire output must be clean, use appropriate headers, and be easily digestible for the user.
7. Do not include preamble about what steps you plan to do. Just output the final report.
8. The final report should start with the schedule table, then list any conflicts or notes that could note be addressed. That is all.
```

# _Project Proposal Development Process_

> <ins>AS-IS: --> (!Old) Workflow</ins>
1. _`Strategic Plane`_
2. _`Meeting`_
3. _`Department Meeting`_
4. _`Prepare Proposal`_
   - Issue
      - idea
      - document
      - Standard
      - code
5. _`Head Department Sign`_
    - Issue
      - take time
      - large document deck.
      - Not complete
6. _`Check Strategic Department`_
   - Issue
      - Not complete
      - Code
      - TOR. (Terms of Reference)
      - quotation

> <ins>TO-BE: --> (!NEW) Workflow</ins>
1. _`Strategic Plane`_
2. _`Meeting`_
3. _`Department Meeting`_
4. _`AI Draft Prososal`_
    - _Human Check Proposal_
    - _AI Check Proposal Aligment with PLan and Standard_
5. _`Head Department Sign`_
6. _`Check Stategic Department`_

# Basic Research Process
>### _`Define a topic`_ --> _`Do Research`_ --> _`Publish`_
---
>### General Research Process
   1. Isue
   2. Research Question
   3. Theory and Related WOrk Review
   4. Research Hypothesis
   5. Research Design
   6. Instrument / Tool Validation
   7. Data Collection
   8. Data Analysis
   9. Report
   10. Publish

>### Engineering Research Process
   1. Issue
      1. Literature Review
   2. New Idea
      1. Theory and Related Work Review
   3. Design
      1. Math Model
         1. Evaluation
         2. Result
      2. Simulation
         1. Evaluation
         2. Result
      3. Implementation
         1. Evaluation
         2. Result
   4. Report
   5. Publish

>### Data Science Research Process
   1. Data / Big Data / Literature Review
      - Literature Review
   2. Data Exploration
   3. Research Question / Hypothesis
   4. Data Preprocessing
   5. Modeling
   6. Evaluation
   7. Result
   8. Report
   9. Publish

# Hybrid Intelligence Research Framework
   1. Problem Framing & Research Focus
   2. Literature Review & Knowledgge Expansion
   3. Research Design & Method Planning
   4. Data Work & Analytical Reasoning
   5. Scholarly Writing, Reflection & Knowledge Contribution

# Writing Process (Pro Tips)
   1. Issue/Topic
   2. Chapter 2 - Literature Review & Gap Analysis
   3. Chapter 3 - Methodology
   4. Chapter 4 - Result & Discussion
   5. Chapter 5 - Conclusion
   6. Chapter 1 - Introduction
   7. Abstract
   8. Publishing

# Stage 1 --> Prompt
   - `Treand:` "Suggest emerging research topics in the use of AI in higher education, with a focus on ethical implications and policy."
   - `Specific Topic:` "Give me 5 research topics combining GenAI and statistical literacy for government employees."
   - `Gap:`"What are the research gaps in applying Generative AI in public sector data analysis?"

# Research Tools
   - [SciSpace](https://scispace.com/th) | Data organization, AI writer, citation generator
   - [Paper Finder](https://github.com/allenai/asta-paper-finder) | Semantic search, explanation of recommendations, free bibliography export
   - [Elicit](https://elicit.com/) | PICO framework, structured data extraction, access to 125 million papers
   - [Consensus](https://consensus.app/) | Consensus meter, specialized for health and medical fields
   - [Scopus](https://www.scopus.com/pages/home) | Large, reliable database; concept maps; deep research capabilities
   - [Gemini Notebook](https://notebook.google.com) | Analyzes uploaded documents, minimizes hallucinations, generates mind maps
   - [Google Scholar](https://scholar.google.com/)
   - [PubMed](https://pubmed.ncbi.nlm.nih.gov/)
