## GitHub 7-Day Beginner Roadmap

This repository now includes a practical plan you can follow to learn GitHub hands-on.

---

## Day 1 — Setup + Core Concepts

### Goals
- Create your GitHub account
- Install Git
- Set your Git identity
- Learn: repository, commit, branch

### Commands
```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global --list
```

### Complete when you can explain
- What a repository is
- What a commit is
- Why branches exist

---

## Day 2 — Local Git Practice

### Goals
- Create a local project
- Make file changes
- Stage and commit
- View commit history

### Commands
```bash
mkdir github-practice
cd github-practice
git init
echo "# GitHub Practice" > README.md
git add README.md
git commit -m "Initial commit"
echo "Learning Git daily." >> README.md
git add README.md
git commit -m "Update README with learning note"
git log --oneline --decorate --graph
```

---

## Day 3 — Push to GitHub

### Goals
- Create a repository on GitHub
- Connect local repo to remote
- Push your commits

### Commands
```bash
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
git remote -v
```

---

## Day 4 — Branch Workflow

### Goals
- Create and switch to a feature branch
- Make a change
- Commit and push branch

### Commands
```bash
git checkout -b feature/day-4-practice
echo "Branch practice line." >> README.md
git add README.md
git commit -m "Practice work on feature branch"
git push -u origin feature/day-4-practice
```

---

## Day 5 — Pull Request + Merge

### Goals
- Open your first pull request (PR)
- Write a clear PR description
- Merge after checks/review

### PR description template
```md
## Summary
- What changed

## Why
- Why this change is useful

## Testing
- How you verified it
```

### Complete when
- PR is opened from your feature branch to `main`
- PR is merged

---

## Day 6 — Collaboration Practice

### Goals
- Review someone else’s PR
- Leave comments
- Request changes
- Approve when ready

### Review checklist
- Is the change clear?
- Does it solve the stated problem?
- Any obvious bugs?
- Is there a better/simpler approach?

---

## Day 7 — Full Workflow Drill

### Goals
- Clone a repo
- Create a branch
- Commit + push
- Open PR
- Resolve a merge conflict
- Merge successfully

### Commands
```bash
git clone https://github.com/<owner>/<repo>.git
cd <repo>
git checkout -b feature/workflow-drill
# make changes
git add .
git commit -m "Workflow drill changes"
git push -u origin feature/workflow-drill
```

If a merge conflict happens:
```bash
git pull origin main
# resolve conflict markers in files
git add <resolved-files>
git commit -m "Resolve merge conflict"
git push
```

---

## Daily Habit (15–30 min)

Each day:
1. Make one real change
2. Commit it
3. Push it
4. Write what you learned

### Daily Log Template
```md
## Date: YYYY-MM-DD
- What I changed:
- Commit message:
- Command I practiced:
- What I learned:
- What confused me:
- Next step tomorrow:
```

---

## Success Criteria (End of Week)

You can do all of these without copy/paste:
- Initialize a repo
- Create and switch branches
- Commit with clear messages
- Push to GitHub
- Open and merge pull requests
- Pull latest changes
- Resolve simple merge conflicts
