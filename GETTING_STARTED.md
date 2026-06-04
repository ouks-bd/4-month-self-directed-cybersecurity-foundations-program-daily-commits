# Getting Started

This is your scaffolding. Here's how to make it your own on Day 1.

## 1. Personalize

Open these files and replace placeholders:

- `README.md` — replace `_add your start date_` with today; add your name where mentioned
- `LICENSE` — replace `[Your Name]` with your actual name
- `00-roadmap/progress-tracker.md` — confirm dates as you complete items
- `daily-log/YYYY-Www.md` — start logging today

## 2. Initialize git and push to GitHub

```bash
# From this folder
git init
git add .
git commit -m "Initial scaffold for cybersecurity journey"

# Create the repo on GitHub (UI or `gh repo create`), then:
git remote add origin git@github.com:YOUR-USERNAME/cybersecurity-journey.git
git branch -M main
git push -u origin main
```

## 3. Pin the repo on your GitHub profile

Settings → Pinned → add this repo. It's the first thing recruiters see.

## 4. Establish the daily commit habit

Every study session:
1. Open the relevant week's `notes/` file
2. Write what you learned in your own words
3. Update `daily-log/YYYY-Www.md`
4. Update `00-roadmap/progress-tracker.md`
5. Commit with a meaningful message:

```bash
git add .
git commit -m "Week 1 Day 3: malware deep dive + WannaCry analysis"
git push
```

## 5. Scenario files are your superpower

For every breach you study, fill in the corresponding `scenarios/*.md` file. The template forces you to map:
- Actor → Vector → Vulnerability → Action → Impact

This is exactly the framework you'll use in interviews. Practicing the structure is more valuable than the specific breach details.

## 6. What NOT to commit

`.gitignore` already blocks most of it, but stay vigilant:
- Real passwords, API keys, AWS credentials
- VPN config files (`.ovpn`)
- TryHackMe / HackTheBox flags
- Anything from active CTFs or private engagements
- Internal documents from work / school

If you commit something sensitive by accident, **don't just delete and re-push**. The data is in git history. Use [BFG Repo-Cleaner](https://rtyley.github.io/bfg-repo-cleaner/) or `git filter-repo`, force-push, and rotate the leaked secret immediately.

## 7. Optional but nice

- Add a GitHub Actions workflow to run a markdown linter
- Add a `CHANGELOG.md` for major milestones (cert earned, etc.)
- Set up GitHub Pages to publish notes as a website later

## You're set

Start with `01-threats-and-principles/README.md` and work through Mon's lesson. Commit when you finish. Don't break the chain.
