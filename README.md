# LLM Evaluation Workbench

A lightweight, browser-based workspace for designing, running, and documenting comparative evaluations of large language models (LLMs).

This project is intentionally **model-agnostic**, **task-agnostic**, and **client-side only**. It is designed to support exploratory analysis, prompt-driven experiments, and structured research notes rather than authoritative benchmarking or leaderboard-style rankings.

---

## Purpose

The LLM Evaluation Workbench enables you to:

- Design and document evaluation prompts
- Run structured comparisons across multiple models
- Capture raw model outputs (e.g. SVG, HTML, code, text)
- Visually inspect rendered outputs directly in the browser
- Record qualitative and quantitative observations
- Archive completed tests for future reference

The tool emphasizes **transparency**, **reproducibility**, and **context preservation** over scoring or ranking.

---

## Key Characteristics

- **Static & portable**  
  Runs entirely in the browser. No backend, no build step, no dependencies.

- **Flexible test design**  
  Suitable for SVG, HTML, reasoning tasks, compression tests, multimodal outputs, or any future evaluation format.

- **Raw output preservation**  
  Stores model outputs verbatim alongside human evaluation notes.

- **Visual inspection first**  
  Rendered views are treated as first-class citizens, not secondary artifacts.

- **Research-oriented**  
  Designed to support discussions, documentation, and longitudinal comparison.

---

## What This Tool Is Not

- Not an official benchmark
- Not a leaderboard
- Not a statistical evaluation framework
- Not affiliated with any model provider

Results are context-dependent and should be interpreted accordingly.

---

## Usage

1. Open `index.html` locally or via GitHub Pages
2. Create a new evaluation project
3. Define the objective and assessment tasks
4. Paste model outputs directly into result fields
5. Switch between code and rendered views as needed
6. Record observations and archive completed tests

All data is stored locally in the browser by default.

---

## Project Structure

repository layout:
llm-evaluation-workbench/
│
├── index.html
├── README.md
├── LICENSE
│
├── structures/
│   ├── svg-benchmarks/
│   │   ├── baseline/
│   │   │   ├── prompt.md
│   │   │   ├── results.json
│   │   │   └── artifacts/
│   │   │       ├── model-a.svg
│   │   │       └── model-b.svg
│   │   ├── minimal/
│   │   └── complex/
│   │
│   ├── reasoning-tests/
│   └── multimodal-tests/
│
└── examples/
└── example-project.json

## Data Storage

By default, projects are stored in browser `localStorage`.

Optionally, completed tests can be:
- Exported as JSON
- Checked into version control
- Referenced directly from GitHub Pages
- Used as discussion artifacts or research citations

A future enhancement may support loading structured test definitions directly from the `structures/` directory.

---

## License

This project is released under the MIT License.

---

## Disclaimer

This tool is intended for exploratory evaluation and documentation.  
Results are context-dependent and should not be interpreted as definitive or authoritative benchmarks.
