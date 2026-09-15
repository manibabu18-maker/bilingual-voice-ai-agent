# bilingual-voice-ai-agent
# Autonomous Bilingual AI Voice Sales Specialist

An end-to-end, ultra-low latency voice agent designed for outbound sales qualification and real-time CRM actions, supporting seamless bilingual code-switching between English and Telugu.

## 🚀 Live Demo & Virtual Line
- **Inbound Line:** `+1 (586) 207-3198`
- **Web Demo:** [Insert your Vapi Demo Link here]

## 🛠️ Architecture & Tech Stack
- **Orchestration & Telephony:** Vapi.ai / Virtual SIP Inbound
- **Speech-to-Text (STT):** Soniox Multilingual (Real-time automatic language identification)
- **Large Language Model (LLM):** OpenAI GPT-4o (Intent classification & Function calling)
- **Text-to-Speech (TTS):** Cartesia Sonic Multilingual (`Aadhya` voice profile)
- **Latencies:** TTS ~260ms | STT ~410ms | Total round-trip ~1.3s

## ⚡ Key Features
- **Dynamic Bilingual Code-Switching:** Seamlessly switches between English and Telugu depending on the customer's conversational language without prompt resets.
- **Agentic Tool Calling:**
  - `send_whatsapp_brochure`: Automatically triggers webhook delivery for HOT leads during the call.
  - `schedule_callback`: Captures preferred callback windows for WARM leads.
- **Sub-1.4s Latency Pipeline:** Tuned speech chunking and turn-taking models to maintain natural human-like voice pacing.

## 📂 Repository Contents
- `system_prompt.txt`: Core agent personality, context boundaries, and language rules.
- `tools_schema.json`: OpenAPI/JSON schema definitions for tool-calling integration.
