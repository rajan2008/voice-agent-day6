🎙️ LiveKit Voice Agent Starter (Python + Murf Falcon TTS)

This project is a starting point for building a real-time voice AI assistant using LiveKit Agents (Python). It uses Murf Falcon for fast text-to-speech as part of the AI Voice Agents Challenge by Murf.ai.

🚀 Features

Voice AI assistant ready to customize

Realtime pipeline with:

LLM

Speech-to-Text

Text-to-Speech

LiveKit Turn Detection

Noise cancellation

Logging & metrics

Dockerfile for deployment

You can connect this backend to a web/mobile frontend or telephony.

🛠️ Setup
1️⃣ Clone & Install
cd agent-starter-python
uv sync

2️⃣ Environment Variables

Copy .env.example → .env.local and update your credentials.

✅ Backend .env.local
LIVEKIT_URL=ws://localhost:7880
LIVEKIT_API_KEY=devkey
LIVEKIT_API_SECRET=secret

GOOGLE_API_KEY=api_key
MURF_API_KEY=api_key
DEEPGRAM_API_KEY=api_key

✅ Frontend .env.local
LIVEKIT_URL=ws://127.0.0.1:7880
LIVEKIT_API_KEY=devkey
LIVEKIT_API_SECRET=secret

NEXT_PUBLIC_LIVEKIT_URL=ws://127.0.0.1:7880
NEXT_PUBLIC_API_KEY=devkey
NEXT_PUBLIC_API_SECRET=secret

NEXT_PUBLIC_APP_CONFIG_ENDPOINT=
SANDBOX_ID=


These values are for local development.

📥 Required Downloads

Before the first run:

uv run python src/agent.py download-files

▶️ Running the Agent
Terminal mode (talk directly)
uv run python src/agent.py console

Dev mode (for frontend/telephony)
uv run python src/agent.py dev

Production mode
uv run python src/agent.py start

💻 Frontend Options

LiveKit provides ready-made starter apps:

Web (React/Next.js)

iOS/macOS (Swift)

Flutter

React Native

Android

Web Embed

Telephony integration

✅ Tests
uv run pytest

🚀 Deployment

This project includes a working Dockerfile and can be deployed:

To LiveKit Cloud

To your own server

Or with a self-hosted LiveKit setup

✅ If You Fork This Repo

Commit your uv.lock

Remove the template-only Git checks

Add LiveKit secrets to GitHub Actions if using CI

📄 License

MIT License.