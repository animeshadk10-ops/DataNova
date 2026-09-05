# DataNova AI

AI-powered data diagnostics, cleaning, and machine learning platform.

## Features

- **AI Data Analysis** — Upload any CSV/Excel/JSON dataset and get instant AI-powered diagnostics
- **Smart Recommendations** — Gemini AI suggests cleaning actions with confidence scores
- **Quiz Mode** — Guess the right fix before the AI reveals it, earn points and streaks
- **Developer Canvas** — Visual node-based pipeline editor with 20+ transform tools
- **ML Model Training** — Train and compare multiple ML models directly on your data
- **Natural Language Chat** — Ask questions about your dataset in plain English
- **What-If Simulator** — Preview the impact of cleaning actions before applying them
- **Data Storytelling** — AI-generated narratives about your data's health
- **Export as Code** — Download cleaning pipelines as Python, Jupyter, or SQL
- **Recovery Dashboard** — Before/after visualization of data quality improvements

## Tech Stack

**Backend:** Python, FastAPI, Pandas, scikit-learn, Gemini API  
**Frontend:** Next.js 16, React, TypeScript, Tailwind CSS, React Flow, Recharts

## Quick Start

```bash
# Backend
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000

# Frontend
cd frontend
npm install
npm run dev
```

Visit `http://localhost:3000`

## Docker

```bash
docker-compose up --build
```

## Architecture

```
├── backend/
│   ├── app/
│   │   ├── routers/     # API endpoints
│   │   ├── services/    # Business logic
│   │   ├── models/      # Pydantic schemas & enums
│   │   └── prompts/     # Gemini prompt templates
│   └── tests/           # 64+ test cases
├── frontend/
│   ├── src/
│   │   ├── app/         # Next.js pages
│   │   ├── components/  # 30+ React components
│   │   └── lib/         # API client & utilities
│   └── ...
└── docker-compose.yml
```

## Canvas Tools

### Data
- File/Session, Data Preview, Dataset Statistics

### Transforms
- Impute (median/mode), Drop Column, Clip Outliers, Merge Categories
- Log Transform, Filter Rows, Sort, Rename Column, Type Cast
- Encode Categories (label/one-hot), Scale/Normalize, Sample Rows

### Visualize
- Scatter Plot, Box Plot, Correlation Heatmap

### Machine Learning
- ML Model Trainer (Logistic Regression, Random Forest, Gradient Boosting, SVM, KNN, Decision Tree, Ridge, Lasso)
- Model Comparison (bar charts, confusion matrices, feature importance)

## License

MIT
