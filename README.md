# ViewsGrow
# ViewsGrow (Full stack) — Demo-ready

## Prereqs
- Node.js >=16, npm
- (Optional) OpenAI API key

## Setup backend
cd backend
npm install
cp .env.example .env
# optionally add OPENAI_API_KEY in .env (if you have)
# You can also set FORCE_DEMO=true to force demo mode
npm run dev

Backend will run on http://localhost:5000

## Setup frontend
cd frontend
npm install
# Optionally set VITE_API_BASE in .env to point to backend
# e.g., VITE_API_BASE=http://localhost:5000/api
npm run dev

Open frontend at http://localhost:5173

## Notes
- If no OPENAI_API_KEY set, backend returns demo-generated results.
- To enable real AI, set OPENAI_API_KEY in backend/.env and restart backend.
- For production, deploy backend on Render/Heroku/Vercel server, and frontend on Vercel/Netlify.
