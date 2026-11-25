# Awesome-Model-Evaluation-LLM-Benchmarking

## Top Model Evaluation & LLM Benchmarking Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on LLM App Evals, RAG Metrics, Agent Testing, Academic Benchmarks & Model Selection*  
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Model Evaluation & LLM Benchmarking**. These tools measure quality, safety, and regression risk for foundation models and LLM applications—from offline test suites to production trace scoring.

**Examples** include LangSmith, Braintrust, DeepEval, Ragas, Arize Phoenix, Galileo, Humanloop, TruLens, Patronus AI, Fiddler AI, and community tooling such as **whichllm** (`Andyyyy64/whichllm`).

**Open-source emphasis**: Evaluation is one of the richest open areas in LLMOps. **DeepEval**, **Ragas**, **promptfoo**, **TruLens**, **Phoenix**, **lm-evaluation-harness**, **Inspect AI**, and **Langfuse** cover app tests, RAG metrics, and model benchmarks. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[LangSmith, Braintrust, Humanloop, Galileo](https://www.langchain.com/langsmith)**  
  Managed evaluation and observability platforms—datasets, LLM-as-judge, experiment tracking, and production monitoring for LLM apps.

- **[Arize, Fiddler AI, Patronus AI](https://arize.com/)**  
  Enterprise AI observability and evaluation—tracing, drift, safety, and continuous eval on live traffic.

- **[Confident AI (DeepEval Cloud) and related app-eval SaaS](https://www.confident-ai.com/)**  
  Hosted layers on top of open eval frameworks for team dashboards and CI reporting.

- **[Other commercial LLM evaluation platforms](https://www.patronus.ai/)**  
  Additional red-teaming, guardrail, and model-quality products.

## Open-Source GitHub Projects

### LLM Application & RAG Evaluation

- **[DeepEval](https://github.com/confident-ai/deepeval)**  
  Open pytest-style framework for LLM apps and agents—50+ metrics including faithfulness, contextual recall, tool correctness, and multi-turn checks (Apache-2.0).

- **[Ragas](https://github.com/explodinggradients/ragas)**  
  Open RAG evaluation library—context precision/recall, faithfulness, answer relevance, and synthetic test-set generation.

- **[TruLens](https://github.com/truera/trulens)**  
  Open evaluation and tracing library (Snowflake)—feedback functions for groundedness, relevance, and custom scores on instrumented apps (MIT).

- **[promptfoo](https://github.com/promptfoo/promptfoo)**  
  Open config-driven prompt and model testing—assertions, LLM-as-judge, red teaming, and CI-friendly failure gates (MIT).

- **[OpenAI Evals](https://github.com/openai/evals)**  
  Open evaluation framework and registry—templates for building and sharing model/app evals.

### Observability + Evaluation Platforms

- **[Arize Phoenix](https://github.com/Arize-ai/phoenix)**  
  Open LLM observability and evaluation—tracing, datasets, and evals you can self-host (note Elastic License 2.0 restrictions on offering it as a managed service).

- **[Langfuse](https://github.com/langfuse/langfuse)**  
  Open LLM engineering platform—traces, scores, datasets, and prompt management; strong self-host path.

- **[Opik (Comet)](https://github.com/comet-ml/opik)**  
  Open LLM evaluation and observability toolkit for tracing and scoring application runs.

### Model Benchmarks & Harnesses

- **[lm-evaluation-harness (EleutherAI)](https://github.com/EleutherAI/lm-evaluation-harness)**  
  Standard open harness for academic and open-weight model benchmarks—dozens of tasks and multiple inference backends.

- **[Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai)**  
  Open framework for rigorous LLM and agent evaluations—sandboxed runs and research-grade task definitions (MIT).

- **[HELM (Stanford)](https://github.com/stanford-crfm/helm)**  
  Open holistic evaluation of language models—multi-metric, scenario-based reporting.

- **[lighteval (Hugging Face)](https://github.com/huggingface/lighteval)**  
  Open evaluation toolkit integrated with the Hugging Face ecosystem.

### Hardware-Aware & Selection Tools

- **[whichllm](https://github.com/Andyyyy64/whichllm)**  
  Open tool to find local LLMs that actually run and perform on *your* hardware—recency-aware benchmarks and engine detection, not just parameter count.

### Additional Strong Open-Source Options

- **Pytest-style app/agent tests**: DeepEval.
- **RAG-focused metrics**: Ragas.
- **CI prompt regression + red team**: promptfoo.
- **Trace + feedback functions**: TruLens or Phoenix.
- **Self-hosted eval platform**: Langfuse or Phoenix.
- **Base-model academic benchmarks**: lm-evaluation-harness, HELM, or Inspect AI.
- **Local model pick by real hardware**: whichllm.
- **Composable stacks**: promptfoo/DeepEval in CI → Ragas for RAG quality → Phoenix/Langfuse for production traces → harness for model swaps.
- Commercial platforms still lead for team UX, compliance workflows, and managed judge infrastructure.

**Frameworks for building custom systems**:  
**DeepEval** or **promptfoo** for automated app tests; **Ragas** for retrieval quality; **TruLens**/**Phoenix**/**Langfuse** for traced evals; **lm-evaluation-harness** when comparing base models; **whichllm** when choosing local runtimes.  
Fully open evaluation stacks are production-ready for startups through research labs.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS/hosted or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- LLM-as-judge metrics can be biased and unstable—calibrate against human labels on your domain. Benchmarks leak and saturate; prefer task-specific evals for product decisions. Some licenses (e.g. Elastic License 2.0) restrict offering the software as a hosted service.
- Open-source tools offer transparency and offline control. Managed platforms shift storage, collaboration, and support to the vendor. Neither replaces clear success criteria and continuous monitoring in production.

---

**Made for LLM engineers, applied researchers, and teams who refuse to ship on vibes alone.**  
Let's expand open model evaluation and benchmarking while recognizing the workflow depth that leading commercial LLMOps platforms deliver.
