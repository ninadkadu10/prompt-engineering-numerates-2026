# Exercise 2 — Prompt Patterns
### MIT-WPU · Numerates Club Workshop · Day 2: Prompt Engineering
**Lab Session | June 2, 2026 | 1:30 PM – 2:00 PM**

---

## The Big Idea

Same task. Three different prompting techniques. Completely different results.  
This exercise teaches you to **choose the right tool for the job**.

---

## The 3 Techniques You'll Use Today

| Technique | One-Line Definition | When to Use |
|---|---|---|
| **Zero-Shot** | Just ask, no examples given | Clear tasks, simple formats |
| **Few-Shot** | Give 2–3 examples, then ask | When tone/format matters a lot |
| **Role Prompting** | Tell AI who to be | When expertise or personality matters |

---

## Pick Your Branch

Choose the track that matches your background before starting:

- [ ] **Track A — CS / AIML** (coding, tech, data)
- [ ] **Track B — AIDS / BCA** (data, analytics, business tech)
- [ ] **Track C — BSc / General** (science, mathematics, open interest)

You'll use your branch context in the prompts below.

---

## Task — Explain "What is an API?"

*(An API — Application Programming Interface — is how two apps talk to each other.  
You don't need to know this deeply. That's the AI's job.)*

---

### Technique 1: Zero-Shot

Write a zero-shot prompt. No examples. Just a clear ask.

**Your prompt:**

```
Act as _________________________ [pick a role].
I am _________________________ [your context: branch, year, background].
Explain what an API is _________________________ [specific angle].
Format: _________________________ [bullets / paragraph / analogy].
Keep it under _________________________ words.
```

**Copy-paste your final prompt here:**

> _______________________________________________
> _______________________________________________

**Rate the output (circle one):**  1  2  3  4  5  6  7  8  9  10

**What was missing from the output?**

> _______________________________________________

---

### Technique 2: Few-Shot

Now guide the AI by providing examples of the *style* you want.

**Your prompt (fill in the examples):**

```
Explain technical concepts using simple real-world analogies, like these examples:

Concept: Database
Analogy: A database is like an Excel sheet for your entire school — every student,
every grade, every subject stored in organized rows and columns.

Concept: Encryption
Analogy: Encryption is like a secret language you and your friend made up in school —
only the two of you can understand it.

Now explain: API
Use the same style. Target audience: _________________________ [your branch/year].
```

**Your output:**

> _______________________________________________
> _______________________________________________

**Compared to zero-shot, this output was:**  
[ ] More relatable  [ ] More accurate  [ ] About the same  [ ] Actually worse

**Why do you think that is?**

> _______________________________________________

---

### Technique 3: Role Prompting

Now give the AI a persona.

**Choose a role that makes sense for your track:**

- Track A: "Act as a senior software engineer interviewing a fresher"
- Track B: "Act as a startup CTO explaining tech to a non-technical investor"
- Track C: "Act as a science teacher explaining tech concepts to a BSc student"

**Your prompt:**

```
_________________________ [your chosen role + description].

Your goal: explain what an API is in a way that resonates with someone in my position.

My position: _________________________ [your branch, year, goals].

After the explanation, give me one example of how an API is used in
_________________________ [field relevant to YOUR branch — healthcare, finance, gaming, etc.].
```

**Your output:**

> _______________________________________________
> _______________________________________________

---

## Comparison Table

Fill this in after all three:

| Criterion | Zero-Shot | Few-Shot | Role Prompt |
|---|---|---|---|
| Relevance to me (1–5) | | | |
| Clarity (1–5) | | | |
| Would I share this? (Y/N) | | | |
| Best for this task? (pick one) | [ ] | [ ] | [ ] |

---

## Branch-Specific Bonus Round

Pick ONE task from your branch and apply ALL 3 techniques to it.

**Track A (CS/AIML):** Explain how a neural network learns (backpropagation — simplified).  
**Track B (AIDS/BCA):** Explain what data cleaning is and why it matters.  
**Track C (BSc/General):** Explain the difference between correlation and causation.

**Your chosen task:** _______________________________________________

**Which technique worked best for this specific task?** _______________________________________________

**Why?**

> _______________________________________________

---

## Takeaway

> **Zero-Shot** = Fast and direct. Works when you describe well.  
> **Few-Shot** = Reliable format and tone. Works when style matters.  
> **Role Prompting** = Specialist expertise on demand. Works when context matters.  

Mix and match. The best prompts often combine all three. → **Exercise 3**
