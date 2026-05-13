# AI Engineering Project Loop

A lightweight workflow for turning AI and data engineering ideas into scoped, validated, operational projects.

This repo is designed for practitioners who use AI assistants, notebooks, code repos, documents, workflows, and iterative experimentation to build real-world AI systems. It emphasizes scope control, thin vertical slices, operational realism, human review, and validation before scaling.

## Why this exists

Many AI projects fail because they become too broad, too automated, or too complex before the actual operational problem is understood. This loop keeps the work grounded:

text messy idea -> problem discovery -> scope refinement -> scoped PRD -> MVP architecture -> build -> validate -> iterate -> operationalize -> scale carefully 

## Core principles

Start messy, then refine.
Solve the actual operational problem first.
Build the smallest meaningful intervention.
Prefer thin vertical slices over broad platform designs.
Validate before scaling.
Keep humans in the loop where risk, uncertainty, policy, privacy, financial impact, or operational consequences are meaningful.
Treat AI systems as operational systems, not demos.
Keep the method lightweight enough to actually use.

## Project loop

1. Raw Brain Dump  
   Capture problems, frustrations, workflows, documents, assumptions, and rough ideas.

2. Problem Discovery  
   Use AI to organize the mess into candidate problems, constraints, workflows, and opportunities.

3. Scope Refinement  
   Human review checkpoint. Decide what matters most, what is out of scope, and what should not be automated.

4. Scoped PRD  
   Convert the selected problem into a focused product requirements document.

5. PRD Review  
   Human review checkpoint. Check scope, assumptions, operational fit, risks, and feasibility.

6. MVP Architecture  
   Design the smallest viable end-to-end system or workflow.

7. Build MVP  
   Build the thin vertical slice. Capture implementation notes, decisions, issues, and artifacts.

8. Validation  
   Test whether the MVP actually works, where it fails, and what should change next.

9. Operationalization  
   Decide whether the workflow can run reliably with real constraints, users, data, and oversight.

10. Scaling  
   Expand only after the system has proven useful, understandable, governable, and maintainable.

## Repository structure

text ai-engineering-project-loop/ | ├── README.md ├── LICENSE | ├── 01-raw-brain-dump/ ├── 02-problem-discovery/ ├── 03-scope-refinement/ ├── 04-scoped-prd/ ├── 05-prd-review/ ├── 06-mvp-architecture/ ├── 07-build-mvp/ ├── 08-validation/ ├── 09-operationalization/ ├── 10-scaling/ | ├── prompts/ ├── templates/ ├── examples/ └── docs/ 

## How to use this repo

Use the numbered folders as the project lifecycle. Use prompts/ for reusable AI prompts, templates/ for repeatable project artifacts, examples/ for completed or sample workflows, and docs/ for reference material.

The goal is not to create process for its own sake. The goal is to make AI engineering work easier to scope, build, validate, and operate.

## Status

Early public release. Actively evolving through real-world usage and experimentation.
