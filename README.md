## Project Overview
Goal: Containerize a tiny Node.js web app, push image to Docker Hub, auto-deploy via GitHub Actions to an AWS EC2 free-tier VM, and expose logs & health metrics.

Success Criteria  
1. `git push` to `main` triggers CI → green build → image tagged and pushed.  
2. VM public IP responds `200 OK` at `/health` within 2 min of push.  
3. `docker logs <container>` shows requests; journalctl shows systemd service logs.  
4. README contains architecture diagram, runbook, screenshots of pipeline + VM + app.  
5. All PM artifacts (WBS, Gantt, Asana/Jira screenshots) linked in README.

Constraints: free-tier only, one developer, 1 week.