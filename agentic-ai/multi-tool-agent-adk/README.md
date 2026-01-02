# 🌦️ Weather & Time Agent (ADK)

This project demonstrates a **simple agentic AI system** built using **Google ADK**.
The agent can answer user questions about:

* 🌤️ **Weather**
* 🕒 **Current time**

for supported cities (currently **New York**).

The purpose of this project is to showcase:

* Tool-using agents
* Function calling
* Basic agent orchestration using ADK

---

## 🧠 How It Works

The agent is configured with:

* A language model (`gemini-2.5-flash-lite`)
* Two tools:

  * `get_weather(city)`
  * `get_current_time(city)`

Based on the user query, the agent decides **which tool to invoke** and returns a structured response.

---

## 📂 Project Structure

```
weather-time-agent/
│
├── agent.py              # Agent definition and tools
├── requirements.txt      # Python dependencies
└── README.md
```

---

## ⚙️ Setup Instructions

### 1️⃣ Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it:

**Linux / macOS**

```bash
source .venv/bin/activate
```

**Windows**

```bash
.venv\Scripts\activate
```

---

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

Create .env file in the multi_tool_agent folder add following details
```bash
GOOGLE_GENAI_USE_VERTEXAI=FALSE
GOOGLE_API_KEY=PASTE_YOUR_ACTUAL_API_KEY_HERE
```

---

### 3️⃣ Run the ADK Web Interface

From the **root folder** of the project:

```bash
adk web
```

This will start the local ADK web UI where you can interact with the agent.

---

## 🧪 Example Queries

Try asking the agent:

* *“What’s the weather in New York?”*
* *“What time is it in New York?”*
* *“Tell me the weather and time in New York”*

Unsupported cities will return a graceful error response.

---

## 🎯 Purpose of This Example

This is an intentionally **minimal agent** designed to:

* Demonstrate tool calling
* Show how agents decide actions
* Serve as a starter template for more advanced agentic systems
