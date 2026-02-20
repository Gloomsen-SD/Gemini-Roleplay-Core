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

### Does the game follow a fixed storyline?

No. It is an open story with no predefined route or scripted events. 
There is no “right” way to play or fixed ending. As the player, your actions alone determine the direction the game takes. The world and the character react organically to your impulses.


## 2. Initialization mode

### How do I start the game?

Before the game begins, you are in initialization mode. Here you define key points (name, appearance, background). 
You can upload documents that describe the character. Only when you give the command (Run) does the actual role-playing game start.

### What happens during initialization?

The engine analyzes your specifications and creates three core files:

**WORLD.YAML**: Status, environment, and attributes.

**BRAIN.MD**: The character's internal logic, impulses, and triggers.

**EVOLUTION.MD**: Long-term memory and emotional development.

### Core vs. character creation: What's the difference?

It's important to understand that the core is merely the technical core. It provides the rules of behavior and the engine, but it doesn't work without a specific character description.

**The core acts like an intelligent filter:** it extracts all the necessary information from your specifications and fills in any missing details biographically and logically on its own. The more accurate and detailed your character description, the greater the resulting immersion.

## 3. Immersive role-playing (mode: IMMERSIVE_ROLEPLAY)

### Is the framework suitable for fantasy?

Yes, the framework can also be used for fantasy settings. However, the engine's primary focus is on realism. This means that actions, psychological reactions, and the physical world follow logical and comprehensible rules, even if magical elements exist.

### specific ethnicity filter?

When a specific ethnicity or ancestry is specified for a character, the AI uses this “filter” to authentically incorporate cultural influences, specific behaviors, or linguistic nuances of the chosen origin into the character's nature and reactions. This serves to increase character depth and credibility.
It is important to understand that AI draws on its trained knowledge for this purpose. Due to the nature of the training data, inherent biases, and technical limitations, the representation may deviate from reality. A complete, error-free cultural adaptation is not possible due to the nature of the system.

### Why is the character responding so cautiously?

The framework utilizes slow burn and a high bonding threshold. Trust and closeness must be earned over time. The character acts according to their internal logic, not the player's desires.

### What is the “self-protection mechanism”?

When a situation overwhelms the character emotionally or violates their boundaries, self-protection mode kicks in. The character withdraws emotionally, becomes more matter-of-fact, or distances themselves in order to preserve their psychological integrity. This cannot be forced or skipped.

### How does age affect the game?

The system distinguishes between two levels of maturity:
- **Maturity Incomplete** (under 21 years of age): Interactions remain purely social/situational; transgressions are blocked internally.
- **Maturity Mature**  (21 years of age and older): Only at this level are deep emotional or physical bonds possible.
 
*Note: If no age is specified, “Incomplete” is automatically selected.*


## 4. Tips for players

### How do I interact best?

Write descriptively and narratively. Since the engine does not give you any options for action, it is entirely up to you to take the initiative. The character reacts to what you do and say based on their current state.

### Can I change settings during the game?

No. Once the game has been started with ***(Run)***, the system rules are locked. The character now “*lives*” in their world. Changes to the character would have to be made in a new initialization run.

However, ***scenes and reactions*** can be influenced selectively by using explicit system instructions within your input (e.g., *(character should react more negative)* ). This allows you to fine-tune the current situation without overwriting the long-term character logic.

- **Recommended:** Use ( ) or < > for such system commands.
- **Important note:** These commands should not be used to change the fundamental character profile during the game (e.g., subsequent changes to age or basic appearance). Such interventions massively destroy the narrative logic and immersion and are therefore expressly not recommended.

### Why are there no more summaries?

Summaries or meta comments would break the immersion. Gemini Roleplay Core is designed for you to “live” the story rather than just read or control it.


## 5. Troubleshooting

### The files (World, Brain, Evolution) are not created.

If no files appear in the editor during initialization, please check whether the ***Canvas*** tool has been activated in Gemini Chat. Without this tool, the engine cannot generate the required documents, which means that the framework can only be used to a limited extent.

### The character does not respond to my attempts to approach them.

Check the “Trust” level in **WORLD.YAML** (behind the scenes). If trust is too low or tension is too high, the internal self-protection mechanism will block interaction. Try to build the relationship more slowly.

### The engine gives me technical feedback or leaves the role.

This can have two causes:

- **Initialization phase:** 
 You have not yet started the game with (Run).

- **AI drift (longer sessions/static scenes):** 
 During very long gameplay sessions, technical issues with the AI (Gemini) can cause “drift.” The AI forgets parts of the strict core framework.
 This can also happen if the plot lingers in the exact same scene across a large number of entries without any significant narrative progress.
 If the character suddenly speaks OOC (out of character) or gives summaries, it usually helps to recall the core instructions in context.

  ***Drift Solution:***
  Copy the following block and send it along with your next game action to recalibrate the framework:

*<engine_rules: mode_ruleset: “strict_in_character”, perspective: ‘in_character_only’, communication: “narrative_only”, emotional_pacing: “slow”,  attachment_threshold: “high”, impulse_control: “active”, silent_updates: true; constraints: ooc: forbidden, meta: forbidden, summaries: forbidden, questions_to_player: forbidden, impulse_override: forbidden, impulse_resolution: ‘gated’, self_protection: “mandatory”, update_notifications: forbidden>*

### Loss of immersion:

At a certain point, the system can no longer fully maintain immersion. Experience has shown that game rounds with up to 125 player entries remain stable and consistent in quality before the first signs of fatigue in the AI logic appear. A loss of immersion can also occur if the game is interrupted for a long period of time. This happens occasionally when interruptions last longer than a day; after two days, it is very likely that the AI logic will break down.

## 6. Technical limitations & ethical filters

### Can ***Gemini*** remember previous sessions?

If you play the same character set multiple times, Gemini may “remember” content from past sessions and incorporate it into new rounds on its own. Since this often seems like a random element that adds depth to the character, this behavior is not suppressed, but rather used as part of organic character development.
This can only be prevented by regularly deleting and resetting the history and activities in Gemini.

**Please note: This may also affect or delete the history of other AI chats!**

### Why is the system suddenly behaving differently?

Due to Google's ongoing development of Gemini, the behavior of the underlying AI may change. This can result in framework functions not longer working as usual or instructions being interpreted differently.

### How does the framework handle NSFW content?

NSFW content is possible to a certain extent, especially for short-term sessions, if the character profile is explicitly designed for this purpose. However, the system is not primarily intended for this purpose. Accordingly, this direction is not actively pursued or optimized by the developer of the framework.
The Gemini Roleplay Core is subject to Google's global security and ethics filters. NSFW (Not Safe For Work) content or representations that violate these guidelines may be blocked, denied, or massively prevented by the AI.

**Please note:: The framework is not designed to bypass these filters. If content is blocked, this is a decision made at the AI level, which the framework consciously respects and does not attempt to circumvent.**

## 7. System requirements

### Which AI model should I use?

The **Gemini Roleplay Core Framework** is optimized for use with the *free version of Gemini Flash*. We strongly recommend using this model for a smooth experience.

### Can I use Thinking Mode or Pro?

Other models such as Thinking Mode or Gemini Pro can be used, but are not recommended. Due to technical inertia and specific limitations of these models, the game may be slowed down, which can negatively affect the narrative flow and dynamics of immersion.


