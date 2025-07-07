# Sunset's Claim

Sunset's Claim is a narrative-driven 3D adventure game set in the American West during the mid-1800s. Players assume the role of a lone traveler navigating a haunted frontier town, unraveling the mystery of a vanished community while making choices that impact the unfolding story.

---

## 🎮 Game Overview

- **Genre**: Narrative Adventure / Mystery  
- **Setting**: 1847, American West  
- **Style**: Third-person exploration with branching dialogue and character-driven storytelling  
- **Themes**: Isolation, folklore, survival, moral ambiguity

---

## 🧰 Tech Stack

- **Engine**: Unreal Engine 5 (C++)  
- **3D Modeling**: Blender  
- **Source Control**: Git + GitHub  
- **CI/CD**: GitHub Actions (basic validation configured)  
- **IDE**: Visual Studio Code

---

## 🧪 GitHub Actions CI

**Workflow location**: `.github/workflows/ci.yml`

Runs on push or PR to `dev` or `release` branches:
- ✅ Checks out the code
- ✅ Displays basic project structure (`tree -L 2`)
- 🚧 Placeholder for future: build steps, commit message linting, Unreal validation, etc.

---

## 🌳 Branching Strategy

- `release` — stable, production-ready branch (**default**)  
- `dev` — active development branch  
- `feature/...`, `bugfix/...`, `chore/...` — temporary branches merged into `dev`  

### Example branch names

feature-npc-dialogue
bugfix-save-load-crash
chore-update-readme

---

## 📝 Commit Message Convention

All commit messages must follow this format:
`[tasktype]: brief summary under 120 characters`

Valid `tasktype` values:
`feature`, `bugfix`, `chore`, `hotfix`, `refactor`, `docs`, `test`

Examples:
`[feature]: add NPC dialogue system`
`[bugfix]: fix ambient audio cutoff in night scenes`
`[chore]: update .gitignore for generated assets`

---

## 🔖 Versioning & Tags

Semantic versioning is used:

- Example tags: `v0.1.0`, `v0.2.0`, `v1.0.0`  
- Tags applied to the `release` branch to mark playable milestones

---

## 📦 Changelog

Changelogs will be generated using GitHub metadata and commit messages.  
First milestone release (`v0.1.0`) will include manually written highlights.

---

## 🛠️ Roadmap

- [ ] Setup C++ linting and header validation  
- [ ] Automate changelog generation  
- [ ] Add Unreal Engine build steps in CI  
- [ ] Document onboarding for collaborators

---
