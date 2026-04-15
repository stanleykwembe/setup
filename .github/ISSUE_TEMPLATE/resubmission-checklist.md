---
name: Resubmission Checklist
about: Checklist for fixing project issues before resubmission
title: "[RESUBMISSION] Fix required issues"
labels: enhancement
assignees: ''
---

# 🧾 Resubmission Checklist

## 🐛 API Issues
- [ ] Model is NOT loaded inside the endpoint (load once at startup)
- [ ] API returns JSON response (not raw string)

---

## ✨ Frontend Requirement
- [ ] Add single HTML page for testing API
  - Project title included
  - Input form for findings text
  - Submit button calling API
  - Output display section

---

## ⚡ Performance & Deployment
- [ ] Model loading optimized for production (no per-request loading)
- [ ] FastAPI app optimized for Render deployment
- [ ] No unnecessary cold start delays

---

## 📄 README Improvements
- [ ] Add deployment explanation (Render setup)
- [ ] Add limitations section (performance + CPU inference)
- [ ] Add system architecture overview
- [ ] Explain training vs inference separation clearly

---

## 📦 Dependencies
- [ ] Remove unnecessary CUDA packages from requirements.txt
- [ ] Separate training and inference requirements files

---

## 🧠 Code Quality
- [ ] Proper model evaluation mode used (model.eval())
- [ ] Clean separation between training and API code
- [ ] Add error handling for inference requests

---

## 📊 Optional Improvements
- [ ] Add simple architecture diagram
- [ ] Improve API documentation/examples in README
