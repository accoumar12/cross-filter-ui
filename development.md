# Development

## Getting Started

### 🐳 Docker

```bash
docker compose -f docker-compose.yml -f docker-compose.dev.yml watch
```

Connect to the Web UI at http://127.0.0.1:3000/. The API server runs on port 8000.

### 💪 Non-Docker

#### Backend

```bash
cd backend
uv sync
uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

#### Frontend

```bash
cd frontend
npm install
npm run dev
```

Connect to the Web UI at http://127.0.0.1:3000/.
