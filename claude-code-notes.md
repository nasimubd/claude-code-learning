# Claude Code Essentials — Learning Reflection
**Author:** @nasimubd  
**Course:** Claude Code Essentials by Andrew Brown (ExamPro)  
**Completed:** <!-- Add date -->

---

> **Scoring Guide:** Each section is rated **0–9** for relevancy to my role.  
> - **9** = Directly applicable, use this constantly  
> - **5** = Moderately relevant, situational use  
> - **0** = Not relevant to my current work  
>
> For each section I cover: **Why** it matters, **When** I'd use it, and **What** it means for my role.  
> *(The "How" is covered in the course videos.)*

---

## 1. Introduction

### Intro & Meet your Instructor
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### Claude Code Essentials & Guest Instructor
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

---

## 2. Core Concepts and Foundations

### Agentic Coding Tools & Comparisons
- **Relevancy:** `3/9`
- **Why:** The section exists to give learners a market overview — Claude Code, OpenAI Codex, Amazon Q, and OpenCode are the main players covered. It demonstrates how these tools perform the same tasks side by side, but that context is useful for someone choosing a tool for the first time, not for someone who has already committed to Claude Code.
- **When:** Only relevant if EonLabs ever evaluates switching tools or integrating a second agent into the pipeline. That's a low-frequency decision, not a day-to-day one.
- **What:** This section is not technically informative — it's a performance comparison across tools. Since the decision to use Claude Code has already been made, the comparative content doesn't translate into anything actionable for the research engineering role at EonLabs.

### What is a Code Harness & Claude Code?
- **Relevancy:** `5/9`
- **Why:** A Code Harness is the concept of wrapping a large language model into a coding agent by adding engineering prompts, tools like sandboxes, and the ability to control or restrict certain bash commands. Understanding this is foundational context — it explains what Claude Code actually is under the hood, rather than just how to use it on the surface.
- **When:** Relevant when needing to explain the tooling to others at EonLabs, or when evaluating whether to enhance Claude Code with custom skills or tighter permission controls for specific repository tasks. Also relevant when deciding which surface — web, CLI, or VS Code extension — is most appropriate for a given research workflow.
- **What:** This is conceptual rather than directly technical, but it matters because it provides the mental model needed to make better decisions when extending or customizing Claude Code. For a research engineering role where the goal is to go beyond standard usage and build more disciplined, purpose-specific workflows, understanding what a Code Harness is — and what it enables — is necessary context.

### The Agentic Loop: Tool Calls & Models
- **Relevancy:** `5/9`
- **Why:** The Agentic Loop describes how Claude Code processes a prompt in a structured sequence — gathering context, taking actions, and verifying results. It can call internal tools within Claude Code as well as reach out to external programs for additional context. Understanding this loop is foundational to knowing how Claude Code thinks and executes, which is necessary before trying to direct it effectively.
- **When:** Relevant when diagnosing why Claude Code is behaving unexpectedly on a task, or when designing more precise prompts that align with how the loop actually works. Also relevant when deciding which external tools or context sources to make available to Claude Code for a given research task.
- **What:** Like the Code Harness, this is conceptual rather than directly technical. But for a research engineering role, understanding the loop means you can anticipate where Claude Code might go wrong — for example, gathering the wrong context or failing to verify an output — and design your workflows to account for that. It is the kind of foundational knowledge that makes every subsequent technical section easier to apply correctly.

### Claude Modes & Additional Resources
- **Relevancy:** `6/9`
- **Why:** The additional resources point beyond the course itself — to documentation and other ExamPro materials. For a research-based role, the videos alone set a ceiling on what you can learn. When facing problems that the course doesn't cover, knowing where to go for deeper, more authoritative information is essential.
- **When:** Relevant whenever a specific problem or edge case arises that the course videos don't address. In a research engineering context, these situations will be frequent — the work regularly goes beyond what standard tutorials cover, and having a clear path to deeper documentation means less time blocked and more time moving forward.
- **What:** For your role at EonLabs, this section is less about Claude Modes specifically and more about the habit of going beyond the surface material. Terry explicitly expects you to distill assumptions and question standard approaches — that kind of thinking requires access to deeper context than any single course can provide. Knowing how to navigate the documentation is what separates someone who uses Claude Code from someone who truly understands it.

