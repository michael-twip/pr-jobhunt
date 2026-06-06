name: evaluer-jobs
description: Evaluate jobs found by the find-jobs skill and provide feedback on their relevance and quality.
---

## Task Overview
The `evaluer-jobs` skill is designed to help users evaluate job opportunities found by the `find-jobs` skill. It takes in a list of job listings and provides feedback on their relevance and quality based on the user's profile and preferences.
The skill assesses various factors such as job title, company reputation, location, salary, and required skills to determine how well each job matches the user's criteria. The output includes a rating or score for each job listing, along with specific feedback on why it may or may not be a good fit for the user.
The found jobs are located in the found_jobs.md file, which is a working document board for the `find-jobs` skill. The `evaluer-jobs` skill will read from this file to access the job listings that need to be evaluated. Each job listing in the found_jobs.md file should include relevant details such as job title, company name, location, salary, and required skills to facilitate a thorough evaluation by the `evaluer-jobs` skill as well as location it was found.
The found_jobs.md file serves as a central repository for the job listings found by the `find-jobs` skill, allowing the `evaluer-jobs` skill to access and evaluate them effectively. The feedback provided by the `evaluer-jobs` skill can help users make informed decisions about which job opportunities to pursue based on their relevance and quality. Each job listing in the found_jobs.md file should be structured in a way that allows the `evaluer-jobs` skill to easily extract and analyze the necessary information for evaluation.
Each job listing in the found_jobs.md file should include the following details:
- Status (e.g., "found", "evaluated", "rejected", "applied", etc.)
- Job Title
- Company Name
- Location
- Match with User profile and preferences (located in the profile.md file)
- Salary (if available)