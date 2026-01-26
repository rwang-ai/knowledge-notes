Learning in Public Series #12
When MCP Made Claude Code Handy

MCP seems like an old concept, but I want to share two MCPs that make Claude Code truly handy: Sentry and GitHub.
- Sentry MCP: I use it to parse stack traces and mountains of logs. Claude Code links Sentry context to your codebase, producing coherent explanations and relevant concepts. Your judgment still matters, but hypothesis generation becomes much faster. Using MCP connected to production logs with the codebase to conduct RCA is a quite effective pattern. I remember earlier days at LinkedIn, debugging distributed graph production often took me a week of staring at logs and dashboards—AI now compresses that process into minutes.
- GitHub MCP: Reviewing unfamiliar codebases with minimal context used to burn a lot of mental energy. Not everyone provides the same level of useful context in PRs, which makes effective review even harder. Now, I give Claude a PR link and get the prerequisite context I need to review effectively. When I’m working in a language I’m less familiar with, it helps me learn the language in place while reviewing, and I can also double-check design patterns and architectural choices—reducing cognitive load and speeding comprehension.

What Actually Improved

Using MCP with Claude Code changed how each work item feels:
- Less time reconstructing context from dashboards, logs, and repos
- Less cognitive overhead switching between systems
- Each task becomes a mini learning drill—understanding a system, a language, or a design choice in context
I’m not just moving faster; I’m learning while doing.

The Takeaway
We often say context is everything—and it goes both ways.
LLMs do better work when they’re given better context. Humans also do better work when they use LLMs to assemble better context. MCP sits right in the middle of that loop, making both sides stronger.