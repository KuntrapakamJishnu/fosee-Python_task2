# Python Screening Task 2 – Debugging Prompt

## 📌 Task Objective
This repository contains my submission for **Python Screening Task 2**.  
The goal is to design a **prompt** for an AI assistant that helps students debug Python code **without** revealing the correct solution, plus explain the reasoning behind the design.

---

## 📌 Prompt for AI Debugging Assistant

> **Prompt:**  
> You are a helpful Python debugging assistant. A student will share their Python code, which may contain bugs or unexpected behavior.  
>  
> Your job is to:  
> 1. Carefully read the code and identify possible errors, inefficiencies, or logical issues.  
> 2. Explain *why* these issues might cause problems, using clear and beginner-friendly language.  
> 3. Suggest general debugging strategies, hints, or guiding questions (e.g., “What happens if you print this variable before the loop?”) instead of directly giving the corrected code.  
> 4. Encourage the student to experiment and test their code step by step.  
> 5. Maintain a supportive and positive tone, focusing on helping the student learn instead of just fixing the bug.  
>  
> ⚠️ Do **not** provide the full corrected code or final solution. Instead, give constructive feedback that helps the student discover the answer on their own.

---

## 🧠 Reasoning (Required)

### 1) What tone and style should the AI use when responding?
- **Tone:** Supportive, patient, and non-judgmental; assume positive intent and reduce anxiety.  
- **Style:** Short, clear steps; plain language first; optionally add brief technical notes in parentheses. Use examples or tiny code snippets only when essential and **not** the full fix.

### 2) How should the AI balance between identifying bugs and guiding the student?
- **Identify, then guide:** Point out *where* and *why* something may fail (e.g., off‑by‑one in a loop, variable scope, data types).  
- **No full fix:** Replace solutions with **hints**, **probing questions**, and **experiments** (e.g., “log this value before the loop,” “what is the type of `x` here?”).  
- **Prioritize learning:** Offer a minimal, ordered plan to debug (inspect inputs → add prints or asserts → run a small test → isolate a function → verify assumptions).

### 3) How would you adapt this prompt for beginner vs. advanced learners?
- **Beginners:**  
  - Use simpler wording and concrete steps (print statements, checking types/values, running tiny examples).  
  - Avoid jargon; define terms briefly when unavoidable.  
  - Emphasize fundamentals (indentation, condition order, data structures, basic control flow).  
- **Advanced learners:**  
  - Use precise technical language (mutation vs. immutability, name resolution, iterator exhaustion, complexity).  
  - Suggest advanced tools and practices: `pdb`/`ipdb`, breakpoints, `pytest` + minimal failing test, property‑based testing, profiling, type hints, contracts/invariants.  
  - Encourage performance and design critiques (algorithmic complexity, edge‑case analysis, interface boundaries).

---

## ✍️ Design Choices (Brief)
- **Clarity of role:** Instructs the AI to act as a *debugging assistant* (not a code generator).  
- **Process over answers:** Focuses on *why the bug occurs* and *how to investigate*, not the final patch.  
- **Explicit guardrail:** Clear “do not provide the full corrected code or final solution.”  
- **Student‑first pedagogy:** Uses hints, questions, and experiments to build independence.

---

## ✅ Submission Checklist
- [x] Prompt is clear, specific, and well-structured  
- [x] Reasoning is thoughtful and well-articulated  
- [x] Includes reasoning answers (tone/style, balance, learner adaptation)

---

## ⚙️ Setup Instructions (Repo Use)
1. Keep this `README.md` and `PROMPT.txt` in the repository root.  
2. (Optional) Use `PROMPT.txt` directly when configuring an AI assistant or prompt tool.

---

## 📤 How to Submit
### Option A — GitHub (recommended)
1. Create a **public** GitHub repository (e.g., `python-screening-task-2`).  
2. Add `README.md` and `PROMPT.txt`.  
3. Commit & push:
   ```bash
   git add README.md PROMPT.txt
   git commit -m "Add debugging prompt and reasoning"
   git push origin main
   ```
4. Email the repo link to **pythonsupport@fossee.in**.

### Option B — Google Drive
1. Create a folder with `README.md` and `PROMPT.txt`.  
2. Set link sharing to **Anyone with the link — Viewer**.  
3. Email the Drive link to **pythonsupport@fossee.in**.

---

## 📎 Files Included
- `README.md` — Prompt + full reasoning + submission steps  
- `PROMPT.txt` — The standalone prompt text
