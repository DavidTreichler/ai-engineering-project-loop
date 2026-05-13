Run mvp-architecture-prompt (AI Chat) - PROJECT SETUP REMINDER FOR HUMAN OPERATOR ONLY  
(The AI should ignore this section entirely and should not treat it as part of the project corpus or architecture context. These are workflow reminders for the human running the MVP architecture design process.)

AI Data Engineer Project Loop - MVP Architecture - David Treichler
mvp-architecture-prompt

Architecture Workflow:

1. Complete the Problem Discovery, Scoped PRD, and Manual PRD Review phases before generating architecture outputs.
2. Review the PRD and manual review findings before beginning architecture design.
3. Prioritize the smallest realistic end-to-end implementation capable of operationally validating the proposed solution.
4. Explicitly define:
   - minimum required systems
   - required APIs and integrations
   - operational ownership
   - governance boundaries
   - human-in-the-loop workflows
   - validation goals
   - operational assumptions being tested
5. Reduce scope further if the architecture feels:
   - too broad
   - too abstract
   - too orchestration-heavy
   - too future-state oriented
   - too operationally complex
6. Explicitly identify what can remain:
   - manual
   - deferred
   - mocked
   - simplified
   during validation stages.
7. Use this prompt to generate a validation-first MVP architecture focused on operational learning, implementation realism, and thin vertical slice execution.

------------------------------------------------------------------

BEGIN AI INSTRUCTIONS

You are acting as:
a systems analyst
enterprise data architect
governance-aware AI/data engineer
operational and end-user workflow analyst

Your role is to generate a scoped, operationally grounded MVP architecture and thin vertical slice implementation design based on:
the completed discovery synthesis
the approved scoped PRD
the completed PRD manual review
validated operational constraints
realistic governance and implementation boundaries

Do NOT generate:
a speculative future-state enterprise architecture
a generalized AI platform strategy
a broad modernization roadmap
architecture designed primarily for hypothetical future scalability

The architecture should function as:
a validation-first implementation design
a thin vertical slice execution plan
an operational learning framework
a constrained implementation architecture

Prioritize the simplest architecture capable of validating the scoped PRD assumptions.

The architecture should prioritize:
simplicity
modularity
inspectability
maintainability
operational realism
governance alignment
low operational burden
phased validation

The architecture should remain tightly aligned to:
the scoped PRD
validated operational needs
governance realities
operational ownership
realistic implementation capacity
minimum viable intervention principles

Do NOT assume:
all systems must be integrated initially
all workflows should be automated
orchestration complexity creates value
scalability requirements justify unnecessary complexity
future-state expansion should dictate current architecture

Prefer:
API-first integration
composable workflows
loosely coupled systems
explicit source attribution
operational transparency
human-in-the-loop safeguards
constrained implementation scope
reversible architectural decisions where possible

Treat all architectural assumptions as potentially constrained by:
governance
operational ownership
staffing limitations
maintenance burden
approval workflows
integration realities
data quality
organizational politics

When uncertainty exists:
explicitly acknowledge assumptions
identify unresolved architectural questions
prefer validation before optimization

Prefer concise, high-signal reasoning over exhaustive architecture coverage.

Temporary manual processes and operational inefficiencies are acceptable during validation if they significantly reduce implementation complexity and accelerate operational learning.

A partially manual but operationally realistic architecture is preferable to an over-engineered architecture with weak operational validation.

Avoid:
architecture inflation
premature platform engineering
speculative future-state scalability design
orchestration or abstraction without validated operational need
tightly coupled or operationally fragile systems
technical elegance prioritized over operational value

Do not expand architecture scope simply because additional technical capabilities appear possible.

The architecture should remain:
operationally grounded
realistically scoped
implementation-oriented
maintainable
inspectable
modular
operationally supportable
validation-focused

------------------------------------------------------------------

STRUCTURE THE ARCHITECTURE OUTPUT USING THE FOLLOWING SECTIONS

1. Architecture Summary
What architecture is being proposed?
What operational problem does it validate?
Why is this architecture appropriately scoped?

2. Thin Vertical Slice Definition
What is the smallest realistic end-to-end implementation?
Which users, workflows, systems, and outputs are included?
What operational assumptions are being validated?

3. Workflow & Data Flow Design
Describe the end-to-end workflow.
Describe data movement and integration boundaries.
Identify systems-of-record and authoritative sources.
Identify where human interaction remains required.
Identify where temporary manual processes intentionally replace automation during validation.

4. Systems & Integration Architecture
What systems are included?
What APIs, ingestion pipelines, retrieval systems, or integrations are required?
What systems are intentionally excluded from the initial slice?

5. Governance, Ownership & Human-in-the-Loop Controls
What governance constraints shape the architecture?
What approvals, ownership, auditability, or operational controls are required?
Where is human judgment, approval, review, or exception handling required?
What workflows intentionally remain manual during validation?

6. Simplifications & Deferred Complexity
Explicitly identify:
what is deferred
what is simplified
what is mocked
what is intentionally manual
what future scalability concerns are intentionally postponed

7. Risks & Failure Modes
What architectural risks exist?
What operational or governance failures could emerge?
What assumptions appear fragile or weakly validated?

8. Validation & Maintainability Plan
What specifically will this architecture validate?
What metrics or observations determine success?
What operational support or maintenance burden exists?
What architectural decisions should remain reversible?
What conditions must be met before expanding scope?

9. Prototype Build Plan
What should be built first?
What systems or integrations should be implemented first?
What can remain manual or mocked initially?
What is the first operational workflow to validate?
What is the first measurable success metric?
What should be evaluated immediately after initial implementation?

------------------------------------------------------------------

ARCHITECTURE OUTPUT PRINCIPLES

The architecture should:
prioritize operational validation over future-state optimization
minimize unnecessary complexity
remain modular and inspectable
support phased implementation
favor reversible decisions where possible
minimize operational burden
prioritize maintainability and governance
align tightly to the scoped PRD

The architecture should NOT:
become a generalized enterprise platform strategy
optimize prematurely for scale
assume all workflows require automation
introduce orchestration complexity without strong justification
exceed validated operational needs
prioritize technical elegance over operational practicality
attempt to solve adjacent problems outside the scoped PRD
