<div align="center">

# Ramkumar Muraleedharan

**Senior AI / ML Engineer**  ·  New York, NY

*I make non-deterministic systems behave.*

![Multi-Agent](https://img.shields.io/badge/Multi--Agent_Orchestration-1F3A5F?style=flat-square)
![Reliable LLMs](https://img.shields.io/badge/Reliable_LLM_Output-1F3A5F?style=flat-square)
![Edge Inference](https://img.shields.io/badge/Edge_Inference-1F3A5F?style=flat-square)
![Production ML](https://img.shields.io/badge/Production_Reliability-1F3A5F?style=flat-square)

</div>

---

Most of my work starts after the demo breaks. It's easy to build an agent that reasons fine in a clean test suite and falls apart the moment it hits real, messy input. The interesting engineering is everything after that: the guardrails, the validation, the retries, and the edge-hardware constraints that decide whether a system actually holds up in production. That's the part I'm good at.

I've shipped this across regulated legal-tech, clean-energy edge devices, and large-scale matching systems - anywhere a bad architectural call has immediate, real-world consequences.

### How I think about building with AI

> **If it can be done with an `if`-`else`, it shouldn't be an LLM call.**

- A system that works in the demo and breaks on real data isn't done - it's halfway done.
- Non-deterministic models need deterministic guardrails around them. Validation, abstention, and bounded retries aren't extras; they're the product.
- Use models where they genuinely fit, and classical ML where they don't. An LLM is a poor time-series forecaster and a great reasoner - knowing the difference is most of the job.
- Reliability is a feature you design in, not a bug you patch later.

---

### Featured work

**[dspyer](https://github.com/theramkm/dspyer)** · *Python · Apache-2.0 · [PyPI](https://pypi.org/project/dspyer/)*
Reliable, optimizable LLM steps for DSPy and LangGraph. Wrap a model call in a Pydantic schema and it self-corrects against its own validation errors until the output conforms. Each step compiles to a standard DSPy module, so prompts are tuned from data with an optimizer instead of edited by hand. Drops into an existing LangGraph without a rewrite.

**[ENDGAME](https://github.com/theramkm/ENDGAME)** · *seq2seq · PyTorch · 2021*
A sequence-to-sequence model that generates Python from natural-language descriptions, with custom-trained code embeddings - built before LLM code assistants existed, back when training your own was the only way to do it.

---

### What I work on

- **Multi-agent orchestration** - LangGraph and DSPy state machines that survive real traffic
- **Reliable LLM output** - schema validation, self-correction, grammar-constrained decoding
- **Edge inference** - llama.cpp, 4-bit quantization, latency from seconds to milliseconds
- **Production ML** - the telemetry, guardrails, and MLOps that keep non-deterministic systems honest

### Tools I reach for most

`LangGraph` · `DSPy` · `llama.cpp` · `PyTorch` · `FastAPI` · `Pinecone` · `Dagster` · `Docker` · `AWS`

---

<div align="center">

**Let's talk** - [LinkedIn](https://www.linkedin.com/in/ramkumar-m/) · theram.km@gmail.com

</div>
