
# AI-Powered Educational Platform

A **modular, AI-integrated E-Learning platform** built with **Django**, designed to showcase real-world skills in educational technology, NLP, LLMs, and full-stack development.

> ✨ Built as a portfolio project for Python Developer roles in AI/Education tech, including Danson Solutions Pvt. Ltd.

---

##  Live Demo

[//]: # ( [Coming Soon – Deployed on Render/Heroku])

---

## Features

| Module | Description |
|--------|-------------|
|  **AI Quiz Generator** | Enter a topic → generate MCQs using OpenAI → export/share |
|  **Course-Aware AI Chatbot** | Upload course PDFs → chat with context-aware AI (LangChain + FAISS) |
|  **AI Writing Assistant** | Essay feedback using spaCy + GPT (grammar, coherence, suggestions) |
|  **Gamified Learning** | Mini-games with XP, badges, and leaderboards |
|  **Content Summarizer** | Paste URL → scrape + summarize with GPT | ELI5 mode |
|  **Learning Analytics** | Track student progress with REST APIs + Pandas reports |
|  **Authentication System** | Students, Teachers, and Admin roles with JWT/Django Auth |

---

##  Tech Stack

**Backend**:
- Django · Django REST Framework
- PostgreSQL · SQLite · FAISS (Vector DB)
- Celery (optional) · Redis (optional)

**AI/NLP**:
- OpenAI GPT (via API)
- LangChain · spaCy · Hugging Face Transformers

**Frontend**:
- Django Templates + Tailwind CSS
- Optional: React (planned)

**Other**:
- BeautifulSoup (web scraping)
- dotenv · Gunicorn · WhiteNoise

---

##  Project Structure

\`\`\`
edu_platform/
├── settings/         # base.py, dev.py, prod.py
├── ai_quiz_generator/
├── ai_chatbot/
├── writing_assistant/
├── learning_games/
├── content_summarizer/
├── learning_analytics/
├── users/
├── templates/        # Tailwind-based pages
├── static/
├── media/
└── manage.py
\`\`\`

---

##  Screenshots

> Will be added after UI implementation. Includes:
- Quiz generation flow
- AI chat with PDF
- Essay feedback results
- Analytics dashboard
- Game leaderboard

---

##  Setup Instructions

### 1. Clone the Repository
\`\`\`bash
git clone https://github.com/saveenstha/edu_platform.git
cd edu-platform
\`\`\`

### 2. Create Virtual Environment
\`\`\`bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
\`\`\`

### 3. Install Requirements
\`\`\`bash
pip install -r requirements.txt
\`\`\`

### 4. Configure Environment Variables
Create a \`.env\` file in the root:
\`\`\`env
DJANGO_SECRET_KEY=your-secret-key
OPENAI_API_KEY=your-openai-key
POSTGRES_DB=dbname
POSTGRES_USER=dbuser
POSTGRES_PASSWORD=dbpassword
POSTGRES_HOST=localhost
POSTGRES_PORT=5432
\`\`\`

### 5. Run Development Server
\`\`\`bash
python manage.py migrate
python manage.py runserver --settings=edu_platform.settings.dev
\`\`\`

---

## Switch Settings Module

- For dev:  
  \`DJANGO_SETTINGS_MODULE=edu_platform.settings.dev\`

- For prod:  
  \`DJANGO_SETTINGS_MODULE=edu_platform.settings.prod\`

---

## Testing (Basic Example)
\`\`\`bash
python manage.py test
\`\`\`

---

## Completed & Planned Modules

| Module             | Status         |
|--------------------|----------------|
| AI Quiz Generator  | In Progress    |
| AI Chatbot (PDF QA)| In Progress    |
| Writing Assistant  | In Progress    |
| Learning Games     | ️ In Progress  |
| Summarizer Tool    | In Progress    |
| Analytics API      | In Progress    |
| User Roles/Auth    | In Progress    |
| Tailwind UI        | ️ In Progress  |

---

[//]: # ()
[//]: # (##  Deployment)

[//]: # (Deployed on:)

[//]: # (- 🔵 Render &#40;backend&#41;)

[//]: # (- 🟣 Railway &#40;alt DB/test&#41;)

[//]: # (- 🔶 Vercel &#40;frontend if React used&#41;)

---

## 🙋‍♂️ Author

**Saveen Shrestha**  
📍 Kathmandu, Nepal  
🎯 Aspiring Python Developer  
🔗 [LinkedIn](#) | [Portfolio](#) | [GitHub](https://github.com/yourusername)

---

## License

MIT License
