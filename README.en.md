<p align="center"><img src="assets/banner.svg" alt="Agent Beyond Hype" width="100%"></p>

# Agent Beyond Hype

**A user's manifesto for reliable AI work: question the labels, measure the outcomes, and explore designs beyond human imitation.**

[中文首页](README.md) · [Full essay, Chinese](docs/manifesto.zh-CN.md) · [Task contract](templates/task-contract.md) · [Experiment template](templates/experiment-report.md) · [Issues](https://github.com/OolongMint/agent-beyond-hype/issues)

> I don't need another name for an agent. I need the same job done faster, cheaper, and more accurately.

This repository turns personal notes into an argument and a small set of reusable Markdown templates. It contains **proposals, not published benchmark results**. Counterexamples are welcome.

## The argument in a minute

| Claim | Practical consequence |
| --- | --- |
| A new label does not establish a new capability | Ask for mechanisms, baselines, costs, and failure cases |
| A capable model is a starting point | Design its tools, context, execution, validation, and recovery |
| Context should be relevant and current | Retrieve as needed and preserve recoverable task state |
| Completion needs evidence | Inspect artifacts against acceptance criteria |
| Token savings are only part of efficiency | Include failed attempts, tool fees, and human rework |
| Human resemblance is an optional design choice | Compare workflows by observable outcomes |

## Start with a task contract

Copy [this template](templates/task-contract.md). It is bilingual and works as a standalone brief.

```text
Goal: What must be delivered?
Inputs: Which sources are authoritative and current?
Authority: What may the system read, change, or publish?
Budget: What are the cost, time, and retry limits?
Acceptance: What evidence establishes success, and who checks it?
Recovery: How does work resume without duplicating actions?
```

Start with the simplest viable approach. Add one tool, skill, or reviewer only when it addresses an observed limitation. Compare both approaches on the same tasks under the same acceptance rules.

The [worked release-notes example](examples/release-notes.md) shows how to define inputs, an output contract, failure cases, and an evaluation plan. It contains no claimed execution results.

## What I mean by a harness

A harness is the runtime system surrounding a model: it supplies context and tools, controls execution, tracks state, enforces limits, and helps establish whether the task is complete. This is a working definition, not a universal taxonomy.

Prompt engineering expresses instructions. Context engineering selects and maintains the information available at a given step. Harness engineering also needs executable mechanisms for state, permissions, retries, validation, and recovery. These areas overlap, but a prompt asking for a budget limit does not itself enforce that limit.

A personal agent is an application direction; a harness is supporting infrastructure. They are not synonyms.

## Skepticism that can survive a counterexample

I am skeptical when familiar pieces—memory, skills, scheduling, tools—are presented as a fundamental breakthrough merely because they have been packaged under a new name.

But integration has real value. Reliable permissions, stable connectors, recovery, and maintenance can make an otherwise unusable system useful. Reused components do not prove that a product is worthless. Nor do they establish a company's fundraising motives.

My test is simple: what mechanism changed, what improved against a baseline, at what cost, and what happens if we remove it?

## Context and reviewers: useful, conditional tools

More context can supply necessary evidence, but irrelevant or stale material can interfere with the task. Shorter is not automatically better either. Compaction and reset with an explicit handoff are alternative strategies whose suitability depends on task continuity and information loss. Neither guarantees correct recovery.

Separating execution from review can improve scrutiny, but two agents can share the same blind spots. Reviewers need access to evidence and clear criteria. Prefer deterministic checks where the problem supports them; compare additional agents against their coordination cost.

Anthropic's [Building effective agents](https://www.anthropic.com/research/building-effective-agents) distinguishes predefined workflows from model-directed agents. Its [context engineering article](https://www.anthropic.com/research/effective-context-engineering-for-ai-agents) discusses managing the information available to a model. These sources inform the questions above; they do not validate every proposal in this repository.

## Measure accepted work

```text
Cost per accepted delivery = total cost of all attempts / accepted deliveries
Total cost = model calls + tools and infrastructure + human review and rework
```

Include failed attempts in the numerator. With zero accepted deliveries, this metric has no finite valid value. Declare how human time is valued and report maintenance cost separately when relevant.

Also report acceptance rate, end-to-end latency, human intervention, and failure categories. Do not hide an unacceptable failure behind a single composite score.

OpenAI's [agent improvement loop example](https://developers.openai.com/cookbook/examples/agents_sdk/agent_improvement_loop) connects traces and feedback to evaluations and subsequent system changes. This repository proposes using that general feedback discipline for small, task-specific experiments.

## Beyond human imitation

Sensors as senses, tools as limbs, and an LLM as a brain are useful introductory metaphors. They are not architectural requirements or evidence that models think like people. Autonomy is a system property, and agents need not use LLMs at all.

Rather than reproduce a human organization, we can compare structured state, direct APIs, batch candidate search, and executable checks against conversational handoffs and role-based coordination. Those alternatives may fail too; they are hypotheses to test.

The aim is to loosen assumptions about the execution path while retaining human-defined goals, authority, and accountability. More training data does not by itself establish general intelligence, and useful agent work does not require solving AGI first.

## Contents and contributions

- [Chinese essay](docs/manifesto.zh-CN.md): the complete argument, limitations, and research questions.
- [Chinese playbook](docs/playbook.zh-CN.md): a practical improvement workflow.
- Bilingual templates: [task contract](templates/task-contract.md), [context handoff](templates/context-handoff.md), [acceptance review](templates/acceptance-review.md), and [experiment report](templates/experiment-report.md).
- [Sources and claim calibration](docs/sources-and-claims.md): distinguishes references, opinions, and untested proposals.
- [Contributing](CONTRIBUTING.md): submit reproducible experiments, failures, or reasoned objections in either language.

If a template saves you a round of rework, star the repository to find it again. More valuable still: share a failure that changes the argument.

Written from the original ideas of [OolongMint](https://github.com/OolongMint), with AI assistance for editing, translation, and source checking. Text and templates: [CC BY 4.0](LICENSE). First edition: 2026-10-25.
