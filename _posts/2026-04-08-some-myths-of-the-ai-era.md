---
title: Some myths of the AI era
author: wenzy
date: 2026-04-08 19:43:00 +0800
categories: [Blogging]
tags: [tool, woolgathering]
math: true
mermaid: true
pin: false
---

{% include embed/spotify.html id='5r3Sm0HSUDpnq3WPDULvvE' %}

![CC robot](/assets/img/claudecode-color.svg)

In 2023, I used AI to assist with research for the first time. I fed various tasks to the most popular tools of the moment, including revising paragraphs, correcting grammatical errors, and standardising terminology. I then tested a few code-editing jobs as well. After several rounds of experimentation, I settled on Claude as my primary AI tool. The main reason was straightforward: even without any personalised configuration, its output was consistently concise and clear. Of all the response styles I encountered, it was the least taxing to read. This reminded me of how I prefer to communicate with people in real life. I find direct, no-nonsense exchanges the most comfortable.

At first, I did not move quickly into heavy AI usage. Partly out of distrust of the results, I treated it mostly as a fallback when a Google search had already failed me, or as a tool for rapidly generating repetitive work I already knew well but was too lazy to redo from scratch. Claude performed well on these tasks, and so from early 2025, I began gradually expanding the ways I used it. The process also sharpened my ability to write prompts. I started to notice that, given the same task, I was retrieving more accurate information faster than I had before, and faster than colleagues who were also using AI.

Over those first few months, a handful of experiences stood out.

One was my first attempt at using Claude to generate a quality report from already-analysed data. For the first time, I realised I could produce an interactive webpage that would spare me the friction of explaining things to collaborators. Previously, joint reports meant sending charts or compiling slides, which invariably required additional rounds of clarification. An interactive report page, by contrast, lets the reader click through to whatever data they want, with explanations already there, removing the need for the low-efficiency back-and-forth that usually follows.

Another experience came when everyone in the group needed to present their progress at a lab meeting. It was informal, so there was no expectation of detailed background introductions, but that was precisely what made it difficult for me. My work sits at the margins of the group's main focus, and without some context, it is hard to convey what I am actually doing. It then occurred to me to use AI-generated diagrams to illustrate the new concepts and terminology. This turned out to be far more intuitive than the dense figures typical of a literature review. The diagrams went down well, and I later noticed that some colleagues had started adopting similar approaches for their own presentations.

A third experience came when my supervisor asked me to help with a large volume of targeted web scraping and summarisation, collecting supplementary material he wanted to include in a grant application. This was entirely outside my area of expertise, so it was the first time I seriously thought through how to vibe-code a small tool capable of doing the job. That experience gave me a concrete sense of how AI tools can enable someone without specialist programming knowledge to accomplish tasks that would otherwise be genuinely laborious.

All of these were achieved through browser-based conversations as a free user with a modest usage quota. They made me want to go further and properly explore vibe coding. Getting there took some effort. Living in a region where things have a way of not working straightforwardly, and relying on tools from a company subject to strict regional controls, I spent a fair amount of time before I finally managed to set up Claude Code and the other extensions I needed.

Once everything was deployed, I felt like I was learning something new at every turn. For instance, rather than installing Claude Code on a remote server or relying on unstable remote access via SSH and the university intranet, is there a better way to operate in a remote environment? Credit here goes to my friend Yang, whose suggestion made it click: my terminal is already connected, so the agent does not need to establish its own connection. It simply needs to use the session that is already open through my existing channel.

There is also a question I am still working through and have not fully resolved. In software development, many programmers have gone all-in on vibe coding. Their typical architecture involves several tasks divided up by load-balancing strategy, explored in parallel, with the results from each compiled into a report. Those of us doing data analysis have not yet developed an equivalent top-down view, one where we think through, in advance and in full, which analyses a given dataset requires and which of those can be pursued in parallel. Pipeline-style work can be planned this way, but the exploratory work that follows tends to be serial and largely improvised. You notice something, think of something, and go try it. As a result, AI agents end up as ad-hoc workers, called upon in new sessions to handle discrete problems, rather than long-term participants embedded in the project. This may partly reflect the nature of my current work, as things feel different when writing software. The question I keep returning to is whether this kind of workflow can be restructured into something more collaborative, where the AI agent and I are both genuinely and continuously engaged together in the same project. If we have not yet established this kind of deep collaborative mode, does it follow that we have not fully unlocked the potential of AI agents in bioinformatics data mining as it currently stands?
