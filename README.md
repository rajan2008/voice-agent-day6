# Day 6 - Fraud Alert Voice Agent

**AI Voice Agents Challenge by [murf.ai](https://murf.ai)**

A professional fraud detection voice agent for SecureBank that verifies suspicious transactions through voice calls.

## Quick Start

**Terminal 1:** `cd livekit && livekit-server.exe --dev`  
**Terminal 2:** `cd backend && uv run python src/agent.py dev`  
**Terminal 3:** `cd frontend && pnpm dev`  
**Terminal 4:** `cd backend && python web_db.py`

## Test

1. Open **http://localhost:3000** (Frontend)
2. Open **http://localhost:5000** (Database Viewer)
3. Click "Connect" 
4. Say card number: **4242**, **8765**, or **1234**
5. Answer security question
6. Confirm/deny transaction
7. Watch live updates at http://localhost:5000

## Test Cases

- **Card 4242** → John Smith (Answer: "Johnson")
- **Card 8765** → Sarah Wilson (Answer: "Chicago") 
- **Card 1234** → Mike Johnson (Answer: "Buddy")

## Database

SQLite database (`fraud_cases.db`) updates in real-time. Watch backend terminal for live changes.

---

**Day 6 Complete!** Built with LiveKit Agents + Murf Falcon TTS