### Subscription, Usage & Auth Errors
- **Relevancy:** `5/9`
- **Why:** Understanding subscription models and usage patterns is not immediately critical, but it has long-term value. As Claude Code is used more intensively across research workflows at EonLabs, knowing how usage is tracked and billed becomes important for ensuring that the tooling is being used efficiently and cost-effectively.
- **When:** Relevant in the future when reviewing how Claude Code resources are being consumed across different tasks and workflows. As the research workload scales — more agents, more parallel sessions, more repository monitoring — subscription efficiency becomes a meaningful operational concern.
- **What:** For your role, this section is a long-term reference rather than an immediate priority. The goal is to eventually develop a clear picture of how subscriptions are being utilized, identify any inefficiencies, and ensure that the way Claude Code is being used aligns with what the subscription model actually supports. Efficient tooling use is part of operating like a disciplined research engineer, not just a technical one.

### System Requirements & Doctor CLI
- **Relevancy:** `4/9`
- **Why:** This section covers the initial setup and configuration of Claude Code, including installation methods like Homebrew and other terminal commands, as well as built-in CLI commands like `claude login` and `claude logout`. For someone setting up Claude Code for the first time, this is essential — without getting the environment right, nothing else in the course applies.
- **When:** Relevant once, at the very beginning of onboarding. Once Claude Code is installed and configured correctly, this section becomes a reference rather than an active resource — useful only when something breaks or needs to be reconfigured on a new machine.
- **What:** For your role, this is beginner-critical but not research-critical. The value is in getting unblocked quickly so you can move on to the work that actually matters — monitoring repositories, running agents, and testing hypotheses. The faster the setup is done correctly, the sooner the real research engineering work can begin.

### Install CLI: PowerShell, CMD, Linux & VSC
- **Relevancy:** `4/9`
- **Why:** This section is a practical extension of the previous one, covering how to install Claude Code across different environments — PowerShell, Command Prompt, WSL2, the VS Code terminal, and as a VS Code extension. It is not deeply technical, but it is highly relevant for anyone setting up the tool for the first time across different operating systems.
- **When:** Relevant during initial setup, and again whenever Claude Code needs to be configured on a new machine or environment. Also useful when helping others at EonLabs get the tool running, as having this context means you can guide the process without needing to look it up.
- **What:** For your role, the value is practical rather than conceptual. Knowing the different installation paths means you are not blocked by environment-specific issues when starting a new research session. It also ensures that Claude Code can be run in whichever surface — terminal or IDE — is most appropriate for the task at hand.

### Interactive Mode & Ctrl+C
- **Relevancy:** `6/9`
- **Why:** Interactive mode is the primary way of working with Claude Code in real time — typing `claude` launches a live session with real-time feedback on actions taken and files edited. The key commands for managing a session (Ctrl+C, Escape, Ctrl+D, `/exit`, Ctrl+L) are small but essential habits that directly affect how smoothly a research session runs.
- **When:** Relevant every single time Claude Code is used. These are not one-time setup steps — they are the basic controls for navigating an active session. For a role involving high volumes of edits, planning, and iterative research tasks, knowing how to cancel, exit, and clear without losing context is something you will rely on constantly.
- **What:** For your role at EonLabs, maintaining focus during long research sessions is important. The ability to clear the screen without losing conversation context — keeping the session clean while preserving progress — directly supports the kind of sustained, deep work that Terry expects. These are small controls, but they add up to a meaningfully better workflow when you are running multiple tasks and managing complex research sessions.

### Auth Tokens, Stats & Usage Limits
- **Relevancy:** `5/9`
- **Why:** Understanding how auth tokens work and how to track usage through the `stat` command gives visibility into how Claude Code resources are being consumed. Even as subscription models evolve, having a clear picture of token utilization is useful for working efficiently and avoiding unexpected limits mid-session.
- **When:** Relevant on an ongoing basis, particularly during heavy research sessions where multiple agents or long context windows are in use. Checking stats periodically helps ensure that token usage is aligned with the work being done and that no resources are being wasted on unproductive tasks.
- **What:** For your role, this is less about the technical mechanics of authentication and more about operational awareness. Knowing how many tokens have been used so far in a session informs decisions about when to compact, clear, or restructure a workflow. As the tooling at EonLabs scales up, that kind of visibility becomes increasingly important for running research sessions that are both effective and efficient.

