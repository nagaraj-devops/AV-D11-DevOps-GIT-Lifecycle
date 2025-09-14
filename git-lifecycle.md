DevOps Git Lifecycle
1. Planning

Define requirements, tasks, and issues (via Jira, Trello, GitHub Issues, etc.)

Map features and bug fixes to branches.

2. Code (Development)

Clone repository → git clone

Create feature branch → git checkout -b feature/new-feature

Code changes are made in isolation.

3. Build

Commit changes locally → git add . + git commit -m "message"

Continuous Integration (CI) tools (Jenkins, GitHub Actions, GitLab CI, etc.) build and validate code.

4. Test

Automated tests run during CI pipeline:

Unit tests

Integration tests

Security scans

Ensures code stability before merging.

5. Release

Merge branch into main/develop via Pull Request (PR) or Merge Request (MR).

Peer code review ensures quality.

Git tagging (git tag v1.0.0) for versioning.

6. Deploy

CI/CD pipeline deploys to environments:

Dev → Staging → Production

Tools: Jenkins, GitHub Actions, GitLab, ArgoCD, Spinnaker, etc.

7. Operate

Application runs in production.

Monitoring tools: Prometheus, Grafana, ELK, CloudWatch.

Rollback strategies in case of failure.

8. Monitor & Feedback

Continuous monitoring of logs, metrics, and performance.

Feedback loop → Issues raised → Back to Planning phase.

🛠️ Common Git Commands in Lifecycle

Clone repo → git clone

Check status → git status

Switch branch → git checkout

Create branch → git checkout -b

Stage changes → git add

Commit changes → git commit

Push changes → git push

Pull updates → git pull

Merge branch → git merge

Resolve conflicts → Edit → git add → git commit

Tag release → git tag vX.X.X

✅ This lifecycle ensures collaboration, automation, and faster delivery of code with minimal errors.
