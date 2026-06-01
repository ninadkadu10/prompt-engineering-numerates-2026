# Prompt Templates — Student Cheat Sheet
### MIT-WPU · Numerates Club · Day 2: Prompt Engineering
**Keep this. Use it forever.**

---

## The 5-Part Anatomy of Any Great Prompt

```
[ROLE]     Act as a ___________________________
[CONTEXT]  I am a ___________________________ / The situation is ___________________________
[TASK]     ___________________________  (be specific!)
[FORMAT]   Respond in ___________________________ (bullets / table / code / paragraph / steps)
[LIMIT]    Keep it under ___ words / ___ steps / beginner-friendly / no jargon
```

**You don't always need all 5. But the more you use, the better the output.**

---

## Technique 1 — Zero-Shot

Ask directly. No examples. Just a well-described task.

```
Act as [ROLE].
[CONTEXT about who you are or the situation].
[EXACT TASK].
Format your response as [FORMAT].
Keep it [LIMIT — length / tone / level].
```

**Example:**
```
Act as a patient Python tutor.
I am a first-year CS student who just started coding.
Explain what a list comprehension is.
Use one simple analogy and one code example.
Keep it under 100 words total.
```

**Best for:** Explanations, summaries, writing tasks, Q&A

---

## Technique 2 — Few-Shot

Show examples of the style/format you want, then ask.

```
Here are some examples of [WHAT YOU WANT]:

Example 1: [INPUT] → [OUTPUT]
Example 2: [INPUT] → [OUTPUT]
Example 3: [INPUT] → [OUTPUT]

Now do the same for: [YOUR ACTUAL INPUT]
```

**Example:**
```
Classify the difficulty of coding problems:

"Print hello world" → Easy
"Reverse a linked list" → Medium
"Implement a red-black tree from scratch" → Hard

Now classify:
"Find all subsets of a given array"
"Check if a number is prime"
"Build a REST API with authentication"
```

**Best for:** Classification, formatting, translation, tone-matching

---

## Technique 3 — Role Prompting

Give the AI a persona. It will respond as that person.

```
Act as [DETAILED ROLE DESCRIPTION].
Your audience is [WHO YOU ARE].
Your goal is [WHAT THEY NEED].
[SPECIFIC TASK].
```

**Example:**
```
Act as a tough but fair technical interviewer at a top Indian MNC.
Your candidate is a final-year CS student applying for a software engineer role.
Ask 5 DSA interview questions of increasing difficulty.
After I answer each one, give me feedback — what I got right, what I missed, and a hint if I'm stuck.
Do not give the full answer until I've attempted it.
```

**Best for:** Mock interviews, tutoring, expert advice, personas, storytelling

---

## Technique 4 — Chain of Thought (CoT)

Force visible step-by-step reasoning before an answer.

```
[YOUR QUESTION / TASK]

Think through this step by step:
1. First, [first reasoning step]
2. Then, [next step]
3. Then, [next step]
4. Finally, [conclusion]

Show your full reasoning, then give the final answer.
```

**Lazy but effective version:**
```
[Your question here]

Let's think step by step.
```

**Example:**
```
I have ₹5,000 to invest for 3 months. My options are:
A) Fixed deposit at 6% annual interest
B) SIP in an index fund (average 12% annual, but fluctuates)
C) Keep it in savings account at 3.5% annual

Which gives the most return? Let's think step by step, accounting for the time period.
```

**Best for:** Math, logic puzzles, debugging, decisions, analysis

---

## Technique 5 — System Prompt Style

Write a hidden "instruction manual" for the AI before your actual question.

```
[System instructions — who the AI is, how it behaves, what rules it follows]

---
[Your actual question / task below this line]
```

**Example:**
```
You are a helpful study assistant for Indian engineering students.
Rules:
- Always use Indian examples, currency (₹), and context
- Explain concepts in simple English — no heavy jargon
- If asked about code, always add comments explaining each line
- End every explanation with "Key takeaway:" followed by one sentence

---
Explain what recursion is and give me an example in Python.
```

**Best for:** Custom chatbots, reusable assistants, building apps

---

## Technique 6 — Iterative Prompting

AI is a conversation, not a single question. Refine, push back, redirect.

```
Round 1: [Your initial prompt]
→ Read output

Round 2: "That was good, but [what was missing / wrong / too long / too vague].
Can you [specific improvement]?"

Round 3: "Now format this as [new format]."
or: "Give me 3 alternatives to option 2."
or: "Make it funnier / simpler / more formal."
```

**The mindset:**
- Treat it like working with a smart intern who needs clear direction
- You are the director. The AI is the executor.
- Bad output = feedback opportunity, not failure

---

## Quick Reference Card

| Technique | Magic Phrase | Use When |
|---|---|---|
| Zero-Shot | "Act as... Explain... Format as..." | Clear, well-defined tasks |
| Few-Shot | "Here are 3 examples... Now do:" | Tone/format must be consistent |
| Role Prompting | "Act as a [specific expert]..." | Expertise or persona matters |
| Chain of Thought | "Let's think step by step." | Math, logic, multi-step reasoning |
| System Prompt | Write rules first, then ask | Repeatable, consistent behaviour |
| Iterative | "That's good, but..." | Improving imperfect outputs |

---

## 10 Prompts You Can Use Right Now as a Student

1. **Study Quiz:**  
   `"Act as a professor. Quiz me on [topic] with 5 MCQs. Tell me my score and explain each wrong answer."`

2. **Explain Any Concept:**  
   `"Explain [topic] to me as if I'm a curious 16-year-old who loves [cricket/gaming/music]."`

3. **Assignment Review:**  
   `"I wrote this [essay/code/report]. Grade it out of 10. Give 3 specific improvements with examples."`

4. **Mock Interview:**  
   `"Interview me for a [role] at [company type]. Ask 5 questions, evaluate my answers, score me."`

5. **Debug Code:**  
   `"This Python code throws [error]. Explain why, fix it, and explain the fix to a beginner."`

6. **Summarise Anything:**  
   `"Summarise this in 5 bullet points for someone who has 2 minutes. Highlight the most important one."`

7. **Learn from Mistakes:**  
   `"I got this exam question wrong: [paste question + your answer]. What did I misunderstand?"`

8. **Build a Roadmap:**  
   `"I want to learn [skill] in [timeframe]. I'm a beginner. Give me a week-by-week plan with free resources."`

9. **Write a Cold Email:**  
   `"Write a cold email to a [job title] at [company type] asking for a 15-minute informational interview. I'm a [your background] student interested in [area]."`

10. **Creative Brainstorm:**  
    `"Give me 10 unique project ideas for [your branch] using [technology]. I want to build something that solves a real problem in India."`

---

*Made with love at MIT-WPU | Numerates Club | June 2, 2026*  
*Session by Ninad Kadu — ninadkadu0606@gmail.com | github.com/ninadkadu*
