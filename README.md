# Fraud Lens

Fraud Lens is a project workspace for fraud detection experiments and application code. The repository is organized into separate areas for the frontend and model services.

## Project Structure

```text
fraud-lens/
├── frontend/   # Frontend application workspace
├── ml-model/   # Machine learning model service or scripts
├── xg-model/   # XGBoost model service or scripts
└── README.md
```

## Current Status

This repository currently contains the project folders and generated files, but no visible application source files, dependency manifests, or run scripts are present yet.

Expected files to add as the project grows:

- `frontend/package.json` for frontend dependencies and scripts
- `ml-model/requirements.txt` or `pyproject.toml` for Python dependencies
- `xg-model/requirements.txt` or `pyproject.toml` for XGBoost model dependencies
- API entry points such as `app.py`, `main.py`, or equivalent service files
- Example environment variables in `.env.example`

## Getting Started

Clone the repository:

```bash
git clone <repository-url>
cd fraud-lens
```

Install and run each part of the project after its dependencies and scripts are added.

### Frontend

```bash
cd frontend
npm install
npm run dev
```

### Python Model Services

```bash
cd ml-model
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

For the XGBoost model workspace:

```bash
cd xg-model
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

## Development Notes

- Keep generated files such as `__pycache__`, build output, logs, and local environment files out of version control.
- Add `.env.example` for required configuration values without committing secrets.
- Document model inputs, expected outputs, and API endpoints as soon as the services are implemented.
- Add tests for model inference, input validation, and frontend workflows before production use.

## Suggested Next Steps

1. Add source code and dependency manifests for each workspace.
2. Add sample input data or request payloads for fraud prediction.
3. Document API endpoints and model response formats.
4. Add setup, test, and deployment commands once finalized.