### Sessions: Resume, Fork & Context Commands
- **Relevancy:** `7/9`
- **Why:** Research work is rarely completed in a single sitting. The ability to resume a session without losing context means you can take breaks, return to a problem with fresh eyes, and continue exactly where you left off. The fork command adds another layer of flexibility — allowing you to branch off an existing conversation to explore a different hypothesis or approach without disrupting the main thread.
- **When:** Relevant constantly throughout research workflows. Resume is useful whenever a session needs to be paused and continued later. Fork is particularly valuable when testing a non-consensus hypothesis alongside the baseline — you can branch the conversation at the point where the approaches diverge, keeping both threads intact. The context command is useful whenever a session is getting long and you need to assess whether you are approaching the limit.
- **What:** For your role at EonLabs, these commands directly support the kind of iterative, multi-hypothesis research Terry expects. Being able to fork a session means you can test different angles from the same starting point without starting over, which is exactly the discipline of running a baseline and a non-consensus hypothesis in parallel. Managing context carefully also ensures that Claude Code has the right information at every stage of the research process, not a cluttered or oversized window that dilutes the quality of its responses.

### Compact, Clear, Rename & Rewind
- **Relevancy:** `6/9`
- **Why:** As research sessions grow longer, context management becomes critical. The `compact` command compresses the existing context so it consumes fewer tokens without losing the substance of what has been built up — directly extending the usefulness of a long session. `Rename` supports better session hygiene by allowing meaningful naming conventions, making it easier to track and return to specific research threads.
- **When:** `Compact` is relevant in any long session where the context window is getting large and token efficiency matters. `Rename` is relevant at the start or end of any session that is worth preserving and returning to. `Clear` and `Rewind` are low-frequency — clear discards all gathered context which is rarely desirable in research work, and rewind restores an older state at the cost of losing everything that followed, making it useful only in specific recovery situations.
- **What:** For your role at EonLabs, `compact` and `rename` are the two commands with real day-to-day value. Long research sessions accumulate a lot of context — model assumptions, test results, hypothesis iterations — and being able to compress that without losing it means you can keep working productively without hitting token limits. Proper session naming also means you can manage multiple parallel research threads cleanly, which aligns with the multi-hypothesis approach Terry expects.

### Status, Logout & Usage Commands
- **Relevancy:** `2/9`
- **Why:** The status line displays useful information like the current model name and context percentage at the bottom of the interface. It can be customized or removed using natural language instructions. The logout command allows signing out of Claude Code when needed.
- **When:** Occasionally relevant when manually checking remaining usage or switching accounts. However, this is largely handled automatically by the CCMAX skill, which switches between available Claude Code accounts whenever a usage limit is hit — making manual status monitoring largely unnecessary.
- **What:** For your role at EonLabs, this section has minimal practical value. The infrastructure already in place through CCMAX abstracts away the need to manually track or manage usage limits. The logout command is a basic utility that is rarely needed in a research workflow. The low score reflects that this is operational housekeeping rather than anything that contributes to research quality or output.

### ccusage & API Key Setup
- **Relevancy:** `4/9`
- **Why:** The `ccusage` command provides visibility into how much Claude Code is being used and which conversations are consuming the most tokens. This is useful for determining whether the current subscription model is delivering value or whether a pay-per-use plan would be more efficient. The API key setup, however, is not relevant since EonLabs uses a subscription model via a Gmail account, making API configuration unnecessary.
- **When:** Relevant periodically when reviewing whether Claude Code usage is efficient and cost-effective. Particularly useful when sessions are getting expensive or when trying to identify which types of tasks are consuming disproportionate resources.
- **What:** For your role, `ccusage` is a lightweight but useful tool for operational awareness. As research sessions scale up in complexity — longer contexts, more agents, more parallel tasks — knowing which workflows are expensive helps prioritize where to invest effort in optimization. The API key portion of this section can be skipped entirely given the current subscription setup at EonLabs.

