# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
Simple UI, 
- List at least two concrete bugs you noticed at the start  
  (for example: "the secret number kept changing" or "the hints were backwards").

---
- The hint is doing the opposite. It tells you to go higher for a lower number and viseversa while it was supposed to do the opposite
- Inconsistant number of attempts. It says out of attempts even if there is 1 attempt left. when the game is run there are 7 attempts for normal difficulty , but when new game is run it says 8 attempts 
- Level difficulty is inconsistant. Range on hard is 1-50 and easy is 1-20. Hard was supposed to have the bigger range 1-50 and easy should be 1-20
- the range always take 1 -100 because it is hard coded insteade of depending on the difficulty level
- inputs are not filtered , incorrect inputs like letters or numbers out of range count as input and the attempt is counted instead of prompting the user to input the correct input
- even number guess are incorrectly compared with the target number because they are converted to string 

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)? 
 claude
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
The AI suggested that even number attempts are not compared with the target correctly,  we vertified that by refering to app.py file line 158 - 161

- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
It didn't suggest anything that was incorrect
--- 

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
- What change did you make that finally gave the game a stable secret number?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
