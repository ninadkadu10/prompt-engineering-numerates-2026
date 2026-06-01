# Exercise 3 — Chain of Thought Challenge
### MIT-WPU · Numerates Club Workshop · Day 2: Prompt Engineering
**Lab Session | June 2, 2026 | 2:00 PM – 2:20 PM**

---

## The Big Idea

> "The AI doesn't think unless you tell it to."

Chain of Thought (CoT) is a prompting technique where you ask the AI to **reason step by step** before giving an answer. This dramatically reduces mistakes on problems that require logic, math, or multi-step thinking.

**Magic phrase:** *"Let's think step by step."*

---

## How This Works

Each problem below has two rounds:

- **Round A** — Ask without CoT. Just a direct question.
- **Round B** — Ask WITH CoT. Add the magic phrase and structured reasoning prompts.

Compare the outputs. Notice what changes.

---

## Problem 1 — Math (Starter)

### Setup
A train departs from Mumbai at 9:00 AM travelling at **80 km/h**.  
Another train departs from Pune (distance = 160 km from Mumbai) at **10:00 AM** travelling toward Mumbai at **100 km/h**.  
At what time do they meet?

---

### Round A — Without CoT

**Prompt:**
```
A train leaves Mumbai at 9 AM at 80 km/h. Another leaves Pune (160 km away) at
10 AM at 100 km/h toward Mumbai. When do they meet?
```

**AI's answer:**

> _______________________________________________

**Is this correct?** [ ] Yes  [ ] No  [ ] Not sure  
*(Correct answer hint: they meet at approximately 10:44 AM)*

---

### Round B — With CoT

**Prompt:**
```
A train leaves Mumbai at 9 AM at 80 km/h. Another leaves Pune (160 km away) at
10 AM at 100 km/h toward Mumbai. When do they meet?

Let's think step by step:
1. First, calculate how far the Mumbai train travels before the Pune train starts.
2. Then calculate the remaining distance between them at 10 AM.
3. Then find the time for them to close that gap when moving toward each other.
4. Finally, add that to 10 AM to get the meeting time.
```

**AI's answer:**

> _______________________________________________

**Did the answer change?** [ ] Yes  [ ] No  
**Was the reasoning visible?** [ ] Yes  [ ] No  
**Which answer do you trust more? Why?**

> _______________________________________________

---

## Problem 2 — Logic Puzzle

### Setup
There are 5 students in a row: Aditya, Bhavna, Chirag, Deepika, and Esha.  
- Aditya is not next to Chirag.  
- Bhavna is between Aditya and Deepika.  
- Esha is at one end.  
- Chirag is not at either end.  

What is the order of students from left to right?

---

### Round A — Without CoT

**Prompt:**
```
5 students: Aditya, Bhavna, Chirag, Deepika, Esha.
Aditya not next to Chirag. Bhavna between Aditya and Deepika.
Esha at one end. Chirag not at either end.
What is the left-to-right order?
```

**AI's answer:**

> _______________________________________________

**Does the AI show its work?** [ ] Yes  [ ] No

---

### Round B — With CoT

**Prompt:**
```
5 students: Aditya, Bhavna, Chirag, Deepika, Esha.
Constraints:
- Aditya is not next to Chirag
- Bhavna is between Aditya and Deepika
- Esha is at one end
- Chirag is not at either end

Solve this step by step:
1. Start with what you know for certain (who is definitely at an end).
2. Apply each constraint one by one to narrow down possibilities.
3. Eliminate arrangements that violate any rule.
4. State the final order and verify it satisfies all constraints.
```

**AI's answer:**

> _______________________________________________

**Correct answer (check yourself):** Esha – Deepika – Bhavna – Aditya – Chirag  
*(or its reverse)*

**Observation:** Did CoT help the AI reason correctly?

> _______________________________________________

---

## Problem 3 — Creative + Open-Ended

### Setup
This one has no single "right" answer. The goal is to see how CoT structures *creative* thinking.

**Topic:** You are a startup founder. Your app idea is: "An AI-powered personal finance tracker for college students in India."  
You need to identify the 3 biggest risks this product faces.

---

### Round A — Without CoT

**Prompt:**
```
What are the 3 biggest risks for an AI-powered personal finance tracker app
for college students in India?
```

**AI's answer (note how it reasons):**

> _______________________________________________
> _______________________________________________

**Depth of reasoning:** [ ] Surface-level  [ ] Moderate  [ ] Deep and nuanced

---

### Round B — With CoT

**Prompt:**
```
You are an experienced startup advisor in India.
I am building an AI-powered personal finance tracker for college students in India.

Identify the 3 biggest risks. Think through this carefully:
1. First, consider the target user — what are their specific constraints and behaviours?
2. Then consider the Indian market context — regulations, data privacy, payment systems.
3. Then consider AI-specific risks — accuracy, trust, hallucination in financial advice.
4. Finally, rank the top 3 risks by likelihood AND impact.

For each risk, also suggest one mitigation strategy.
```

**AI's answer:**

> _______________________________________________
> _______________________________________________

**Which output would you actually use to build a business plan?**  [ ] Round A  [ ] Round B

---

## Reflection

| Question | Your Answer |
|---|---|
| In which problem did CoT make the biggest difference? | |
| Does CoT always help, or are there cases where it's overkill? | |
| What happens if you just add "Let's think step by step" at the end? Try it! | |

---

## The CoT Formula

```
[Normal prompt describing the task]

Think through this step by step:
1. Start with [first logical step]
2. Then [next step]
3. Then [next step]
4. Finally, [conclusion step]
```

**Or the lazy version that still works surprisingly well:**

```
[Your question here]

Let's think step by step.
```

---

## Takeaway

> CoT works because LLMs generate text left-to-right.  
> When you force visible reasoning, the model can "check its own work" as it writes.  
> It's not magic — it's just giving the model room to think before committing to an answer.

Ready for the fun part? → **Prompt Battle (Exercise 4)**
