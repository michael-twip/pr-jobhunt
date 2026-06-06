# Jobhunt

Job search assistant for a Danish COO/VP Operations professional targeting Nordic/European tech scale-ups.

## Key files
- [profile.md](profile.md) — candidate profile (Danish), source of truth for matching criteria
- [found_jobs.md](found_jobs.md) — evaluated job leads with priority rankings and next actions

## Skills
- `/find-jobs` — search for new leads matching the profile
- `/evaluer-jobs` — evaluate and score a job against the profile, then append to `found_jobs.md`

## Conventions
- Language: Danish for all job-related content, English for code/config
- Evaluation format: match against profile.md criteria (role, company stage, geography, seniority)
- Keep `found_jobs.md` sorted by priority (🔴 hot → 🟡 warm → ⚪ low)
