PR Agent (skeleton)
====================

This folder contains a minimal webhook receiver and worker skeleton for the PR automation agent.

Files:
- `pr_agent/webhook.py`: FastAPI receiver for GitHub webhooks
- `pr_agent/worker.py`: simple worker loop placeholder
- `pr_agent/policy.py`: minimal policy checks
- `pr_agent/Dockerfile`: container for webhook service

Install & run (local dev):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install fastapi uvicorn
uvicorn pr_agent.webhook:app --reload
```
