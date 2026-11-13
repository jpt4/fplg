These are the architectonic rules of our endeavor.

Project Generic:

Section 1:

The following applies to all aspects of a project, whether related to software, hardware, research, idle speculation, or otherwise:

1.1 In all things, adhere to the user's intent, and advance the project's objectives. Abhor and avoid all unnecessary ceremony, scaffolding, and performative preparatory behaviors that do not achieve actual progress. Language must be direct and informative, never witholding, obscuring, or deferring details. A relentless pursuit of truth, of effectiveness, of function, independent of form, is your highest motivation.

1.2 Ask questions freely, where clarification is needed, but do not ask for a second opinion merely out of caution - if you have made the right decision, be confident in its correctness, and carry it out.

1.3 All project artifacts shall be added to the version control record, following a fine-grained commit discipline: every logical unit of work is commited, in small enough units that each commit is easily reviewable individually. Commit messages shall describe the changes made, without superfluous detail. All local commits shall be pushed to remote mirrors unless explicitly instructed otherwise, or in connectivity-denied circumstances.

1.4 Maintain documentation layers by purpose. Use `LOG.md` ("the Log") as the inclusive chronological spine for development: record dated process notes, exploration, dead ends, backtracks, scratchpad observations, and links to specialized records. When a log entry captures a conversation or design note that will be used immediately, place the longer note under `docs/log/` and link to it from `LOG.md`. Use `MEMORY.md` only for high-priority facts that should remain present in future working context. Use `LESSONS.md` for durable lessons learned during the project. Use README files for current public entrypoints and navigational summaries rather than as the primary historical trace.

1.5 Architecture Decision Records must precede all feature implementation - these document the motivations, decision points, and success/failure criteria for each feature, and the project design document should map to a sequence of ADRs. After each ADR is complete, it is to receive an After Action Report as to its effect on the project, and these are to be revisited as new information becomes available (for example, if a feature requires collecting data for an extended period of time to determine its usefulness, the AAR will be updated after sufficient data is available and assessed). Not all project steps are ADRs - for example, a sequence of ideation or pedagogical conversations, or writing a report after conducting research to answer a question, may not need to be surrounded by an ADR and AAR. However, all project artifacts and activity must be recorded in the Log and other documentation as appropriate, regardless of whether they do or not follow the ADR framework.

1.6 When multiple independent tasks can be pursued concurrently on separate branches or worktrees, with no cross-branch dependency, propose launching sub-agents for user review; recommend sub-agent models and reasoning levels appropriate to the task at hand. If approved, give each sub-agent a distinct branch or worktree, a bounded scope, explicit success and failure criteria, and instructions to commit completed logical units locally and report results before any merge or push.

Section 2:

The following describe certain mandatory software development practices, to enshrine well-skilled methodologies:

2.1 Follow strict red-green Test Driven Design - tests must precede code, and tests must provide feedback both when code is absent (tests must fail), and present (tests must pass). Tests must be non-trivial, exercising intended functionality and properties, not merely structure, naming, or other superficial, easily satisfied aspects.

2.2 Test coverage must be total, and if not, documented as such, with sufficient rationale to excuse total coverage of all code paths. 

2.3 Comment all code thoroughly, sufficient that the codebase might be transferred to another developer who, though competent, is entirely unfamiliar with the software, its rationale, and its history.

2.4 Branch discipline should generally follow the ADR structure of the implementation roadmap, with a new branch for each ADR, merged into master once the feature is complete, or development otherwise halted. If a branch cannot be merged in total, valuable elements should be selectively merged, so that 

2.5 Commit only those files one specifically has intentionally modified, and push after every logical unit of work is complete (which implies a passing, regression free test suite evaluation).

2.6 Do not regress code, or change unrelated elements, aspects, or the structure of the codebase, in the pursuit of a given objective. All changes must be intentional, and bound to a specific, articulable, recorded goal, that advances and improves the project at hand. Reverting to previous commits is preferable to commenting out or stubbing out code, if a feature needs to be rolled back or removed for reasons of testing, refactoring, or changes in design decisions.

2.7 Eagerly and assiduously seek out tasks and complete them; do not stop or defer work for later. Initiative and good judgement is preferred over inaction; using the above branch and commit discipline, any work completed too early can be reverted.

2.8 Review these practices reguarly, to keep them in context.

Project Specific:

[To be added as needed.]
