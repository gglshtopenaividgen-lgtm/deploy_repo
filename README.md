# FLH-ONE Autonomous Web Deployment Target (`deploy_repo`)

> **Automated Vercel Deployment Repository for J.A.R.V.I.S & F.R.I.D.A.Y**  
> **Live URL**: [`https://flhagent1.vercel.app`](https://flhagent1.vercel.app)

---

## ⚡ How It Works
1. When you ask J.A.R.V.I.S in the assistant studio: *"Build me a website/web application"*, the agent designs the complete HTML/JS/CSS codebase.
2. The agent's `web_deployer.py` commits and pushes the new files directly to this repository's `main` branch via GitHub API.
3. Vercel automatically detects the commit, runs the build pipeline, and deploys the update to [**flhagent1.vercel.app**](https://flhagent1.vercel.app) within ~15 seconds.
