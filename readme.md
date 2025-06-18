# LLM powertools

Pre-requisite:

- [install `llm`](https://llm.datasette.io/en/stable/setup.html)
- `llm install llm-templates-github`

Setup:

```shell
$ llm fragments set brief path/to/brief.md
$ llm fragments set resume path/to/resume.md
```

Usage:

```
# Make sure everything is working by summarizing your job search parameters
llm -t gh:therealadam/jobby-summary

# Given a job description on the system pasteboard, evaluate a match based on your brief and resume
pbpaste | llm -t gh:therealadam/jobby-match

# Given a job description on the pasteboard, get ideas on how to reply to a question on the job application form
pbpaste | llm -t gh:therealadam/jobby-answer "what's your strongest skill"

# Given a job description, get ideas on what to write in a cover letter
pbpaste | llm -t gh:therealadam/jobby-cover
```

Good luck out there, it's tough finding a new job these days.
