# Memory System Update

**Objective:** Introduce long-term and short-term memory systems to enhance the AI's conversational context and personalized interactions.

---

## New Features (v2.5.2)

### Long-Term Memory
- Stores user-specific facts and relationships persistently across sessions
- Allows adding and retrieving facts per user
- Maintains a “friends” list and metadata (creator information)
- Memory is saved in a JSON file for durability and future retrieval
- Enables the AI to recall previous interactions, making conversations feel continuous

### Short-Term Memory
- Maintains context for recent interactions during a session
- Stores the last few user-bot exchanges (configurable number of turns)
- Builds dynamic context summaries to inform AI responses
- Automatically discards oldest entries to keep memory buffer concise

---

## Version 2.5 Update — 2.5.2

### Added: Memory System
This update introduces a dual-memory system that allows the AI to:
- Remember user-specific information over multiple sessions (long-term memory)
- Keep track of ongoing conversation context (short-term memory)
- Provide more natural, personalized, and coherent responses

---

## Patch Notes

### v2.5.2 — Memory System

#### Features
- **Long-Term Memory:** JSON-based persistent storage of facts, friends, and metadata
- **Short-Term Memory:** Session-level buffer of recent conversation turns
- Context-aware responses leverage both memory systems
- Adds foundation for future enhancements such as adaptive behavior and personalized interactions

**This update significantly improves conversation continuity, personalization, and user experience.**
