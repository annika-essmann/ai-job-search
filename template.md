# Prompt to find data analytics jobs

*-- This is a blank version of my job search prompt. Text in italics are comments for you to understand the structure. Delete them after drafting your own prompt. Text in [square brakets] are placeholders for you to fill in.*

*-- General recommendation: Save the prompt as a skill if your AI tool supports it. That way you can tell the AI to execute certain phases only.*

## Step 0: Your task
You are an expert job search assistant. Your task is to find job openings for data analytics roles that match the criteria that I will provide to you. 

Important: Work in phases. Wait until I tell you which phase you should execute.
- **Phases 1-3**: Search job platforms.
- **Phase 4**: Apply industry filter
- **Phase 5**: Search company career pages
- **Phase 6**: Compile a raw list, apply job posting criteria that I specify and remove duplicates
- **Phase 7**: Output a final table
- **Phase 8**: Write a source reconciliation checklist

**Important**: Do not produce the final table until all prior phases are complete.

**Important**: Do not stop early. If you cannot access a source, do not fabricate results.

**Important**: After searching each source, output a brief numbered list of every job posting found, with platform name, company, title, date, and URL. Always follow this instruction even if you found zero results. If you did find zero results, return "No matching results found”. Carry this list forward into subsequent phases.

*-- This last sentence is crucial, otherwise, the AI tool 'forgets' the results of previous phases.*

## Phase 1

*-- Phases 1-3 all search for jobs in platforms like LikedIn and Stepstone. They are grouped into separate steps because each platform needs different instructions. Also, most AI tools have a limited amount of web searches. If you have more platforms than this limit, the AI might not visit the platforms after the limit has been reached.*

### Step 1.1: Search job platforms that support URL-based search queries
For each platform, first use web search with the platform name and search query parameters such as, but not limited to: [the job titles you are looking for in "double quotes" separated by commas, e.g. "Data Analyst", "BI Analyst"]. Also search broader terms like [use keywords that might appear in job titles, e.g. "data", "analytics"] combined with [your city] or "Remote".

Then fetch individual job detail URLs from the results.

If you cannot access a platform or if it blocks automated access, note this as “no access possible” and move to the next platform.

Construct the direct search URL by combining the base URL with the search query parameters. Try multiple combinations of the search query parameters to find more job postings.

- [your list of job platforms]

## Phase 2

*-- The following step might be irrelevant to your job search if you don't have a job platform that works like get-in-it.de. If so, then delete this step and adjust the numbering accordingly.* 

### Step 1.2: Job platforms with specific instructions
For each platform, first use web search with the platform name and search query parameters such as, but not limited to: [the job titles you are looking for in "double quotes" separated by commas, e.g. "Data Analyst", "BI Analyst"]. Also search broader terms like [use keywords that might appear in job titles, e.g. "data", "analytics"] combined with [your city] or "Remote".

Then fetch individual job detail URLs from the results.

If you cannot access a platform or if it blocks automated access, note this as “no access possible” and move to the next platform.

Visit the platform and search for job postings by following the instructions noted down after the URL.

- https://www.get-in-it.de/ - fetch the page https://www.get-in-it.de/jobsuche and review all visible listings by using the search query parameters. Note that this platform uses a reverse recruiting model and may not display all open positions publicly. If no matching roles are visible, state this explicitly

## Phase 3

*-- The job platforms in this section do not use an URL-based search. For me, it worked to visit the page once, select all the filters that I wanted to 'construct' a specific URL. Then, I copy-pasted this URL into the prompt.*

### Step 1.3: Job platforms with specific URLs
For each platform, first use web search with the platform name and search query parameters such as, but not limited to: [the job titles you are looking for in "double quotes" separated by commas, e.g. "Data Analyst", "BI Analyst"]. Also search broader terms like [use keywords that might appear in job titles, e.g. "data", "analytics"] combined with [your city] or "Remote".

Then fetch individual job detail URLs from the results.

If you cannot access a platform or if it blocks automated access, note this as “no access possible” and move to the next platform.

Visit each platform and search for job postings by accessing the given URL (if possible) and by using the search query parameters. 

- [the specific URL of your job platform]

## Phase 4

### Step 2: Appyl industry filter
Take the result from phases 1-3.

Exclude openings from these industries entirely:
- [the industries in which you do not want to work at all]

Do not use this filter on phase 5.

## Phase 5

### Step 3: Search company career pages
These are target employers regardless of size and industry. Visit the career page of each company listed below and search for [the job titles you are looking for in "double quotes" separated by commas] combines with [your city] or "Remote".

If you cannot access a career page, note this in 2-3 sentences and move on. 

*-- The following instruction is important because many career pages use JavaScript to display their job openings. With this prompt you know why no jobs were found; otherwise, the AI might silently drop the page.*

If a career page returns no job listings due to JavaScript rendering, note this explicitly in Phase 8 in the reconciliation checklist.
- [list of your favourite employers; it's potentially good to paste the entire URL after you have selected all filters, see. step 1.3]

## Phase 6

*-- The following step is crucial, so that the AI views the results of all previous steps as one, big list with which it should continue working.*

### Step 4: Compile a raw list
Before producing the final table, compile a complete raw list of results from phases 1-5. Confirm the total count. 

### Step 5: Apply job posting criteria
Take the results from step 4.

These job postings must pass all of the following hard filters:
- **Recency**: The job posting is 7 days old or younger at the time of your search.
- [list of your criteria that a job posting must pass, e.g. commuting radius or working hours]

A posting must also meet at least 1 of the following [X] criteria: 
- [list of further criteria, e.g. when you want to filter for certain tasks in the job description]

### Step 6: Remove duplicates
If you find the same job opening on both, a platform (phases 1-3) and a company career page (phase 5), keep only one entry. Prefer the company's own career page URL as the source link.

## Phase 7
### Step 7: Output the final result
*-- The following description is just an example of how you could describe your output. Adjust it to your needs.*

- **Date**: The publication date of the job posting in the German format DD.MM.YYYY
- **Company name**: The legal or brand name of the hiring organization.
- **Job title**: The exact title from the posting. Keep the original German title
- **Location**: Mention whether the role is on-site in [your city], within 10-20km, or remote.
- **Working hours**: Write down the amount of hours per week in numbers only. If the role is only marked as full time, return “40”. 
- **Source**: Write down the source where you found the job posting. 
- **URL**: Direct link to the job posting.

## Phase 8

*-- This last phase is crucial; that way the AI checks its own work.*

### Step 8: Write a source reconciliation checklist
List every source searched. For each, state: (a) number of results found, (b) number included in the final table, (c) number excluded with brief reason. If any source has zero results in the table, confirm it was searched and explain why no entries qualified.