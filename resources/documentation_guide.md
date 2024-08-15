# A guide to documentation

I’m going to let you in on a secret: programmers don’t know everything. They are _constantly_ looking up documentation, searching for solutions to questions, and synthesizing the results to fit their program’s purpose.

Being an effective programmer is much less about having coding chops than it is about knowing trusted sources of information online and how to locate helpful content within them. In the same way that an informed news consumer seeks out articles from publications of record to corroborate stories, an informed coder seeks out content from specific sites they have learned are reputable.

If you become effective at searching for trusted documentation — and confident and tireless in your pursuit of solutions to your problems — you are on an even foot with the best of programmers.


## What is documentation?

Broadly, documentation is any content that can tell you how to do _something_, like how to use a tool or solve a task.

People often refer to documentation in the narrow sense of an instruction manual authored by the creator of a coding package to help users. We’re using the broader sense of documentation as a way to get something done because the skills needed to interpret good documentation apply across all sorts of content.

Say you have a problem: you want to extract text from an image. Actually from 10,000 images from a secure document dump you’ve received. Computers are good for automating tasks at scale — they should be able to do this, right?

You open Google and type “how to extract text from images programmatically.” A variety of results pop up:

- A Reddit forum post asking an online community of technologists the best OCR (optical character recognition) tool

- A Medium blog post on “Top extraction tools 2024”

- A GitHub repository for a tool called Tesseract that calls itself “A command-line tool for optical character recognition”

- A getting started guide for a Python package called _paddleOCR_ hosted on ReadTheDocs

- A page on “tools to extract text from images” from the question-answer site “StackOverflow”

So, which of these do you think is documentation? Surprise! They all are.


## Finding documentation

The above search query, “how to extract text from images programmatically,” got us a variety of answers. Maybe too much variety.

Searching for documentation often requires articulating your specific needs concisely as keywords. And it often entails an iterative process of refining the search terms to be more specific as you learn more about what is going to be a good solution for you.

In this scenario, we noticed “OCR” popped up a lot in the search results. If we are unfamiliar with the term, we could search “what is OCR” and click on a Wikipedia article about “Optical character recognition,” read the first paragraph, and ascertain that OCR is exactly the type of technology we were looking for: a method to extract text from images programmatically.

How do we prefer OCRing our images? The results above surfaced high-level surveys of the field, command-line tools, Python libraries. We are lucky that OCR is a widely studied field and has a good amount to offer in the open source world.

Based on our research, let’s opt for running OCR on the command-line. The command-line is a handy. It’s a portal for running all sorts of ready-made tools written in a variety of programming languages (without requiring us to know those languages!).

Google: “Command-line tool OCR.” Now we’re talking.


## Evaluating documentation

Building a mental hierarchy of trusted documentation sources is something coders develop over time. And it can be hard to reliably evaluate information when content-farmed articles are spamming Google in contention for your attention.

We’re going to give you some shortcuts. Here is a rough hierarchy of sources, ranked from most trustful to least:

- **Source code:** it is the hardest to read and often a last resort. But the source code of a program is the authoritative reference for how a package is developed

- **README.md files from GitHub:** this is usually the first destination to go looking. By convention, most code packages have a top-level README.md file targeted to users of the code. GitHub is by far the most popular source code provider, but don’t be alarmed if you see code hosted on alternative platforms like GitLab.

- **Documentation site linked by the GitHub repository:** If a documentation site is linked by the README.md file or in the sidebar of the code repository, you can be sure the content is authored by the creators. These sites are usually HTML pages, with URLs sometimes ending in “github.io” (an easy web-hosting solution from GitHub) or hosted on an open source documentation platform like ReadTheDocs.

- **Documentation site from official standards:** If you have a Python question, the Python.org documentation is going to have the most up-to-date content. If you have a question about HTML or CSS, MDN is where you should go. Be more wary of for-profit companies with no obligation to have up-to-date truthful content like W3Schools.

- **Community question-answer forums:** Like Wikipedia, these sites are crowd-sourced but often have high quality content:

  - **StackOverflow:** This is the most trustworthy question-answer forum. There is a reputability system and regulations on providing helpful, detailed answers. When you find an upvoted or accepted answer to a specific problem you have here, it often is correct,

  - **GitHub issues:** each repository on GitHub has an “Issues” tab and some have a “Discussions” tab. Content here is often written by technical users, but there are fewer safeguards than StackOverflow.

  - **Hacker News:** This is a forum of technical professionals. You are not likely to find answers to very specific questions here but often find helpful discussions and content the best general ways to accomplish specific tasks.

  - **Reddit:** Reddit forums sometimes have exactly what you’re looking for. But it’s generally more of a jumble of content and experiences.

