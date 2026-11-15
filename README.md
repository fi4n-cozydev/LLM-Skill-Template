# LLM-Skill-Template-by-CBTU-MU:

##### Google Antigravity Workshop Outline
- Course Ref. --> [here](https://cbtumu.net/coursenew/cbtu-ai-day-ai-for-work/)
- Slide/Prompt/Tutorial --> [here](https://claude.ai/artifact/V4k8UXsE9qRm6AEEK8f8SL)
- Download Skill --> [here](https://skillsmp.com/)
- Markdown Cheat Sheet --> [here](https://github.com/lifeparticle/Markdown-Cheatsheet)

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

# Skill Structure:
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

# _Project Proposal Development Process_

## **AS-IS: --> !Old Workflow**
1. `_Strategic Plane_`
2. `_Meeting_`
3. `_Department Meeting_`
4. `_Prepare Proposal_`
   - Issue
      - idea
      - document
      - Standard
      - code
5. `_Head Department Sign_`
    - Issue
      - take time
      - large document deck.
      - Not complete
6. `_Check Strategic Department_`
   - Issue
      - Not complete
      - Code
      - TOR. (Terms of Reference)
      - quotation

## *TO-BE: --> !NEW Workflow*
1. _`Strategic Plane`_
2. _`Meeting`_
3. _`Department Meeting`_
4. _`AI Draft Prososal`_
    - _Human Check Proposal_
    - _AI Check Proposal Aligment with PLan and Standard_
5. _`Head Department Sign`_
6. _`Check Stategic Department`_
