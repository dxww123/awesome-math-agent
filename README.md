# Awesome Math Agents

A curated list of AI agents, agent workflows, and supporting tools for mathematical research, problem solving, proof review, formalization, and theorem proving.

**Scope.** Entries should do mathematical work through an agent loop, tool use, proof search, or coordinated generation and verification. A few closely related tool servers and research baselines are included because they are useful when building math agents. A project that reviews a proof in natural language does **not** necessarily produce a machine-checked proof; consult its documentation for its actual guarantees.

Projects are grouped by their primary use; some span multiple categories.

## Contents

- [Mathematical research and natural-language proof](#mathematical-research-and-natural-language-proof)
- [Formal proving and verification](#formal-proving-and-verification)
- [Olympiad and mathematical modeling](#olympiad-and-mathematical-modeling)
- [Agent skills, plugins, and tools](#agent-skills-plugins-and-tools)
- [FirstProof submissions and research baselines](#firstproof-submissions-and-research-baselines)
- [Hosted services](#hosted-services)
- [Historical and unavailable projects](#historical-and-unavailable-projects)
- [Contributing](#contributing)

## Mathematical research and natural-language proof

- [QED](https://github.com/proofQED/QED) — Open-source multi-agent system for generating mathematical proofs of open problems.
- [AIM](https://github.com/TheoryFoundry/AIM) — Rust-based AI Mathematician for exploratory, self-verifying research-level problem solving; formerly hosted at [Carlos-Mero/AIM](https://github.com/Carlos-Mero/AIM).
- [AIMv2](https://github.com/TheoryFoundry/AIMv2) — CLI math research assistant with theorem-graph memory, multipass review, and resumable work.
- [Rethlas](https://github.com/frenzymath/Rethlas) — Worker-and-verifier system for research-level mathematical proof search.
- [Rethlas, yexf308 fork](https://github.com/yexf308/Rethlas) — Fork with expanded Codex orchestration, verification records, and a proof-and-repair loop.
- [Danus](https://github.com/frenzymath/Danus) — Multi-agent mathematical reasoning organized around a verifier-gated fact graph.
- [Vibefeld](https://github.com/tobiasosborne/vibefeld) — Agent-first framework for adversarial construction and review of structured natural-language proofs.
- [coverify](https://github.com/chaoxu/coverify) — Adversarial natural-language proof workflow with independent auditing and reconstruction; results are [not machine checked](https://github.com/chaoxu/coverify#readme).
- [xean](https://github.com/chaoxu/xean) — Durable mathematical exploration and verification solver with restartable campaigns and an audit-oriented kernel.
- [vibe-proving-math](https://github.com/ml1301215/vibe-proving-math) — Research assistant for proof generation and review, theorem retrieval, and citation checks.
- [research-math-assistant](https://github.com/ml1301215/research-math-assistant) — Local solve–verify–revise research assistant with literature lookup, a web UI, and LaTeX output.
- [bourbaki](https://github.com/0bserver07/bourbaki) — Tool-using math assistant integrating SymPy, Lean 4, OEIS, and arXiv.
- [co-mathematician](https://github.com/VeryMath/co-mathematician) — Persistent research workbench connecting sources, notes, model conversations, computation, proofs, and review.
- [AxiomRelay](https://github.com/ot-triton-lab/AxiomRelay) — Proof hill-climbing system that separates search, synthesis, and independent verification.
- [Moonshine](https://github.com/DeepMathLLM/Moonshine) — Autonomous mathematical research agent for conjecture generation and persistent exploration.
- [Math-Research-Agent](https://github.com/Shengrong-Wu/Math-Research-Agent) — Depth-first mathematical proof agent with persistent memory and optional Lean verification.
- [Math-Research-Agent-v2](https://github.com/Shengrong-Wu/Math-Research-Agent-v2) — Umbrella project for natural-language and Lean-first proof workflows.
- [math-explorer-agent](https://github.com/xyzmtx/math-explorer-agent) — LLM-based mathematical exploration agent.
- [ResearchMathAgent](https://github.com/sjtuytc/ResearchMathAgent) — Multi-agent research-level math prover with structured memory and iterative verifier feedback.
- [OpenTorus](https://github.com/maximilianbehr/OpenTorus) — Open-problem research agent with literature search, proof and refutation branches, gap tracking, and evidence records.
- [TeXRA](https://github.com/LionSR/TeXRA) — AI theorist with mathematician agents for open problems, proofs, and Lean formalization.
- [proof-council](https://github.com/eth-sri/proof-council) — Autonomous math research workflow developed around FirstProof-style problems and human review.
- [tcs-prover](https://github.com/yonggangjiang/tcs-prover) — Agentic proof search for theoretical computer science with statement review and independent criticism.
- [STAR-PolyaMath](https://github.com/Julius-Woo/STAR-PolyaMath) — Multi-agent mathematical reasoning under persistent strategy supervision.

## Formal proving and verification

- [openproof](https://github.com/mxthematic/openproof) — Conversational Lean 4 theorem prover combining agentic proof repair with tactic search; Lean checks accepted proofs.
- [ulamai](https://github.com/ulamai/ulamai) — Lean 4 proving and formalization CLI with LLM guidance, premise retrieval, search, and Lean checking.
- [LeanAgent](https://github.com/lean-dojo/LeanAgent) — Lifelong-learning framework for Lean theorem proving across expanding mathematical knowledge.
- [Prover-Agent](https://github.com/kAIto47802/Prover-Agent) — Lean theorem prover combining informal reasoning, formal proof models, auxiliary lemmas, and compiler feedback.
- [ml-hilbert](https://github.com/Rose-STL-Lab/ml-hilbert) — Fork of [Apple's ML-Hilbert](https://github.com/apple-aiml-research/ml-hilbert), which recursively builds formal Lean proofs from informal reasoning.
- [lean4_verification_pipeline](https://github.com/LogicEnj/lean4_verification_pipeline) — Model-backed pipeline for generating Lean formal proofs and verifying mathematical solutions.
- [goedels-poetry](https://github.com/KellyJDavis/goedels-poetry) — Multi-agent theorem prover that formalizes statements and generates Lean 4-verified proofs.
- [MechMath-v1](https://github.com/MechMath/MechMath-v1) — Lean 4 proving workflow that repairs failed attempts and recursively decomposes remaining goals.
- [numina-lean-agent](https://github.com/project-numina/numina-lean-agent) — Claude Code-based formal theorem-proving agent with Lean tools and search.
- [copra](https://github.com/trishullab/copra) — In-context proof agent for formal theorem proving in Lean, Isabelle, and Coq.
- [APOLLO](https://github.com/aziksh-ospanov/APOLLO) — Agentic Lean 4 proof repair driven by compiler feedback.
- [HERMES](https://github.com/aziksh-ospanov/HERMES) — Stepwise natural-language proof verifier that autoformalizes claims into Lean 4.
- [lean-prover](https://github.com/Lean-Prover/lean-prover) — Autonomous Lean proof agent using an LLM draft, compile, and repair loop.
- [LEAN-formalization-loop](https://github.com/hregahego/LEAN-formalization-loop) — Multi-agent plan, work, and review loop for formalizing detailed proof sketches in Lean 4.
- [MerLean](https://github.com/MerLeanProver/MerLean) — Mathematics agents for proof exploration, Lean formalization, and paper writing.
- [Archon](https://github.com/frenzymath/Archon) — AI-assisted Lean project automation with dependency-graph blueprints and multi-agent proving.
- [Archon-Horizon](https://github.com/frenzymath/Archon-Horizon) — Long-horizon successor coordinating Lean formalization across interdependent projects.
- [LeanMarathon](https://github.com/YuanheZ/LeanMarathon) — Blueprint-based, long-horizon Lean 4 autoformalization with parallel Codex agents.
- [OpenGauss](https://github.com/math-inc/OpenGauss) — Project-scoped multi-agent Lean workflow orchestrator built around `lean4-skills`.

## Olympiad and mathematical modeling

- [IMO25](https://github.com/lyang36/IMO25) — Multi-provider AI agent system and parallel runner for IMO 2025 problem solving.
- [Vibe-Mathematics](https://github.com/ChongCyrus/Vibe-Mathematics) — DeepSeek Harness presets for collaborative math solving and formal verification.
- [dsh-math-olympiad](https://github.com/988hj7tczd-oss/dsh-math-olympiad) — DeepSeek Harness skills for Olympiad mathematics with adversarial verification.
- [dsh-ultramath](https://github.com/Andiii208/dsh-ultramath) — DeepSeek Harness multi-agent mathematical modeling plugin.
- [dsh-math-team](https://github.com/OrinVoss/dsh-math-team) — DeepSeek Harness mathematical modeling agent presets.
- [MathModelAgent](https://github.com/jihe520/MathModelAgent) — Mathematical modeling agent and skill collection.

## Agent skills, plugins, and tools

- [dsh-alphasolve](https://github.com/dxww123/dsh-alphasolve) — DeepSeek Harness plugin for AlphaSolve-style solve, check, and revise workflows.
- [dsh-danus](https://github.com/Fisfzy/dsh-danus) — DeepSeek Harness adaptation of Danus with verifier-gated, multi-agent proof search.
- [qmd-prover](https://github.com/powergiant/qmd-prover) — Quarto Markdown proof workspace with a semantic dependency graph and configurable agent verification.
- [jacobian](https://github.com/morluto/jacobian) — MCP server offering searchable, typed mathematical operations to AI agents.
- [lean4-skills](https://github.com/cameronfreer/lean4-skills) — Lean 4 proof and autoformalization workflows for coding agents, including autonomous modes.
- [dsh-math-proof](https://github.com/clearnature/dsh-math-proof) — DeepSeek Harness proof preset with Agda-kernel checking.
- [math-research-dsh](https://github.com/xsoc1/math-research-dsh) — DeepSeek Harness adaptation of mathematical research skills.
- [dsh-frontier-math](https://github.com/inoricon1/dsh-frontier-math) — Evidence-gated DeepSeek Harness workflow for frontier mathematics.

## FirstProof submissions and research baselines

- [UCLA FirstProof Batch 2 submission](https://github.com/1stproof/batch-2/tree/main/batch-2-submissions/ucla) — Parallel solution generation, literature research, and verification components.
- [Princeton FirstProof Batch 2 submission](https://github.com/1stproof/batch-2/tree/main/batch-2-submissions/princeton) — Multi-agent research solver with parallel candidates, graders, and a shared notebook.
- [ImproofBench FirstProof Batch 2 submission](https://github.com/1stproof/batch-2/tree/main/batch-2-submissions/improofbench) — ProofStack/mathagents, a configurable math-research workflow framework.
- [cumulative-reasoning](https://github.com/iiis-ai/cumulative-reasoning) — Research implementation of proposer, verifier, and reporter agents evaluated on math reasoning tasks.

## Hosted services

- [Primus](https://primus.lab.cloud/) — Hosted autonomous research service with a [math mode](https://lab.cloud/primus/math/), symbolic computation, and optional Lean-checked proofs; access requires an account.

## Historical and unavailable projects

- [AlphaSolve](https://github.com/tanzcoding/AlphaSolve) — Formerly public multi-agent mathematical research project; its source repository is currently private.
- [Alethfeld](https://github.com/tobiasosborne/alethfeld) — Unmaintained adversarial multi-agent proof prototype superseded by Vibefeld.
- [Natty](https://github.com/medovina/natty) — Inactive natural-language proof assistant with an automatic higher-order-logic prover.
- [AlphaSolve, skyshaokai fork](https://github.com/Vegedoge-Doero/AlphaSolve) — Fork of [`skyshaokai/AlphaSolve`](https://github.com/skyshaokai/AlphaSolve), an earlier multi-agent theorem-proving system.

## Contributing

Suggestions and corrections are welcome through issues or pull requests. Please link the canonical project page, give a one-sentence English description, identify what the agent does, and note whether its claims are checked by a proof assistant or reviewed only in natural language. For forks, explain what differs from the upstream project. Report private, archived, or inactive projects so their status stays clear.
