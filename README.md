# SarvamAI 
# **GoodFoods AI Reservation Agent 🍽️🤖**  
A conversational AI agent that handles **restaurant search, real-time slot availability, and table booking** across 100+ restaurants. Built using **Python, Streamlit, LLM orchestration, tool-calling, and JSON-based slot persistence**.

---

# 🎥 **Demo Video & Screenshots**

### 📺 **YouTube Demo:**  
https://youtu.be/i_e3DAKCrhE

### 📸 **Demo GIF:**  
![Demo GIF](Screen%20Recording%202025-11-27%20at%201.14.00%20AM.gif)


---

# 🚀 **Project Overview**

GoodFoods is a multi-location restaurant chain aiming to automate and modernize its reservation process.  
This project implements an **end-to-end AI-powered reservation system** with:

- 🧠 LLM-powered intent recognition (Grok / mock fallback)  
- 🛠️ Tool-calling architecture (search, availability, booking)  
- 🕒 Slot-based reservations with real-time slot removal  
- 📊 Data analytics (top cuisines, rating distribution)  
- 💬 Chat-style UI + Manual booking UI  
- 🌐 Streamlit frontend with Cloudflare/Ngrok tunnel  
- 📁 Fully persistent datastore (JSON)

This system is scalable and can be used by **restaurant chains, food apps, co-working spaces, salons, events, and more**.

---

# 📂 **Project Structure**

📦 GoodFoods-AI-Agent
├── generate_data.py # Generates restaurants.json
├── create_slots.py # Creates restaurant_slots.json
├── tools.py # Backend tool functions
├── orchestrator.py # LLM intent parsing → tool invocation
├── grok_llm.py # Optional Grok API integration
├── app.py # Streamlit frontend
├── restaurants.json # 100 restaurants dataset
├── restaurant_slots.json # Slots for each restaurant
├── bookings.json # Confirmed bookings
└── GoodFoods_Final.ipynb # Complete runnable notebook (Colab-ready)


---

# 🧠 **Tech Stack**

| Component         | Technology |
|------------------|------------|
| Frontend         | Streamlit |
| Backend Logic    | Python |
| LLM              | Grok API (optional) + Mock fallback |
| Tool Calling     | Custom orchestrator (no LangChain) |
| Data Storage     | JSON-based persistence |
| Deployment       | Cloudflare Tunnel / ngrok |
| Charts           | Pandas, Streamlit Charts |

---

# ✨ **Key Features**

### 🤖 Conversational AI Agent  
Understands natural language queries:
- “Find Italian restaurants near Koramangala”
- “Book restaurant 5 at 19:00 for 4 people”
- “Is 20:00 available at restaurant 8?”

### 🔧 Tool-Calling System  
LLM decides → Tool called:
- `search_restaurants`
- `get_availability`
- `book_slot`
- `cancel_booking`

### 🕒 Real-Time Slot-Based Booking  
- Books specific time slots  
- Removes booked slot from datastore  
- Prevents double-booking  

### 📊 Dashboard & Analytics  
- Chart: Top cuisines  
- Chart: Rating distribution  
- Sample restaurant dataset table  

### 💬 Persistent Chat History  
Streamlit session stores all past messages for a smooth UI experience.

---------------