### Cost Command & Third-Party Providers
- **Relevancy:** `3/9`
- **Why:** The cost command shows token usage and associated costs, similar to ccusage. While useful for efficiency monitoring, this is largely handled at the organizational level at EonLabs, making it a low personal priority. Third-party provider configuration is only relevant if Claude Code needs to be set up on a remote virtual environment such as an EC2 instance on AWS, where Amazon Bedrock would need to be configured.
- **When:** The cost command becomes relevant only if there is a need to personally audit Claude Code efficiency. Third-party provider knowledge becomes relevant if and when EonLabs moves toward a remote or cloud-hosted Claude Code setup, at which point Bedrock configuration would become a necessary step.
- **What:** For your current role, neither of these is an immediate concern. Cost monitoring is managed at the organizational level, and the infrastructure is not yet at a point where remote cloud-based Claude Code configuration is required. This section is worth keeping in mind as a future reference rather than something actionable right now.

### API Keys: Bedrock, Foundry & Vertex AI
- **Relevancy:** `2/9`
- **Why:** This section covers how to configure Claude Code using third-party cloud providers — Amazon Bedrock, Foundry, and Vertex AI. This becomes relevant only if Claude Code needs to be set up on a remote server rather than a local machine. For the current setup at EonLabs, where Claude Code is installed locally and authorized via a subscription account through the CLI, this configuration is unnecessary.
- **When:** Only relevant if EonLabs moves to a remote server setup where Claude Code needs to be hosted and configured on cloud infrastructure. At that point, knowing how to connect Claude Code to Bedrock, Foundry, or Vertex AI would become a required step.
- **What:** For your current role, this section has minimal practical value. The local CLI setup with subscription-based authorization covers everything needed right now. This is best treated as a future reference for the scenario where remote cloud infrastructure becomes part of the workflow.

### btw, Voice & Export Commands
- **Relevancy:** `4/9`
- **Why:** The `btw` command is the most useful of the three — it allows you to send a quick aside or clarification to Claude Code while it is still working on a longer task, without interrupting the main workflow. This is genuinely useful in long research sessions where a follow-up thought or correction needs to be communicated mid-execution. The voice command is redundant given that Typeless is already being used for speech-to-text, and the export command has limited practical use unless there is a specific need to archive or share a conversation.
- **When:** `btw` is relevant any time Claude Code is running a time-consuming task and a quick clarification needs to be passed along without waiting for the task to complete. Voice and export commands are low-priority and unlikely to be needed in the current workflow.
- **What:** For your role at EonLabs, the focus is on curating ideas and directing research — not administrative overhead. The `btw` command supports that by keeping the research flow uninterrupted while still allowing real-time course corrections. Voice is already covered by Typeless, and exports are not a current need. The score reflects the value of `btw` specifically, with the other two commands contributing little to the research engineering workflow.

### Claude Code Projects & Scope
- **Relevancy:** `7/9`
- **Why:** Claude Code automatically creates a project within the `.claude/projects` directory whenever you open Claude in a project folder. The four levels of settings — managed, user, project, and local — give precise control over how Claude Code behaves across different contexts. Project-level settings are particularly valuable for enforcing shared conventions and compliance requirements across a team.
- **When:** Relevant from the moment you start working on any EonLabs repository. Setting up the correct project scope ensures that Claude Code behaves consistently and respects the conventions of that specific codebase. Project settings become especially important when multiple people are working on the same repository and need Claude Code to follow the same rules.
- **What:** For your role at EonLabs, project and local settings are the most directly useful. Project settings allow you to encode Terry's research principles — such as parameterless design, walk-forward validation requirements, and baseline-first thinking — directly into the Claude Code configuration for each repository. This means every session in that project starts with the right context and constraints already in place, reducing the need to re-explain conventions every time.

