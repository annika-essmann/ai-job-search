# The AI searches for jobs, I apply: How I reduced my job search from 2 hours to 15 minutes

*This is a translation of my [LinkedIn article](https://www.linkedin.com/pulse/erstelle-deinen-prompt-f%C3%BCr-die-jobsuche-annika-e%C3%9Fmann-n1q6f/) published in German on Sept 21, 2026.*

*The file [template.md](template.md) in this repository outlines a blank version of my job search prompt. You can use it to start your own prompt right away.*

## Create your own job search prompt
It had long bothered me that finding suitable jobs to apply for took me like forever. So I built a master prompt for myself that runs five pages long. Now the search no longer takes me 2 hours, but 15 minutes.

Step by step, I'll walk you through how I built it.

## ✍️ Prepare your information
- Collect job platforms: Which websites do you use to search for jobs?
- Draw up a shortlist of companies: Which companies do you find exciting?
- Write down your criteria for your job search: What matters most to you?
- Collect links to job descriptions: What did you last apply to?
- Visualise the result: Should it end up as a table, a dashboard, or something else entirely?

## ✅ Results of your preparation
- Job platforms as URLs
- Career pages as URLs
- List of your criteria, e.g. work model, commuting radius, or preferred industries.
- URLs to job postings you have applied for
- A precise, brief description of what your result should look like, e.g. the number of columns in a table and their headings.

## ❗ Good to know
Use several chats so the AI can, for example, critique analysis results or first drafts. If you put everything in one chat, the tool won't be critical enough and may also lose track of things.

Document every step, because the process can turn into a real slog very quickly. Trust me. 😅

## 🔎 Uncover hidden criteria
Have the job postings you've already applied for analysed to find out what criteria you've been filtering by without realising it. You can then add these to your list of criteria.

    Role: You are helping me find potential job openings. Task: I will give you job postings I have already applied for. Carry out a multi-stage analysis. [the links to your job postings] Compare the postings: What do they have in common? Define up to 10 criteria that capture what these job descriptions have in common. Goal: I want to use these criteria later to find more similar job postings.

## 💬 Let AI be the quiz master
Put everything you have so far into one chat and prompt the AI to ask you questions so you can build a master prompt together.

    Role: You are helping me create a prompt for an AI to find job openings on the internet. Task: Complete the task in several steps:

    Read my entire message. Do you have any questions about my task? Ask those first before continuing.
    Read this information and use every detail to create the prompt.

    2.1 Job platforms
    [Your list of job platforms]
    Include any potential companies, provided they meet the criteria named in step 2.3.

    2.2 Career pages
    In addition to step 2.1, search the career pages of the following companies for job openings.
    [Your list of companies]
    If you cannot access a career page, explain why in one sentence. Do not create duplicates. If you find the same posting in both step 2.1 and 2.2, keep only one.

    2.3 Criteria for the job posting
    [Your criteria]

    2.4 Final result
    [Your description]

## 🤔 A little criticism goes a long way
Have the master prompt critiqued in a new chat – preferably more than once, to expose its weak spots.

    You are a prompt engineer. I wrote this prompt to search for job openings in the field of [your field]. Task: Give me up to three suggestions for making the prompt deliver more precise results. Any questions before we begin?

## 💻 Test the prompt
Put the master prompt to the test: Does it deliver what you want? Review the output and click through the links to the job postings. If problems occur, think about how to fix them, and if you can't come up with a solution, ask the AI for advice – in the same chat where you ran the test.

**💪 Your master prompt is ready!**

## 💡 Tips
If your prompt is very long, split it into phases and state at the beginning that the AI should maintain a running list of all job postings it has found, and carry that list over into subsequent phases.

If you have several job platforms and companies, the AI may fail to treat the search results as a single list on which to apply your criteria. To avoid that, ask the AI in an extra step to compile all results into one master list and work with that list for all subsequent phases.

Save the prompt as a skill or project description if your AI tool supports it. That way you won't have to keep pasting the prompt — you can simply tell the AI which phase to run.

Let the AI review its own work: right at the end, after it has produced your result, instruct it to compare the search results against the output: Is everything there, or did the AI "forget" something?

*Info: I use GreenPT's Starter subscription for this master prompt. It's fairly token-heavy, and I can well imagine it would be very slow on free plans, or that the memory available wouldn't be enough for a good result.*