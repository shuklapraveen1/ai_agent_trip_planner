# 🌍 RoamAI – AI-Powered Travel Planner

RoamAI is an AI-powered travel planning application that creates personalized travel itineraries based on your destination, travel dates, budget, hotel preferences, and interests. It leverages Google's Gemini AI to generate detailed, day-wise travel plans through a modern and intuitive web interface.

## ✨ Features

- 🤖 AI-generated personalized travel itineraries
- 📍 Destination and departure city selection
- 📅 Interactive travel date picker
- 👥 Traveler configuration
- 💰 Budget planning
- 🏨 Hotel preference selection
- 🎯 Interest-based itinerary customization
- 🌤️ Weather information widget
- 💱 Currency conversion widget
- 🧳 Smart packing checklist
- ⏳ Trip countdown
- 🌙 Light & Dark mode support
- 📄 Beautiful markdown itinerary rendering
- 📱 Fully responsive UI

---

## 🛠️ Tech Stack

### Frontend

- React 19
- TypeScript
- TanStack Start
- Tailwind CSS v4
- Framer Motion
- React Hook Form
- React Markdown
- Radix UI
- Lucide React
- Sonner

### Backend

- FastAPI
- Python
- Google Gemini API
- Pydantic
- Uvicorn

---

## 📂 Project Structure

```
ai_agent_trip_planeer/
│
├── backend/
│   ├── main.py
│   ├── agent.py
│   ├── requirements.txt
│   └── ...
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── routes/
│   │   ├── services/
│   │   └── ...
│   ├── package.json
│   ├── vite.config.ts
│   └── ...
│
├── .gitignore
└── README.md
```

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/shuklapraveen1/ai_agent_trip_planeer.git

cd ai_agent_trip_planeer
```

---

# Backend Setup

## Create a Virtual Environment

```bash
python -m venv venv
```

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r backend/requirements.txt
```

---

## Configure Environment Variables

Create a `.env` file inside the **backend** directory.

```env
GOOGLE_API_KEY=YOUR_GEMINI_API_KEY
```

---

## Start the Backend

```bash
cd backend

python main.py
```

or

```bash
uvicorn main:app --reload
```

The backend will run at:

```
http://127.0.0.1:8000
```

Swagger API documentation:

```
http://127.0.0.1:8000/docs
```

---

# Frontend Setup

Open a new terminal.

```bash
cd frontend

npm install

npm run dev
```

The frontend will run at:

```
http://localhost:8080
```

---

# API Endpoint

### Generate Travel Plan

**POST**

```
/api/plan
```

### Sample Request

```json
{
  "destination": "Paris",
  "departure": "Delhi",
  "travel_dates": "12 Aug - 18 Aug",
  "travelers": "2 Adults",
  "budget": "150000",
  "hotel": "Luxury",
  "interests": "Museums, Food, Shopping"
}
```

### Sample Response

```json
{
  "success": true,
  "itinerary": "# Day 1\n..."
}
```

---

# 🏗️ Architecture

```
              User
                │
                ▼
      React + TypeScript UI
                │
         REST API Request
                │
                ▼
        FastAPI Backend
                │
                ▼
      Google Gemini API
                │
                ▼
      AI Travel Itinerary
                │
                ▼
      Markdown Response
```

---

# 📸 Screenshots

Add your project screenshots inside a `screenshots/` folder.

```
screenshots/
├── home.png
├── planner.png
├── itinerary.png
└── dark-mode.png
```

Example:

```markdown
## Home Page

![Home](screenshots/home.png)

## AI Generated Itinerary

![Itinerary](screenshots/itinerary.png)
```

---

# 🌟 Future Enhancements

- Flight search integration
- Hotel booking APIs
- Google Maps integration
- PDF itinerary export
- User authentication
- Trip history
- AI budget optimization
- Multi-language support
- Calendar integration

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Praveen Shukla**

- GitHub: https://github.com/shuklapraveen1
- Repository: https://github.com/shuklapraveen1/ai_agent_trip_planeer

---

If you found this project helpful, consider giving it a ⭐ on GitHub!