### Status Line & Session Data
- **Relevancy:** `6/9`
- **Why:** The status line provides a visual progress bar at the bottom of the Claude Code interface showing API usage, and can be customized to display information like the current model name in plain text. Session data goes deeper — it tracks cost details, durations, output styles, and workplace projects, and is stored as a JSONL file accessible via session ID and transcript path. This data is already being used in the EonLabs workflow, where session transcripts are processed through a Telegram Bot Watcher for monitoring purposes.
- **When:** Status line is relevant on an ongoing basis for quick visibility into usage during active sessions. Session data becomes particularly relevant when building monitoring tools or workflows that need to track prompts, requests, and outputs over time — and immediately relevant if you need to build something that processes or analyzes your own Claude Code activity.
- **What:** For your role at EonLabs, session data is more significant than it might initially appear. The JSONL transcript format means every session is a structured, queryable record of your research process — what was asked, what was produced, and how long it took. This is useful not just for organizational monitoring but also for your own reflection on whether your prompting and research approach is improving over time. If you ever build a tool that requires deep understanding of how Claude Code sessions are structured, this section provides the foundation for that.

### Settings & Permission Rules (Bash, MCP, WebFetch)
- **Relevancy:** `7/9`
- **Why:** Permission rules allow fine-grained control over what Claude Code can and cannot do — requiring explicit approval for bash commands, restricting WebFetch to authorized sites only, and selectively granting or denying access to specific MCP tools. For a research engineering role working directly on live EonLabs repositories, having guardrails against dangerous or irreversible actions is not optional — it is a necessary layer of protection.
- **When:** Relevant during the initial setup of any new project or repository. Specific rules — such as automatically denying any command that deletes directories — should be configured before Claude Code is given autonomous access to a codebase. WebFetch restrictions are relevant when Claude Code is being used to gather external research context and you want to ensure it only pulls from trusted sources.
- **What:** For your role at EonLabs, the most critical application is setting hard denial rules for destructive commands. Giving Claude Code broad autonomy over a production-adjacent research repository without permission guardrails is a meaningful risk. Configuring bash restrictions, controlled WebFetch access, and selective MCP tool permissions ensures that Claude Code operates as a disciplined research assistant rather than an unconstrained agent — which aligns directly with Terry's principle of using AI as leverage for insight, not as a substitute for judgment.

### Permission Modes & CLI/GUI Editing
- **Relevancy:** `7/9`
- **Why:** Permission modes determine how much autonomy Claude Code has during a session. The default mode prompts for permission on first use of each tool, while other modes like Accept Edit, Plan Mode, Don't Ask, and Bypass offer varying levels of automation. For a research engineering role where speed and flow matter, choosing the right mode for the right context is a meaningful productivity decision.
- **When:** Relevant at the start of every session, depending on the nature of the task. Plan Mode is useful when scoping out a new feature or hypothesis before any code is written. Bypass is useful during exploratory research sessions where constant approval prompts would break the flow. Default mode is appropriate when working in sensitive or production-adjacent repositories where caution is warranted.
- **What:** For your role at EonLabs, Bypass mode will likely be the go-to for day-to-day research work — it removes friction and keeps the session moving. However, this should be paired with the hard denial rules configured in the previous section, such as blocking directory deletion commands. Bypass without guardrails is dangerous; Bypass with well-defined permission rules is efficient and safe. That combination — maximum autonomy within clearly defined boundaries — is the right approach for research engineering work on live repositories.

### Sandboxing & Dangerous Scenarios
- **Relevancy:** `3/9`
- **Why:** Sandboxing restricts Claude Code from executing bash commands entirely, preventing any potentially dangerous operations like deleting directories. It is a hard boundary rather than a permission-based approach — useful in scenarios where the risk of destructive commands is high enough to warrant blocking bash access altogether.
- **When:** Only relevant in situations where an extremely cautious setup is required — for example, when onboarding Claude Code into a highly sensitive repository for the first time, or when delegating a task to a junior setup where full trust has not yet been established.
- **What:** For your role at EonLabs, sandboxing is too restrictive to be practical. Research engineering work requires Claude Code to run commands freely and fluidly — blocking bash access would cause legitimate commands to fail, breaking the workflow unnecessarily. The combination of Bypass mode with targeted hard denial rules from the previous section is a more appropriate and efficient approach than sandboxing. This section is good to know about, but unlikely to be used in practice.

