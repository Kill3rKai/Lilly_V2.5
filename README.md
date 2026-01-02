# Lilly AI | Project VSM V2.5 Development Information Document Showing **Major** Updates And Patch Notes

[![Project Status: Active](https://img.shields.io/badge/Project%20Status-Active-brightgreen)](https://github.com/your-username/your-repo)
[![Version](https://img.shields.io/badge/Version-2.5-blue)](https://github.com/your-username/your-repo)

Lilly AI (Lilly AI Self Named) is a state-of-the-art virtual content creator developed for the **VSM** group by member Kill3rKai. Lilly V2.5 is designed to function as an autonomous AI VTuber capable of real-time audience interaction, personality-driven gaming, and dynamic live-stream content.

## 🌟 Overview
Lilly V2.5 represents a significant leap from previous iterations, focusing on reduced latency, more natural speech patterns, and a complex, stronger, filter system. Unlike standard chatbots, Lilly is optimized for the high-energy environment of live streaming.

## 🚀 Key Features
- **Personality Engine:** A custom Large Language Model (LLM) fine-tuned for the unique "Lilly" persona—balancing wit, curiosity, and VSM group inside jokes.
- **Dynamic Content Filter:** A multi-layered safety system that blocks prohibited content while generating character-appropriate "annoyed" or "sassy" responses when boundaries are hit.
- **Low-Latency TTS:** High-fidelity voice synthesis designed for real-time conversation.
- **Vision & Perception:** Ability to perceive stream events and react to visual stimuli, In order to play games and interact.
- **Avatar:** To Humanize It.
- **Browser:** It can Google search if it is unsure
- **Discord:** It can, Chat, DM, Talk in Voice Calls

## 🛠 Tech Stack
* **Language:** Python 3.10+
* **Core AI:** Mistral With Llama 3 Fallback
* **Voice:** W.I.P
* **Integration:** Discord currently
* **Avatar:** W.I.P

## 📂 Project Structure

The system is architected to separate the core AI logic from the persistent data and the external communication layers.

```text
AI_SYSTEM V2.5/
├── main.py                # Terminal Chat System
├── discord_bot.py         # Discord API Integration & Event Handling
├── requirements.txt       # Project Dependencies & Environment Specs
├── brain/                 # Core Intelligence & Logic
│   ├── controller.py      # System Orchestration & Logic Flow
│   ├── filters.py         # Content Moderation & Safety Logic
│   ├── generator.py       # LLM Inference & Response Construction
│   ├── intent.py          # User Intent Analysis & Classification
│   ├── longterm.py        # Logic For Deep Context Retrieval
│   ├── longterm_memory.json # Persistent Historical Data
│   ├── memory.py          # Short-term/Working Memory Management
│   ├── persona.py         # Character Trait Application Logic
│   ├── scorer.py          # Response Evaluation & Ranking
│   ├── session.json       # Current Active Session State
│   └── tools.py           # Utility Functions & Helper Scripts
└── data/                  # Static Assets & Configuration
    └── persona.txt        # Raw Character Data & System Prompting
