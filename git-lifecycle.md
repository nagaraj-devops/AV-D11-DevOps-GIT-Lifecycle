# DevOps – Git Lifecycle

The Git lifecycle in a DevOps workflow defines how code changes flow from development to production with proper version control, collaboration, and automation.

---

## 1. Code
- Developers write code locally.
- Code is tracked with **Git**.
- Branching strategies are applied (e.g., `feature`, `develop`, `release`, `main`).

---

## 2. Commit
- Changes are staged (`git add`).
- Commits are created (`git commit`).
- Best practices:
  - Atomic commits (small, single-purpose).
  - Meaningful commit messages.

---

## 3. Push
- Code is pushed to a **remote repository** (GitHub, GitLab, Bitbucket).
- Collaboration happens via pull requests (PRs) / merge requests (MRs).

---

## 4. Build
- Triggered by **CI/CD pipeline** after push or merge.
- Steps include:
  - Code compilation
  - Dependency installation
  - Static code analysis

---

## 5. Test
- Automated testing integrated:
  - Unit tests
  - Integration tests
  - Security scans
  - Performance tests

---

## 6. Release
- Build artifacts are versioned and stored (e.g., Docker images, JAR/WAR, packages).
- Tagged in Git (`git tag`).
- Release branches created for stable versions.

---

## 7. Deploy
- Deployment to different environments:
  - **Dev** → internal testing
  - **QA/Staging** → pre-production validation
  - **Production** → live environment
- Automated with tools like Jenkins, GitHub Actions, GitLab CI, or ArgoCD.

---

## 8. Operate
- Application monitored in production:
  - Logging (ELK, Splunk)
  - Monitoring (Prometheus, Grafana, CloudWatch)
  - Alerting (PagerDuty, OpsGenie)

---

## 9. Feedback
- User and system feedback collected.
- Metrics used to improve future cycles.
- Continuous improvement of code and pipelines.

---

# Git Lifecycle in DevOps (Simplified Flow)
1. **Code** → 2. **Commit** → 3. **Push** → 4. **Build** → 5. **Test** →  
6. **Release** → 7. **Deploy** → 8. **Operate** → 9. **Feedback**

---

## Tools Commonly Used
- **Version Control**: Git, GitHub, GitLab, Bitbucket  
- **CI/CD**: Jenkins, GitHub Actions, GitLab CI/CD, CircleCI  
- **Build & Packaging**: Maven, Gradle, Docker  
- **Deployment**: Kubernetes, Helm, Terraform, Ansible  
- **Monitoring**: Prometheus, Grafana, ELK, CloudWatch  

---
<img width="748" height="446" alt="image" src="https://github.com/user-attachments/assets/40c7a771-7c4b-4acf-85e6-f29db076287a" />
