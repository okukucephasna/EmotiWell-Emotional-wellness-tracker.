A simple mental wellness companion web app built with **React**, **Flask**, and **PostgreSQL**.  
MindTrack helps users **track their moods**, **log journal entries**, and receive **personalized coping strategies** to improve emotional well-being.

---

## Features
- 🌱 **Mood Logging:** Record daily moods with stress and energy levels.
- 📝 **Journal Entries:** Add personal notes to reflect on your day.
- 🎯 **Personalized Suggestions:** Get self-care tips based on your current mood.
- 📊 **Mood Trends Dashboard:** Visualize mood patterns over time.
- 🔐 **User Authentication:** Secure sign-up and login for personal data privacy.

---

## Tech Stack
| Technology    | Usage |
|---------------|-------|
| **React**     | Frontend UI with Tailwind CSS |
| **Flask**     | Backend REST API |
| **PostgreSQL**| Relational database for moods and users |
| **SQLAlchemy**| ORM for Flask-Postgres interaction |
| **JWT**       | Secure authentication |

---

## Project Structure
```

mindtrack/
│
├── backend/          # Flask backend
│   ├── app.py        # Main Flask app
│   ├── models.py     # Database models
│   ├── routes/       # API route files
│   ├── requirements.txt
│
├── frontend/         # React frontend
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── App.js
│   ├── package.json
│
└── README.md

````

---

## Installation

### 1. Clone the repository
```bash
git clone https://github.com/your-username/mindtrack.git
cd mindtrack
````

---

### 2. Backend Setup (Flask)

```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
pip install -r requirements.txt
```

Create a `.env` file in the `backend` folder:

```
DATABASE_URL=postgresql://username:password@localhost:5432/mindtrack_db
SECRET_KEY=your_secret_key
```

Run database migrations:

```bash
flask db upgrade
```

Start the backend server:

```bash
flask run
```

---

### 3. Frontend Setup (React)

```bash
cd frontend
npm install
npm start
```

---

## API Endpoints

| Method | Endpoint            | Description                    |
| ------ | ------------------- | ------------------------------ |
| POST   | `/api/register`     | Register a new user            |
| POST   | `/api/login`        | User login                     |
| POST   | `/api/mood`         | Log a mood entry               |
| GET    | `/api/mood/history` | Retrieve mood history          |
| GET    | `/api/strategy`     | Get coping strategy for a mood |

---

## Example Use Case

1. User signs up and logs in.
2. Logs mood: **"Stressed 😰"** with a note: *"Had a tough meeting."*
3. Backend saves mood and returns a relevant strategy:

   > "Try deep breathing: inhale for 4 seconds, hold for 7, exhale for 8."
4. User sees this tip on the dashboard.
5. Over time, user views a mood chart and sees stress levels peak on weekdays.

---

## Roadmap

* [ ] Add sentiment analysis for journal entries
* [ ] Integrate external API for guided meditation videos
* [ ] Dark mode for better accessibility
* [ ] Mobile-friendly version

---

## License

This project is licensed under the MIT License.

Would you like me to generate a **backend folder structure with Flask boilerplate code** next?
```
