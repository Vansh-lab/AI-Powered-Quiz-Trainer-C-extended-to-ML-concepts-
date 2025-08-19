# AI-Powered-Quiz-Trainer-C-extended-to-ML-concepts-
An adaptive quiz platform with an anime AI tutor, focused on programming languages (C, C++, Java, Python, JS, Go, Rust) and DSA. Features include weekly national contests (Sunday 7 PM IST), adaptive learning (IRT + spaced repetition + bandits), detailed explanations, and a national/state/college leaderboard
# AI‑Powered Quiz Trainer

An **adaptive quiz platform** with an anime AI tutor, focused on programming languages (C, C++, Java, Python, JS, Go, Rust) and DSA. Features include weekly national contests (Sunday 7 PM IST), adaptive learning (IRT + spaced repetition + bandits), detailed explanations, and a national/state/college leaderboard.

---

##  Features

* Anime **AI Tutor** (Live2D/Lottie) that explains answers and motivates learners.
* Quizzes for **C, C++, Java, Python, JavaScript, Go, Rust, and DSA topics**.
* **Adaptive learning engine**: error tracking, spaced repetition (SM‑2), IRT difficulty adjustment.
* **Weekly Sunday Contest (7:00 PM IST)** with national/state/college leaderboards.
* **Leaderboards**: ELO‑style ratings (national, statewise, collegewise).
* **PWA support**: installable app, offline practice for recent sets.
* **Admin console**: CRUD for questions, contest scheduling, import/export.
* **Secure sandbox** for code output questions.
* Accessibility: screen‑reader support, dyslexia‑friendly fonts, keyboard navigation.

---

##  Tech Stack

* **Frontend**: Next.js 14, TailwindCSS, shadcn/ui, Framer Motion.
* **Backend**: FastAPI or NestJS, PostgreSQL, Redis, Docker.
* **Auth**: Google/GitHub OAuth, JWT.
* **Infra**: Vercel/Fly.io/Render, Cloudflare CDN, S3 object storage.

---

##  Getting Started

### Prerequisites

* Node.js 20+
* Python 3.11+ (if FastAPI backend)
* PostgreSQL 15+
* Redis 7+
* Docker (optional for sandbox & deployment)

### Setup

```bash
# Clone repo
git clone https://github.com/your-org/ai-quiz-trainer.git
cd ai-quiz-trainer

# Install frontend
yarn install

# Install backend (FastAPI)
cd backend
pip install -r requirements.txt

# Setup DB
createdb quiz_trainer
prisma migrate deploy

# Run dev servers
# frontend
yarn dev
# backend
uvicorn app.main:app --reload
```

### Environment Variables

Create a `.env` file in both root and backend:

```
DATABASE_URL=postgresql://user:pass@localhost:5432/quiz_trainer
REDIS_URL=redis://localhost:6379
NEXTAUTH_SECRET=your_secret
NEXTAUTH_URL=http://localhost:3000
GOOGLE_CLIENT_ID=xxx
GOOGLE_CLIENT_SECRET=xxx
GITHUB_ID=xxx
GITHUB_SECRET=xxx
```

---

##  Roadmap

* [ ] Add code runner for all languages.
* [ ] Mobile app (React Native shell).
* [ ] Discord/Telegram integration.
* [ ] Private college contests.

---

##  Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss.

---


