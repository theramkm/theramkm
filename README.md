<div align="center">

# Ramkumar Muraleedharan

**Senior AI/ML engineer in New York. I build LLM and ML systems that hold up in production: multi-agent workflows, evaluation pipelines, structured-output constraints, and low-latency inference on CPU-only edge hardware.**  

*I make non-deterministic systems behave.*

![Multi-Agent](https://img.shields.io/badge/Multi--Agent_Orchestration-1F3A5F?style=flat-square)
![Reliable LLMs](https://img.shields.io/badge/Reliable_LLM_Output-1F3A5F?style=flat-square)
![Edge Inference](https://img.shields.io/badge/Edge_Inference-1F3A5F?style=flat-square)
![Production Reliability](https://img.shields.io/badge/Production_Reliability-1F3A5F?style=flat-square)

</div>



---

### **Most of my work starts after the demo breaks.**

It's easy to build an agent that reasons fine in a clean test suite and falls apart the moment it hits real, messy input. The interesting engineering is everything after that: the guardrails, the validation, the retries, and the edge-hardware constraints that decide whether a system actually holds up in production. That's the part I care about.

I've shipped this across regulated legal-tech, clean-energy edge devices, and large-scale matching systems, anywhere a bad architectural call has immediate, real-world consequences.

---

### How I think about building with AI

> **If it can be done with an `if`-`else`, it shouldn't be an LLM call.**

- **A demo that breaks on real data isn't done.** It's halfway done.
- **Non-deterministic models need deterministic guardrails.** Validation, abstention, and bounded retries aren't extras; they're the product.
- **Use models where they fit, classical ML where they don't.** An LLM is a poor time-series forecaster and a great reasoner. Knowing the difference is most of the job.
- **Reliability is designed in, not patched on.**

### Selected results

- Cut edge-gateway inference latency **~90%** (≈5s to under 500ms) on CPU-only hardware by replacing cloud APIs with 4-bit quantized local models via llama.cpp.
- Raised legal-clause retrieval accuracy **40%** over a golden-dataset baseline with hybrid search and parent-child document indexing.
- Forced **100% schema-valid** model output under live load using grammar-constrained decoding (GBNF), eliminating command-parsing failures.

---

## Projects
 
**[traceval](https://github.com/theramkm/traceval)** · `pip install traceval` · MIT
 
Turns agent trace exports (OpenTelemetry GenAI, Langfuse, LangSmith) into runnable pytest eval suites. Clusters failures, generates golden and regression cases, compares runs, gates CI with exit codes, and calibrates LLM judges against blind human labels. Offline, deterministic, no platform account.
 
**[dspyer](https://github.com/theramkm/dspyer)** · `pip install dspyer` · GPL2
 
Validated, self-correcting LLM steps for DSPy and LangGraph. Wraps model calls in Pydantic schemas, feeds validation errors back until output conforms, and compiles to DSPy modules so prompts can be tuned from data.
 
**[ENDGAME](https://github.com/theramkm/endgame)** · PyTorch · 2021
 
Natural-language-to-Python code generation, built before LLM code assistants existed. Seq2seq model trained on a hand-built 4,600-pair dataset with whitespace-aware tokenization; the README documents the experiments that failed (custom code embeddings) as carefully as the ones that worked.
 

 

### What I work on

| | |
|---|---|
| **Multi-agent orchestration** | LangGraph and DSPy state machines that survive real traffic |
| **Reliable LLM output** | Schema validation, self-correction, grammar-constrained decoding |
| **Edge inference** | llama.cpp, 4-bit quantization, latency from seconds to milliseconds |
| **Production reliability** | The telemetry, guardrails, and MLOps that keep non-deterministic systems honest |

### Tools I reach for most

`LangGraph` · `DSPy` · `llama.cpp` · `PyTorch` · `FastAPI` · `Pinecone` · `Dagster` · `Docker` · `AWS`

---

<div align="center">

**Let's talk:** &nbsp; [LinkedIn](https://www.linkedin.com/in/ramkumar-m/) &nbsp;·&nbsp; theram.km@gmail.com

</div>
