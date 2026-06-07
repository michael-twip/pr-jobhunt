name: find-jobs
description: Find job opportunities based on the specific profile and location provided in the `profile.md` file.
---

## Task Overview
The `find-jobs` skill is designed to help users find job opportunities based specifically on the profile and location provided in the `profile.md` file. The skill will search for job listings that match the user's profile and preferences, taking into account factors such as job title, company reputation, location, salary, and required skills. The skill will utilize various job search platforms and databases to gather relevant job listings that align with the user's criteria.

The output of the `find-jobs` skill will be a list of job opportunities that are 
relevant to the user's profile and location. Each job listing will include details such as job title, company name, location, salary (if available), and a brief description of the job requirements and responsibilities. The found job listings will be stored in the `found_jobs.md` file, which serves as a working document board for the `find-jobs` skill. This file will allow the user to review and evaluate the found job opportunities before deciding which ones to pursue further. 

The `find-jobs` skill will also provide information on where each job listing was found, such as the specific job search platform or database used to locate the opportunity. This information can help the user understand the source of each job listing and potentially explore similar opportunities on the same platform. Overall, the `find-jobs` skill aims to streamline the job search process by providing users with a curated list of job opportunities that are tailored to their profile and location, making it easier for them to find relevant job openings and take the next steps in their job search journey.

The `find-jobs` skill will utilize the information provided in the `profile.md` file to ensure that the job listings it finds are relevant and aligned with the user's career goals and preferences. The skill will analyze the user's profile, including their skills, experience, and desired job criteria, to filter and identify job opportunities that are a good match. By leveraging various job search platforms and databases, the `find-jobs` skill will aim to provide a comprehensive list of job opportunities that meet the user's specific requirements, ultimately helping them find suitable job openings more efficiently. 

Each job listing found by the `find-jobs` skill will be structured in a way that allows for easy evaluation and comparison. The listings will include key details such as job title, company name, location, salary (if available), and a brief description of the job requirements and responsibilities. This structured format will enable the user to quickly assess the relevance and quality of each job opportunity and make informed decisions about which ones to pursue further. The `find-jobs` skill will also provide information on where each job listing was found, such as the specific job search platform or database used to locate the opportunity. This information can help the user understand the source of each job listing and potentially explore similar opportunities on the same platform. By providing a curated list of job opportunities that are tailored to the user's profile and location, the `find-jobs` skill aims to streamline the job search process and increase the chances of finding relevant job openings that align with the user's career goals and preferences.

Make sure to respect the found_jobs file statuses. If status have been set to rejected, do not include those again. If a company has been marked as rejected,  do not include any opportunities from that company. 

Do not include opportunities that are  marked as closed in any of the job search platforms or databases, unless the opportunity is still open according to the company website, the position has a high chance it might be reopened or there's an extremely good reason to include it.

## Verification Step — Required Before Adding Any Match

Before adding a job opportunity to `found_jobs.md`, you **must** verify that the position is genuinely open using at least two of the following methods:

1. **Fetch the company's own careers page** (e.g. `company.com/careers`) and confirm the role is listed there right now.
2. **Fetch the direct job posting URL** and confirm it does not show "removed", "expired", "no longer available", or similar language.
3. **Check a secondary source** (e.g. builtin.com, LinkedIn, Glassdoor, greenhouse.io, ashbyhq.com) and confirm the listing is active — not cached or closed.

Search engines (Google, Bing) cache job postings for months after they are removed. A job that appears in search results is **not** confirmed active — the original page must be fetched and verified. Do not rely on a search snippet alone.

If a listing cannot be confirmed open on the company's own site or a live job board, mark it as `Lukket` and move it to the market intelligence section rather than the active section.

Stop if you have found 50 job opportunities or if you have exhausted all relevant job search platforms and databases. The `find-jobs` skill will prioritize quality over quantity, ensuring that the job listings it provides are highly relevant and aligned with the user's profile and location.


 