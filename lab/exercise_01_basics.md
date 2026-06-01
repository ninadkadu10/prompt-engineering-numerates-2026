# Exercise 1 — Vague vs Specific Prompting
### MIT-WPU · Numerates Club Workshop · Day 2: Prompt Engineering
**Lab Session | June 2, 2026 | 1:00 PM – 1:30 PM**

---

## The Big Idea

> "A bad prompt is like a bad Google search — you get something, but not what you needed."

The quality of your AI output is **directly proportional** to the quality of your input.  
This exercise will make you *feel* that difference in under 20 minutes.

---

## How This Works

1. Each task below has a **Vague Prompt** already written for you.
2. You will **run the vague prompt** in ChatGPT and note what you get.
3. You will then **write an improved prompt** using the 5-part anatomy:
   - **Role** → who should the AI be?
   - **Context** → what's the situation?
   - **Task** → what exactly do you want?
   - **Format** → how should the answer look?
   - **Constraints** → length, tone, level, etc.
4. Run your improved prompt and compare.
5. Discuss with the person next to you — who got the better output?

---

## Task 1 — Explain a Concept

### Vague Prompt (run this first)
```
Explain machine learning.
```

**What did you get?** *(jot it down)*

> _______________________________________________
> _______________________________________________

**Was it:**  [ ] Too long   [ ] Too technical   [ ] Too simple   [ ] Actually useful

---

### Now Write Your Improved Prompt

Use the template below. Fill in every blank.

```
Act as [ROLE: e.g. a patient professor / friendly tutor].
I am [CONTEXT: your background — 1st year CS student / 12th grade student].
Explain [TOPIC] using [ANALOGY TYPE: a cooking analogy / a cricket analogy / etc.].
Keep it under [WORD COUNT] words and use [FORMAT: bullet points / short paragraphs].
End with one real-world example I can relate to as a student in India.
```

**Your improved prompt:**

> _______________________________________________
> _______________________________________________
> _______________________________________________

**What changed in the output?**

> _______________________________________________

---

## Task 2 — Write Something for Me

### Vague Prompt (run this first)
```
Write a cover letter.
```

**What did you get?**

> _______________________________________________

**Problem with this output?**

> _______________________________________________

---

### Now Write Your Improved Prompt

```
Act as a professional career coach with experience in the Indian tech industry.
I am a [YOUR BRANCH] student at MIT-WPU, Pune, graduating in [YEAR].
Write a cover letter for an internship application at [COMPANY TYPE: a startup / MNC / AI company].
Highlight these skills: [LIST 2-3 SKILLS YOU HAVE].
Keep it under 250 words. Tone should be professional but not robotic.
End with a confident closing line.
```

**Your improved prompt:**

> _______________________________________________
> _______________________________________________
> _______________________________________________

**Output score (out of 10):** ___   **Would you actually use this letter?** [ ] Yes  [ ] No  [ ] After edits

---

## Task 3 — Debug / Explain Code

### Vague Prompt (run this first)
```
Fix my code.
```

*(ChatGPT will ask for the code — it can't read your mind. Note this.)*

**What happened?**

> _______________________________________________

---

### Now Write Your Improved Prompt

Copy-paste this broken Python code into your prompt:

```python
def calculate_average(numbers):
    total = 0
    for num in numbers:
        total = total + num
    return total / len(numbers)

result = calculate_average([])
print(result)
```

**Your improved prompt (wrap the code inside it):**

```
Act as a Python mentor teaching a beginner.
The following Python code crashes when given an empty list.
[PASTE THE CODE HERE]
Explain:
1. Why it crashes (in simple terms)
2. How to fix it with a code example
3. One general rule to always follow to prevent this type of bug
Keep the explanation simple enough for someone who just started Python.
```

**What was different about the output vs just asking "fix my code"?**

> _______________________________________________
> _______________________________________________

---

## Reflection (discuss with your neighbour)

| Question | Your Answer |
|---|---|
| Which task showed the biggest improvement? | |
| What ingredient (Role/Context/Task/Format/Constraint) helped most? | |
| Would you use AI differently for assignments after this? | |

---

## Key Takeaway

> **Vague in → Vague out.  
> Specific in → Specific, useful, and often surprising out.**

Prompting is a skill. You just started practising it. Now let's go deeper → **Exercise 2**