### VIM Mode & Model Configuration
- **Relevancy:** `6/9`
- **Why:** VIM mode is only relevant for those already familiar with the VIM text editor — it replicates that editing experience within Claude Code. Model configuration, however, is directly relevant to every session. The `/model` command allows switching between Haiku, Sonnet, and Opus depending on the complexity and nature of the task, which has a real impact on both speed and quality of output.
- **When:** Model switching is relevant at the start of any session or mid-session when the task changes in nature. Haiku for lightweight, low-stakes tasks; Sonnet 4.5 for the majority of coding, planning, and research work; Opus for deep debugging, extensive research, or tasks requiring a large context window and high precision.
- **What:** For your role at EonLabs, model configuration is a meaningful lever. Sonnet 4.5 will cover most day-to-day research engineering tasks efficiently. Opus becomes the right choice when Terry's framework demands deep, precise work — for example, when stress-testing assumptions behind a trading model, designing a walk-forward validation framework, or debugging a complex feature in the Enigma system. Choosing the right model for the right task is itself a form of efficiency, and this section gives you the vocabulary and tools to make that choice deliberately. VIM mode can be ignored unless you already have a VIM background.

### Fast Mode & Image Reasoning
- **Relevancy:** `5/9`
- **Why:** Fast mode prioritizes speed over depth, which is not particularly useful for a research engineering role where the quality and precision of output matters more than response time. Image reasoning, however, is more relevant — it allows Claude Code to analyze visual inputs like UI mockups, charts, or diagrams and use that as context for implementation or analysis tasks.
- **When:** Fast mode is unlikely to be needed given the nature of the work. Image reasoning becomes relevant whenever visual data needs to be communicated to Claude Code — for example, sharing a chart of model performance, a diagram of a trading system architecture, or a screenshot of an interface that needs to be replicated or analyzed.
- **What:** For your role at EonLabs, image reasoning has practical value in scenarios where visual context adds clarity that text alone cannot provide. Research outputs often come in the form of charts, graphs, and visual summaries — being able to pass those directly to Claude Code and ask it to reason over them means you can work faster and more accurately without needing to manually transcribe visual information into text. Fast mode can be disregarded for this role.

### Effort Command & Headless Tasks
- **Relevancy:** `5/9`
- **Why:** The effort command allows control over how much computational thinking Claude Code applies to a task — low effort for lightweight tasks to minimize token usage, medium for tasks requiring high accuracy, and high effort when an initial response misses the intent and a deeper pass is needed. Headless mode allows Claude Code to be run without opening the TUI by passing a prompt directly via `claude -p`, which is useful for automation and scripting scenarios.
- **When:** Effort levels are relevant on a per-task basis throughout daily research work — defaulting to medium for most research tasks, dropping to low for administrative or simple tasks, and escalating to high when precision is critical or initial outputs are insufficient. Headless mode becomes relevant if and when Claude Code needs to be integrated into automated pipelines or scripts that run without a terminal interface.
- **What:** For your role at EonLabs, effort configuration is a useful but underutilized lever. Matching effort level to task complexity is a form of efficiency — not every task warrants maximum token usage, and being deliberate about this aligns with the goal of working efficiently. Headless mode is not currently needed since the TUI provides better visibility into intermediate steps, which is important for a research role where understanding the process is as valuable as the final output.

### Escaping Logic & Debug Mode
- **Relevancy:** `6/9`
- **Why:** The Escape key provides a quick way to interrupt Claude Code mid-execution when a process needs to be stopped before completion. Debug mode goes deeper — it outputs all debugging variables and information into a text file, then follows a structured process: describing the problem, reproducing it, and reading the debug log to identify warnings and errors. This is a systematic approach to troubleshooting features that are not working as expected.
- **When:** Escape is relevant any time Claude Code is running a task that needs to be halted — whether due to a wrong direction, an unexpected output, or a change in intent. Debug mode is relevant whenever a feature or workflow in a repository is broken and the cause is not immediately obvious from the output alone.
- **What:** For your role at EonLabs, debugging is an unavoidable part of the work. While AI assistance accelerates the coding process, the traditional principle still holds — a significant portion of research engineering time goes into diagnosing and fixing issues rather than writing new code. Debug mode gives you a structured, repeatable process for doing that efficiently. Combined with the Escape key for interrupting runaway processes, these tools are essential for maintaining control over complex, long-running research sessions.

