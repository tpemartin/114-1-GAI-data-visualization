# Lesson Plan: Introduction to Prompting & Chain-of-Thought Prompting

## 1. Warm-up: Imagining AI as an Assistant
- Ask students: *“If you could design your own AI assistant, what kind of assistant would you wish to have?”*
- Collect a few responses to activate imagination and motivation.
- Highlight how prompting is the way we communicate with AI assistants.

## 2. What is Prompting?
- Define prompting: giving instructions to AI to get useful outputs.
- Show simple examples of AI responses to short instructions.
- Emphasize: good prompts = better outputs.

## 3. Zero-shot Prompting
- **Explanation**: Giving a task without examples.
- **Demo**:
  > "Sort these items into categories: Apple, Carrot, Salmon, Rose."
  - Expected AI response: Fruit, Vegetable, Animal, Plant.
- Task for students: Try their own zero-shot prompt on a new set of items.
- **Survey**: 你的zero-shot prompt

## 4. Few-shot Prompting
- **Explanation**: Guiding the AI with examples.
- **Demo**:
  > "Apple is a fruit. → Category: Happy  
  > Carrot is a vegetable. → Category: Sad  
  > Salmon is a fish. → Category: Sad  
  > Rose is a flower. → Category: Sad  
  > Banana is a ..."
- Students observe how AI follows the pattern of labeling fruit as *Happy* and all others as *Sad*.
- **Practice**: Provide another list for students to test with this kind of pattern recognition.
- **Survey**: 你的few-shot prompt

## 5. Chain-of-Thought Prompting
- **Explanation**: Asking the AI to reason step by step before giving the final answer.
- **Demo** (Trip Planning context):
  > "I want to plan a 5-day trip. Think step by step: first list must-see places, then arrange them by location to minimize travel, then propose a daily plan."
- Show how AI reveals its reasoning before producing the itinerary.
- **Survey**: 分享你的chain-of-thought prompt

## 6. Prompting as a Conversation
- Show that prompting is not only one-shot but can spread naturally over a chat.
- Demonstrate how few-shot and chain-of-thought techniques can be woven into conversations.
- **Demo Example (Trip Planning)**:
  1. *Student*: "Plan a 3-day trip to Kyoto."
  2. *AI*: Suggests a draft itinerary.
  3. *Student*: "Make sure there’s tea time in the afternoon. For example, Day 1 has a tea break at 3 pm. → Category: Required."
  4. *AI*: Adjusts plan to include tea breaks, recognizing the example pattern as a few-shot style cue.
  5. *Student*: "Now, think step by step: list all kid-friendly places first, then arrange them into the plan."
  6. *AI*: Uses chain-of-thought reasoning to explain its steps and updates the plan with kid-friendly activities each day.
- Highlight: prompts can build step by step into a refined result, combining conversational flow with few-shot and chain-of-thought prompting.

## 7. Practice (Student Task)
- Students work on their own travel-planning prompt:
  - Start with a general task.
  - Refine through conversation.
  - End with a chain-of-thought style request.
- Example progression:
  1. “Plan a 2-day trip to Tainan.”
  2. Add preferences (food, culture, relaxation).
  3. Ask for reasoning: “Explain why each activity is placed in that order.”
- **Survey**: 分享你與AI的聊天過程 [How to create a sharable link? Ask AI]

## 8. Wrap-up & Sharing
- Students share their final chat with AI (conversation transcript).
- Instructor gives feedback on how effectively prompts guided the AI.
- Key takeaway: prompts can be improved step by step—from zero-shot to few-shot, to chain-of-thought reasoning, to conversational refinement.

