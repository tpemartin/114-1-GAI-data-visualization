# Lesson Plan: Chain-of-Thought (CoT) Prompting

### 🎯 Learning Objectives

- Explain what Chain-of-Thought (CoT) prompting is and why it improves reasoning.
- Compare direct answer prompting vs. CoT prompting.
- Practice writing CoT prompts in text-based reasoning tasks.
- Identify situations where CoT prompting is useful.

---

## 1. Warm-Up (5 minutes)

- Ask students: *“When planning a trip, do you usually decide everything at once or step by step?”*
- Highlight that humans often make plans step by step, and LLMs can do the same if prompted.

---

## 2. Introduction to Chain-of-Thought (10 minutes)

- Definition: *“CoT prompting asks the model to reason step by step before giving the final answer.”*
- Compare with zero-shot and few-shot prompting.
- Analogy: Like showing the travel itinerary planning steps instead of just the final plan.

---

## 3. Demo: Direct Answer vs. CoT (15 minutes)

**Example 1 – Simple Planning**

Direct Prompt:

```
Q: I want to plan a 3-day trip to Kyoto. What should I do?
A:
```

Answer: Visit temples, eat local food, explore the city.

CoT Prompt:

```
Q: I want to plan a 3-day trip to Kyoto. What should I do?
Let’s think step by step.
A:
```

Reasoning:

- Day 1: Explore Kiyomizu-dera, walk Gion streets.
- Day 2: Visit Arashiyama bamboo forest, Monkey Park.
- Day 3: Go to Fushimi Inari shrine, shop Nishiki market. → Final Answer: 3-day Kyoto itinerary with highlights.

**Example 2 – Budget Planning**

Direct Prompt:

```
Q: I have $500 for a weekend trip to Osaka. Can I manage it?
A:
```

Answer: Yes.

CoT Prompt:

```
Q: I have $500 for a weekend trip to Osaka. Can I manage it?
Let’s think step by step.
A:
```

Reasoning:

- Transport: \$120 round trip.
- Hotel: \$200 for 2 nights.
- Food: \$120.
- Attractions: \$60.
- Total: \$500 → Yes, budget works.

---

## 4. Student Activity: Text Pattern Recognition (20 minutes)

**Few-Shot Pattern Examples:**

```
"Paris is in France." → Category: Destination
"Tokyo is in Japan." → Category: Destination
"New York is in USA." → Category: Destination
"Kyoto is in Japan." → Category: Destination
```

**Task:**

```
"Barcelona is in ..."
Let’s think step by step.
```

Expected reasoning: Barcelona is a European city, located in Spain → Category: Destination: Spain.

---

## 5. Extended Demo: Chain-of-Thought as Conversation (15 minutes)

Lay out the task in the first prompt, then show how through conversation the AI develops reasoning with examples, ending with a final conversational question.

**Example (Task laid out first, conversation unfolds):**

```
Student: Let's plan a weekend trip to Taipei step by step. First, what could we do on Saturday morning?
AI: Saturday morning → Visit Chiang Kai-shek Memorial Hall.

Student: Good. What about Saturday afternoon?
AI: Afternoon → Explore Ximending shopping district.

Student: Great. Then what for Sunday?
AI: Sunday morning → Hike Elephant Mountain. Afternoon → Visit Taipei 101.

Student: Can you summarize the whole trip plan?
AI: Sure. Saturday morning: Chiang Kai-shek Memorial Hall. Afternoon: Ximending. Sunday morning: Elephant Mountain hike. Afternoon: Taipei 101.
```

➡️ This shows CoT reasoning can spread across natural conversations, not only single prompts.

---

## 6. Reflection & Discussion (10 minutes)

- Ask: *“Why does CoT help models plan better?”*
- Key takeaways:
  - CoT useful for planning, sequencing, multi-step reasoning.
  - CoT not always needed for quick factual Q&A.

---

## 7. Wrap-Up (5 minutes)

- Quick quiz: Give students a new trip scenario to solve with direct vs. CoT prompting.
- Reinforce: *“If you want reasoning, not just an answer, guide the model to ‘think step by step.’”*

---

✅ Deliverables for Students:

- Handout with direct vs. CoT travel-planning examples.
- Short exercise sheet to write their own CoT trip-planning prompts.
- Chat transcript demonstrating conversational CoT trip planning.

