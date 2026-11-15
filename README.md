# LLM-Skill-Template-by-CBTU-MU:

## Google Antigravity Workshop Outline
- Course Ref. --> [here](https://cbtumu.net/coursenew/cbtu-ai-day-ai-for-work/)
- Slide/Prompt/Tutorial --> [here](https://claude.ai/artifact/V4k8UXsE9qRm6AEEK8f8SL)
- Download Skill --> [here](https://skillsmp.com/)
- Markdown Cheat Sheet --> [here](https://github.com/lifeparticle/Markdown-Cheatsheet)
- Workflow Discovery Coach --> [here](https://github.com/toche7/mySkills)

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
| **section** | **role** |
|-:|:-|
|SKILL.md|Name, description, and instructions|
|references/|Criteria or reference documents|
|assets/|Templates used to generate outputs|
|scripts/|Programs for processing, as needed|

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