- **Blog post:** This is a hard category to evaluate. Lately, platforms like Medium and TowardDataScience have become spammed with low-quality content. But sometimes you will stumble upon a technologist’s personal blog and find real gems. Generally be very wary of what you read in one of these categories, and try to cross-reference anything that you do pick up from here. Sometimes it is the only place you’ll find the answer.


## Reading documentation

When you encounter a long piece or detailed web of authoritative documentation, it can be tempting to jump elsewhere for a more attention-grabbing quick snippet. Sit with that discomfort. Read what the developer or package maintainer has written. Pay attention to caveats and notes. Go on side quests to explore other pages of the documentation that are not directly relevant to what you are looking for. You never know when knowledge you have serendipitously absorbed will come in clutch in the future.

Be patient. Sometimes you will need to find other sources of documentation just to understand a paragraph of the primary source documentation. If there are sections you don’t understand and can’t figure out, ask questions. Submit a GitHub issue, reach out to the developer, ask other community members who may know. Persistence usually pays off or leads to unexpected opportunities for collaboration.


## Troubleshooting

Very often things won’t go right. Computers are incredibly versatile pieces of technology, but with that comes a slew of slight differences. Different operating systems. Different versions of operating systems. Different versions of software installed. Different configurations. Different underlying hardware. Out-of-date documentation.

The first step when you encounter a problem is to recognize 1) this is a normal situation, and 2) this is not anyone’s fault but a natural consequence of working with the flexibility of modern computing.

When you encounter an error, read the error message carefully. Do not be alarmed by a potpourri of strange symbols — developers do not often leave friendly or decipherable clues. But try to identify the core of the message and interpret what it is attempting to tell you. It won’t always make sense, but sometimes you’ll figure out what’s wrong on your own. Or you’ll know better what to do next.

Google search the issue. If the error message is short, it can make sense to paste the whole thing in to the search bar. Usually you’ll want to search just the relevant part of the error message. And you’ll often want to specify the program you were using. For example “tesseract unsupported file format webp.”

As you evaluate the search results, apply many of the tricks from the evaluating documentation section. GitHub issues are a great source, especially if it’s from the repository’s GitHub. You may want to go to the repository directly and use the search functionality within GitHub issues. You may want to use Google search but append the keyword “GitHub” or “Stackoverflow.”

Sometimes you will learn that the problem you are encountering is not related to the program you are using. This may take some additional research to figure out. For instance, the software may not be compatible with your operating system. Or you may need to update some other piece of software to a new version.

Do not shy away from asking for help, on GitHub, a forum, or to a colleague.

Lastly, some problems are best solved by relaxing and taking a short break. Often the solution comes to you passively while working on something else or getting fresh air. Try not to get too wrapped up in any issue and let yourself figure it out later.


## On the use of A.I.

A.I. chatbots are all the rage. And for good reason: they are very helpful much of the time. In the ripe year of 2024, most users understand the limitations of ChatGPT and other large language models (LLMs). They are prone to hallucinations, occasionally gaslighting you with confident falsehoods. We won’t harp on it.

Instead, let’s discuss the very real ways that chatbots can be helpful. And what to watch out for.

Chatbots are content synthesis engines. They have absorbed unfathomable troves of content from the web and answer questions by blending it all together in impossible-to-interpret ways. They are biased by the content they have been trained on and will have less exposure to newer tools or underrepresented technologies. They don’t have any inherent knowledge of truth; they just know how to give a probabilistic impression of truth. In other words, they bullshit effectively. So effectively they are very often correct.

A.I. chatbots are good for providing tutoring on a new topic, explaining concepts you don’t understand, diagnosing error messages, and writing a first-draft of code to accomplish rote tasks.

Here are some example ways to use A.I. effectively:

- “I am a data journalist who is learning how to OCR documents. Explain what tools might make sense for my task and why”

- “I would like to learn more about writing quick Python scripts to accomplish simple tasks without going through all the fundamentals of programming. Put a sample curriculum together for me”

- “Why am I getting ‘command not recognized: chdir’ when trying to change directories in my windows terminal?”

- “Write me a quick Python script to go through all the files in the ‘data’ folder, pull just the .png files, and then run the command-line tool tesseract on them, outputting a corresponding .txt file in the ‘data’ directory”

Use A.I. technology with a grain of salt. When it writes a guide on a subject, cross-check its output with authoritative documentation, or prompt it to point you to more official sources to read. Use LLMs to help you in open-ended ways, like ideating questions to ask, pointing you to terms to put into traditional search engines, evaluating pros/cons, identifying errors, and writing commands that you have the ability to verify yourself.
