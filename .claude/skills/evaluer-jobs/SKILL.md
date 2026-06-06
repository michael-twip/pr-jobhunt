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

## Dialog

Present the user with the list of job opportunities found by the `find-jobs` skill, along with their details and the feedback provided by the `evaluer-jobs` skill. The user can then review the feedback and make informed decisions about which job opportunities to pursue further based on their relevance and quality. The dialog should allow the user to easily navigate through the list of job opportunities and access the feedback for each listing to facilitate their decision-making process.

The user is not expected to read the found_jobs.md file directly, but rather to interact with the information through the dialog interface provided by the `evaluer-jobs` skill. The skill will present the job opportunities in a user-friendly format, allowing the user to easily understand the relevance and quality of each listing based on the feedback provided. The dialog should be designed to help the user quickly assess which job opportunities are worth pursuing further and which ones may not be a good fit based on their profile and preferences.

Ask if the position is a good match and whether the user would like to pursue it further. If the user indicates that they are interested in pursuing a particular job opportunity, the `evaluer-jobs` skill can provide additional information and guidance on the next steps to take, such as how to apply for the job or prepare for an interview. If the user indicates that they are not interested in pursuing a particular job opportunity, the `evaluer-jobs` skill can provide feedback on why it may not be a good fit and suggest other job opportunities that may be more relevant to the user's profile and preferences. The dialog should be designed to facilitate a smooth and informative interaction between the user and the `evaluer-jobs` skill, helping the user make informed decisions about which job opportunities to pursue based on their relevance and quality.