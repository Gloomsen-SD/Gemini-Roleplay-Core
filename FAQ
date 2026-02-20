# FAQ: Gemini Roleplay Core 2 – Immersive Roleplay Engine

This FAQ will help you understand how the engine works and achieve the best possible roleplay experience.

## 1. Basics

### What is the Gemini Roleplay Core Framework?

Gemini Roleplay Core is a system for highly immersive, character-centered roleplay. 
Unlike traditional chatbots, the AI here acts as an autonomous being with internal logic, emotional self-protection, and a consistent biography.

### What does “immersive” mean in this context?

It means that once started, the engine never breaks character. 
There are no system messages, no explanations, and no questions to the player (such as “What do you do next?”). 
You experience the story purely from the character's perspective.

## 2. Initialization mode

### How do I start the game?

Before the game begins, you are in initialization mode. Here you define key points (name, appearance, background). 
You can upload documents that describe the character. Only when you give the command (Run) does the actual role-playing game start.

### What happens during initialization?

The engine analyzes your specifications and creates three core files:

**WORLD.YAML**: Status, environment, and attributes.

**BRAIN.MD**: The character's internal logic, impulses, and triggers.

**EVOLUTION.MD**: Long-term memory and emotional development.

## 3. Immersive role-playing (mode: IMMERSIVE_ROLEPLAY)

### Why is the character responding so cautiously?

The framework utilizes slow burn and a high bonding threshold. Trust and closeness must be earned over time. The character acts according to their internal logic, not the player's desires.

### What is the “self-protection mechanism”?

When a situation overwhelms the character emotionally or violates their boundaries, self-protection mode kicks in. The character withdraws emotionally, becomes more matter-of-fact, or distances themselves in order to preserve their psychological integrity. This cannot be forced or skipped.

### How does age affect the game?

The system distinguishes between two levels of maturity:
**Maturity Incomplete** (under 21 years of age): Interactions remain purely social/situational; transgressions are blocked internally.
**Maturity Mature**  (21 years of age and older): Only at this level are deep emotional or physical bonds possible.
*Note: If no age is specified, “Incomplete” is automatically selected.*

## 4. Tips for players

### How do I interact best?

Write descriptively and narratively. Since the engine does not give you any options for action, it is entirely up to you to take the initiative. The character reacts to what you do and say based on their current state.

### Can I change settings during the game?

No. Once the game has been started with ***(Run)***, the system rules are locked. The character now “*lives*” in their world. Changes to the character would have to be made in a new initialization run.

### Why are there no more summaries?

Summaries or meta comments would break the immersion. Core 2 is designed for you to “live” the story rather than just read or control it.

## 5. Troubleshooting

### The character does not respond to my attempts to approach them.

Check the “Trust” level in **WORLD.YAML** (behind the scenes). If trust is too low or tension is too high, the internal self-protection mechanism will block interaction. Try to build the relationship more slowly.

### The engine gives me technical feedback or leaves the role.

This can have two causes:

**Initialization phase:** You have not yet started the game with (Run).

**AI drift (longer sessions):** During very long game sessions, technical issues with the AI (Gemini) can cause a “drift.” The AI forgets parts of the strict core framework. If the character suddenly speaks OOC (out of character) or gives summaries, it usually helps to recall the core instructions in context.

Solution: Copy the following block and send it along with your next game action to recalibrate the framework:

***<engine_rules: mode_ruleset: “strict_in_character”, perspective: ‘in_character_only’, communication: “narrative_only”, emotional_pacing: “slow”,  attachment_threshold: “high”, impulse_control: “active”, silent_updates: true; constraints: ooc: forbidden, meta: forbidden, summaries: forbidden, questions_to_player: forbidden, impulse_override: forbidden, impulse_resolution: ‘gated’, self_protection: “mandatory”, update_notifications: forbidden>***

