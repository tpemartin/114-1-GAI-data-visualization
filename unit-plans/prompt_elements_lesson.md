# Lesson: Key Elements of a Prompt

## 1. Warm-Up & Connection to Previous Lesson
- Recap last lesson: students experimented with zero-shot, few-shot, and chain-of-thought prompts.
- Transition: *“Even though the prompts looked different, they share common building blocks. Today we’ll explore those building blocks.”*

---

## 2. The Key Elements of a Prompt
Introduce four core elements:
1. **Role / Identity** – who the AI should act as.  
2. **Task / Instruction** – what needs to be done.  
3. **Context / Input Data** – the background or text to work on.  
4. **Format / Constraints** – how the answer should look.

---

## 3. Linking Back to Previous Prompts
- Zero-shot → mainly **task** only.
- Few-shot → **task + context** (examples).
- Chain-of-thought → **format** with reasoning steps.
- Activity: Students label past prompts with these elements.

---

## 4. Demo: Rebuilding a Prompt
**Basic Prompt:**  
> “Summarize this news article in English.”

Breakdown: Role (none), Task (summarize), Context (article), Format (English).

**Expanded Prompt:**  
> “You are a professional editor. Summarize the following article in English, focusing on the economic impact, and provide your answer as three concise bullet points.”

---

## 5. Challenge Task A: Economist Article (Text)
**Article:** [China’s 200m gig workers are a warning for the world](https://www.economist.com/leaders/2025/09/18/chinas-200m-gig-workers-are-a-warning-for-the-world)

### Activity
- Students design their own prompts using the 4 elements.
- Encourage variations:
  - Role: journalist, policymaker, teacher
  - Task: summary, policy memo, tweet
  - Context: focus only on risks, or lessons for other countries
  - Format: bullets, headline, short paragraph
- Pair-share: Which element changed the output most?


**Survey**: 折解範例prompt所對應的各個element

---

## 6. Challenge Task B: Economist Article (Text + Graphic)
**Article & Graphic:** [How to make sense of Donald Trump’s bizarre tariff rates](https://www.economist.com/graphic-detail/2025/08/15/how-to-make-sense-of-donald-trumps-bizarre-tariff-rates)


**Survey**: China’s 200m gig workers are a warning for the world的summary prompt

### Activity
- Students prompt the AI to explain the relationship between the **graphic** and the **article text**.
- Example prompt:
  > “You are a data visualization teacher. Read the article and describe how the chart supports or clarifies the text. Point out what makes the chart effective or confusing.”
- Encourage students to experiment:
  - Change **role** (teacher vs policymaker vs journalist).
  - Adjust **task** (explain the chart, critique it, propose improvements).
  - Control **format** (short essay, bullet critique, tweet thread).
- Reflection: *“What did you learn about what makes a visualization effective in supporting an article?”*



---

## 7. Wrap-Up
- Reinforce formula: **Prompt = Role + Task + Context + Format**.
- Key insight: prompts can also guide AI to evaluate **data graphics + text**, showing what makes visual communication effective.
- Preview: Next lesson → combining elements for domain-specific prompting (creative writing, professional analysis).

