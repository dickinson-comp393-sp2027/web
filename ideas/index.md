# Ideas for course content

## Content from an existing online course

* Include some or all of Andrew Ng's [Agentic AI course](https://www.deeplearning.ai/courses/agentic-ai) at deeplearning.ai.
  * [list of course topics](ng-course-topics.md)

## Required readings and discussions

just a few ideas...

### technical concepts

* Hu, Shengran, Cong Lu, and Jeff Clune. "Automated design of agentic systems." International Conference on Learning Representations. 2025.
* Belcak, Peter, et al. "Small language models are the future of agentic ai." arXiv preprint arXiv:2506.02153 (2025).

### governance and safety

* Kasirzadeh, A., Gabriel, I. Agentic profiles for effective AI governance. Nature 656, 320–328 (2026). <https://doi.org/10.1038/s41586-026-10805-z>

* Bengio, Yoshua, et al. "Managing extreme AI risks amid rapid progress." Science 384.6698 (2024): 842-845.


## Possible assignments

### Present a research paper

* Students will select a research paper published at a recent AI conference and related to the course content. They present it to the class via poster and/or oral presentation.

### Final project

Conduct research on a question about agentic AI.

### Claude's suggestions

> I think two assignments is the right instinct, but I'd frame the split differently. "Single agent vs. multi-agent" is a weaker dividing line than "understand the machinery vs. apply it to something you care about." Multi-agent systems are often overused, and students tend to add agents because it sounds impressive rather than because the problem needs them.

> **Assignment 1: Build an agent from scratch.** Students write the core loop themselves against a raw model API, with no agent framework. That means defining tool schemas, parsing tool calls, dispatching them, feeding observations back, handling errors and stopping conditions, and managing the context window. It's maybe 150 to 300 lines of code, and it demystifies what frameworks like LangChain or the various agent SDKs hide. You can make it gradable by giving every student the same set of tasks (say, a few file-manipulation or research tasks in a sandbox) and checking whether their agent completes them.

> **Assignment 2 (optional but valuable): A controlled comparison.** Rather than "build a multi-agent system," have students take a task and test architectures against each other: single agent vs. planner/executor, with vs. without memory or reflection, one agent vs. several specialized ones. They have to build a small evaluation harness and report what actually helped. This is where a course at the undergraduate level can become more scientific than most agent tutorials, and it naturally teaches that multi-agent is a design choice with costs (latency, token spend, error propagation), not a goal.

> **Final project: the open-ended system in a topic they're passionate about.** Students can use frameworks here, and multi-agent is allowed but must be justified. Make evaluation and failure analysis a graded component. How do they know it works? What are three ways it broke? What did it cost per run? That keeps passion projects from being demos that only work on the happy path.

> A few things I'd build in throughout: sandboxing and permissions (agents that can run code or touch files are a good place to teach safety concretely), cost and token budgets, and a short reflection on where the agent should not be trusted to act autonomously.

> If the course is a full semester, this maps well to roughly 3 weeks on Assignment 1, 3 on Assignment 2, and the back half on the project with checkpoints. If time is tight, fold Assignment 2 into the project as a required comparison section.

> One question that would shape this: do students have a firm programming and API background going in, or will some need ramp-up on things like calling a model API and handling JSON? That determines how much scaffolding Assignment 1 needs.

