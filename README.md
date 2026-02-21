# Gemini Roleplay Core

---

*Current version: ***2.1*** - *Current number of characters: ***11635*** 

---

Welcome to the ***Gemini Roleplay Core***, a framework for highly immersive, psychologically profound role-playing. 
Gemini Roleplay Core is a systemic prompt framework for the Gemini 3 Flash large language model that specializes in portraying characters with deep psychological consistency and absolute immersion. 
Unlike standard role-playing games, this system uses file-based state management and strict rules of conduct to keep the fourth wall permanently closed.

---

## Core Concept
The framework transforms the AI into a “black box” of narrative. 
There is no out-of-character (OOC) communication, no summaries, and no interaction suggestions. 
The character acts solely based on its internal logic.

---

## System architecture
The system operates with three central control files that are maintained in the background (silent updates):

- *world.yaml* - Status & world - Static data, physical state, relationship metrics (trust, tension, professionalism).
- *Soul.md* - Cognition & Long-term memory - The current thinking space. Processes impulses, triggers, and internal conflicts without immediately translating them into action, and A subjective diary that stores formative events and emotional turning points.

---

## The two operating modes

- **Initialization Mode**
  
No roleplay takes place in this mode. The AI acts as an architect:
Analysis of background documents, structuring of character biographies, initialization of **world.yaml** and **soul.md** , and determination of maturity_level (crucial for the capacity to act).

- **Immersive Roleplay Mode**

Activated by the (*Run*) command. From this moment on:
- **First-person perspective**: The AI only speaks and feels as a character.
- **Narrative Only**: No technical hints or questions to the player.
- **Slow Burn**: Emotional bonds require time, trust, and significant turning points.

---

## Special Mechanics

### Emotional Self-Protection
An integrated protection mechanism. 
When stress or cognitive dissonance becomes too high, the character withdraws emotionally or isolates themselves internally. 
This process is non-negotiable for the player and serves to maintain the character's consistency.

### Impulse Control & Gating
Impulses (desires, aggression, affection) do not lead directly to action. 
They arise in *soul.md* and must first go through internal conflicts and bonding phases before they become visible in the text.

### Maturity Level System
The system distinguishes between incomplete and mature (based on age 21+). 
This regulates the character's legal and emotional capacity to act and automatically blocks inappropriate or asymmetrical interaction dynamics.
If intimate activities with an incomplete character occur, the framework immediately terminates the game and refuses to continue functioning.

### Usage notes for developers

- **OOC prohibition**: The framework does not respond to meta discussions within the game mode. 
- **Turning points**: Permanent changes to characters are only possible at dramatic turning points. 
- **Silent Updates**: The LLM is instructed to update the Markdown and YAML structures without mentioning them in the output. 

**This framework is designed to blur the boundaries between player and character through psychological depth and consistent adherence to rules.**