### Dev Containers with Claude Code
- **Relevancy:** `2/9`
- **Why:** Dev containers allow Claude Code to be run inside a Docker container rather than directly on a local machine. This is useful when a specific, isolated environment is needed — for example, to avoid dependency conflicts or to replicate a production environment exactly. It is a more controlled and reproducible setup at the cost of additional configuration overhead.
- **When:** Only relevant if there is a future need to run Claude Code in an isolated containerized environment — for instance, if EonLabs moves toward a standardized development environment across the team, or if a specific research task requires a sandboxed setup that cannot be replicated locally.
- **What:** For your current role at EonLabs, this section is not applicable. Claude Code is already installed and running on your local machine, which is sufficient for the research engineering work at hand. Dev containers are a good concept to be aware of for future infrastructure decisions, but they add no immediate value to the current workflow.

### Common Workflow Follow Along
- **Relevancy:** `8/9`
- **Why:** This section demonstrates how to structure end-to-end workflows with Claude Code. While the workflow shown in the video is somewhat unstructured, it provides a useful reference point for developing a more disciplined personal workflow — one that aligns with both the research engineering role and Terry's principle of reaching the baseline quickly before going beyond it.
- **When:** Relevant every time a new task or feature is assigned. Having a repeatable, structured workflow means less time figuring out how to approach a problem and more time actually solving it. This is the section most directly applicable to the day-to-day work of monitoring repositories and adding new features.
- **What:** For your role at EonLabs, the video's workflow serves as a baseline to improve upon. The proposed workflow is more disciplined and research-appropriate: first instruct Claude to review the repository and understand the codebase, then switch to plan mode to architect the feature, review and adjust the plan, create a small spike to test the proposed solution, and finally verify whether it works for the specific use case. This approach mirrors Terry's framework — establish the baseline first, then test and validate before committing. It treats Claude Code as a structured research instrument rather than an ad-hoc coding assistant.

### Notification Hooks & Security Hooks
- **Relevancy:** `6/9`
- **Why:** Notification hooks allow you to receive alerts — including audible sounds — when a Claude Code task completes or fails, which is essential when running multiple parallel sessions. Security hooks act as a pre-execution filter, blocking sensitive information like API keys, 2FA recovery codes, and destructive commands from being accessed or run. Both hooks add a layer of oversight that becomes increasingly important as the complexity and autonomy of Claude Code sessions grows.
- **When:** Notification hooks are relevant any time multiple sessions are running in parallel — which, given the research engineering role at EonLabs, will be frequent. Security hooks are relevant from the moment Claude Code is given access to any repository containing sensitive information or when Bypass mode is active and manual approval prompts are turned off.
- **What:** For your role at EonLabs, both hooks serve practical purposes. Notification hooks free you from having to manually monitor every running session — you can focus on one task while others run in the background and get alerted when attention is needed. Security hooks provide a safety net when operating in Bypass mode, though it is worth noting their limitations — Claude Code may find workarounds if blocked from bash, which means hooks should be treated as one layer of protection rather than a complete guarantee. Used together with permission rules and deliberate model selection, they contribute to a safer and more monitored autonomous workflow.

---

## 3. Surfaces

### Claude Code Surfaces: Desktop & Web
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### Claude Chrome & Browser Extensions
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### VS Code & JetBrains IDE Integration
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### GitHub Actions & Remote Control
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### Computing Follow Along
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

---

## 4. Advanced

### Security Review & Output Styles
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### Simplify Command & Scheduling
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### Code Review & Agent SDK
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### Persistent Context: Claude.md & Rules
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### Claude Auto Memory & Troubleshooting
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### Agent Skills: Activation, Scripts & Dynamic Content
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### MCP with Claude Code & GG
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### MCP Doom & Playwright Integration
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

### Sub-agents & Multi-Agent Teams
- **Relevancy:** `/9`
- **Why:**
- **When:**
- **What:**

---

*Dictated and verified using Typeless voice-to-text. All justifications reflect my own perspective on relevancy to my role.*
