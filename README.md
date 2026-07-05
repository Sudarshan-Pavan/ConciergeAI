# ConciergeAI 🏨

An intelligent multi-agent hotel assistant that automates the complete guest interaction workflow—from room discovery and booking to check-in guidance, room service requests, and checkout management.

Built as part of Google's **5-Day Agents Intensive Course**, ConciergeAI demonstrates how Large Language Models can orchestrate multiple function-calling tools to perform real-world business workflows autonomously.

---

## 🚀 Features

- 🔍 Search available hotel rooms
- 📅 Book rooms based on guest preferences
- 🛎️ Provide check-in instructions and hotel guidance
- 🍽️ Handle room service requests
- ✅ Manage guest checkouts
- 💾 Store and update booking records automatically
- 🤖 Autonomous decision-making using an LLM-powered agent

---

## 🏗️ System Architecture

The project follows an **Agent + Tools** architecture.

```
                  User
                    │
                    ▼
          ┌──────────────────┐
          │  Gemini AI Agent │
          └──────────────────┘
                    │
     ┌──────────────┼──────────────┐
     │              │              │
     ▼              ▼              ▼
 Room Search    Booking Tool   Room Service
     │              │              │
     └──────────────┼──────────────┘
                    ▼
            Checkout Tool
                    │
                    ▼
             Booking Database
             (Structured Files)
```

The LLM analyzes user requests, determines the appropriate action, invokes the required tool, and updates the booking records accordingly.

---

## 🧠 Technologies Used

- Python
- Google Gemini API
- Function Calling
- Agentic AI
- Prompt Engineering
- Jupyter Notebook

---

## ⚙️ How It Works

1. User submits a hotel-related request.
2. Gemini interprets the intent.
3. The agent selects the appropriate function/tool.
4. Tool executes the requested operation.
5. Booking information is updated.
6. Response is returned to the user.

---

## 📂 Project Structure

```
ConciergeAI/
│
├── ConciergeAI.ipynb
├── bookings.json
├── README.md
└── assets/
```

*(Folder structure may vary depending on your implementation.)*

---

## 💡 Design Philosophy

Instead of hardcoding every workflow, ConciergeAI follows an **Agentic AI** approach where the language model dynamically decides which tool to invoke based on the user's request.

This architecture makes the system modular, extensible, and adaptable for future hotel operations.

---

## 🔮 Future Improvements

- Web interface using FastAPI + React
- Multi-agent architecture
- Authentication and guest profiles
- Database integration (PostgreSQL/MySQL)
- Email confirmations
- Payment gateway integration
- Live room availability
- Voice-enabled interaction

---

## 📌 Note

This project was developed as a proof of concept during Google's **5-Day Agents Intensive Course**. The focus was on demonstrating Agentic AI workflows, tool orchestration, and autonomous task execution rather than building a production-ready hotel management platform.

---

## 👨‍💻 Author

**Pulipaka Sudarshan Pavan Kumar**

GitHub: *your profile*

LinkedIn: *your profile*
