# 📋 UXMap App – Version Log & Update Notes

Chronological changelog of project decisions and feature changes.

---
## 2025-06-28 – Day 4

- Refactored frontend UI to use side navigation for analysis results; removed raw element list from user view
- Added loading spinner to improve user feedback during analysis requests
- Backend now returns structured JSON including `ux_score`, summary, and reason
- Updated backend prompt to instruct AI to return a score and reason in JSON format
- Implemented JSON parsing logic in backend; fixed indentation and error handling
- Frontend now displays UX score, summary, and reason in the Results tab
- Cleaned up `.gitignore` and removed tracked build/artifact folders from GitHub
- Debugged navigation, API, and deployment issues; confirmed end-to-end flow is working
- Pushed all updated code to GitHub for both frontend and backend


## 2025-06-25 – Day 3 Backend Security & API Refactor
- Moved OpenAI API key and all OpenAI requests from Flutter frontend to backend (`server.py`) for improved security
- Added `/analyze` endpoint to Flask backend to perform crawling, clickable element extraction, and AI UX analysis
- Updated requirements.txt to include all necessary dependencies for cloud deployment (e.g., `bs4`)
- Fixed Render deploy failures caused by missing modules
- Verified that frontend now communicates only with the backend; no API keys or HTML parsing in Dart code
- Backend API returns both clickable elements and UX analysis as JSON for use in the Flutter app


## 2025-06-20 – Day 2
- Started project documentation
- Agreed to structure `/docs/` folder with `ideas.md` and `updates.md`
- Reconfirmed Option 1: GitHub-based ideation + versioning
- Next step: Initialize Flutter project and basic UI

---

## 2025-06-19 – Day 1
- Project concept discussed
- Agreed to build in Flutter (multi-platform)
- Goal: Website UX analyzer + journey mapper
- Consideration: Token limit for GPT analysis
- API cost/ROI explored
- User experience tied to clickable elements
- Vision of crawl + summarize per layer (3 steps)

---
