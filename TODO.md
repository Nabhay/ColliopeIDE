# Project Roadmap & TODOs

Welcome to the Calliope IDE roadmap! This document lists the features and improvements we plan to implement. Community contributions are highly encouraged for any of these items.

## 🟢 Good First Issues (Beginner Friendly)

- [ ] **Implement `main.py` entry point**
  - Currently `main.py` is empty. We need a CLI wrapper that can start both the frontend and backend servers, or at least guide the user to do so.
- [ ] **Add proper `requirements.txt`**
  - Create a standard requirements file for the Python backend dependencies (`flask`, `google-generativeai`, etc.).
- [ ] **Fix Linter Errors**
  - Run `npm run lint` and resolve any outstanding style or type issues in the frontend code.

## 🟡 Backend Improvements

- [ ] **Database Integration**
  - Implement a persistent database (PostgreSQL/SQLite) to save user sessions, chat history, and project metadata.
- [ ] **Authentication System**
  - Add user accounts and secure authentication (OAuth/Email) to replace the current local storage based identity.
- [ ] **Enhanced Security**
  - Implement stricter input validation in `server/agent.py`.
  - Add sandboxing for the code execution environment to prevent system vulnerability usage.

## 🟠 Frontend Enhancements

- [ ] **Mobile Responsiveness**
  - Improve the layout on smaller screens, specifically the IDE workspace.
- [ ] **Theme Customization**
  - Allow users to create and save custom syntax highlighting themes.
- [ ] **Accessibility**
  - Audit and improve ARIA labels and keyboard navigation support across all components.

## 🔴 DevOps & Infrastructure

- [ ] **Docker Support**
  - Create a `Dockerfile` and `docker-compose.yml` to spin up the entire stack with one command.
- [ ] **CI/CD Pipeline**
  - Set up GitHub Actions for automated testing and linting on Pull Requests.
- [ ] **Monitoring & Analytics**
  - Integrate telemetry to track usage patterns and errors (e.g., Sentry, PostHog).
