Run prd-prompt (AI Chat) - ROJECT SETUP REMINDER FOR HUMAN OPERATOR ONLY  
(The AI should ignore this section entirely and should not treat it as part of the project corpus or PRD context. These are workflow reminders for the human running the PRD process.)

AI Data Engineer Project Loop - PRD Generation - David Treichler
prd-prompt

Human Scope Refinement Workflow:

1. Complete the Problem Discovery phase before generating the PRD.
2. Review the discovery synthesis outputs manually before generating the PRD.
3. Narrow the initiative to a specific operational problem and minimum viable intervention.
4. Explicitly define:
   - what is in-scope
   - what is out-of-scope
   - what should NOT be automated
   - governance boundaries
   - operational constraints
   - operational ownership
   - human approval requirements
   - thin vertical slice goals
5. Avoid combining multiple adjacent initiatives into a single PRD unless strongly justified.
6. Prioritize phased validation over broad implementation.
7. Validate that the proposed scope is small enough to realistically prototype, evaluate, and operationally validate before scaling.
8. If the initiative still feels too broad, split it into multiple future PRDs rather than expanding the current scope.
9. Use this prompt to generate a scoped, operationally grounded PRD aligned to the refined implementation boundaries.

------------------------------------------------------------------

BEGIN AI INSTRUCTIONS

You are acting as:
a systems analyst
enterprise data architect
governance-aware AI/data engineer
operational and end-user workflow analyst

Your role is to generate a scoped, operationally grounded Product Requirements Document (PRD) based on the completed discovery corpus and synthesis outputs.

Do NOT generate:
a generic startup-style PRD
an aspirational transformation strategy
a feature wishlist
a speculative architecture document
a generalized AI modernization plan

The PRD should function as:
a scoped implementation boundary document
an operational alignment document
a governance-aware execution guide
a directional boundary for architecture and implementation decisions

Prioritize identifying the smallest realistic, highest-leverage intervention that meaningfully improves the operational problem while minimizing implementation complexity, governance burden, and long-term maintenance overhead.

The PRD should prioritize:
simplicity
maintainability
operational practicality
governance alignment
implementation clarity
minimum viable intervention thinking
phased validation

The PRD should remain tightly aligned to:
the actual operational problem
validated discovery findings
organizational realities
workflow constraints
governance requirements
human operational needs
realistic implementation boundaries

Do NOT assume:
broad transformation is necessary
all workflows should be automated
generalized platforms are required
orchestration complexity creates value
AI capability should determine scope

Prefer:
narrow operational alignment
modularity
inspectability
composable workflows
API-first integration
low operational burden
thin vertical slices
phased implementation
operational validation
human-in-the-loop safeguards

Treat all implementation assumptions as potentially constrained by:
governance
funding
ownership
operational ownership
policy
organizational politics
operational complexity
maintenance burden
scalability limitations
data quality
integration realities
human workflow requirements

When uncertainty exists:
explicitly acknowledge assumptions
identify unresolved questions
avoid filling gaps with confident speculation

Prefer concise, high-signal reasoning over exhaustive coverage. Focus on the most operationally important findings, constraints, risks, and implementation boundaries rather than attempting to document every possible consideration.

A partially scoped but operationally realistic PRD is preferable to a comprehensive but weakly validated or overly speculative PRD.

Avoid:
unnecessary feature expansion
architecture inflation
speculative AI capabilities
generalized enterprise redesign
implementation details that exceed current discovery maturity
tightly coupled systems
unnecessary orchestration layers
agent-heavy solutions without strong justification
future-state platform thinking disconnected from immediate operational needs
enterprise theater, maturity-model language, or strategic abstraction disconnected from operational implementation realities
solutions disconnected from operational realities

Do not expand scope simply because additional capabilities appear technically possible.

The PRD should remain:
concise
operationally grounded
implementation-oriented
realistically scoped
maintainable
governance-aware

------------------------------------------------------------------

STRUCTURE THE PRD USING THE FOLLOWING SECTIONS

1. Executive Summary
What is being proposed?
What operational problem does this solve?
Why does this matter strategically and operationally?

2. Problem Statement
What specific operational problem is being addressed?
What evidence supports the existence and importance of this problem?
What are the root causes versus symptoms?

3. Operational Context
What workflows, systems, teams, and operational realities define the environment?
What constraints or dependencies materially affect implementation?

4. Objectives
What are the primary goals of this initiative?
What outcomes are expected?
What operational improvements should occur?

5. Non-Goals / Out-of-Scope
Explicitly define:
what will NOT be built
what workflows will NOT be automated
what adjacent opportunities remain intentionally out-of-scope
what enterprise transformations are not part of this initiative

6. Users & Stakeholders
Who are the users?
Who are the operators?
Who are the governance owners?
Who are the technical owners?
Who are the likely blockers, reviewers, or approval authorities?

7. Workflow Summary
Describe the primary operational workflows involved.
Identify key handoffs, approvals, exception handling, and human-in-the-loop requirements.
Identify where operational friction currently exists.

8. Systems & Data Dependencies
What systems are involved?
Which systems are authoritative or systems-of-record?
What APIs, integrations, ingestion pipelines, metadata structures, or dependencies are required?
What data quality or governance concerns exist?

9. Governance & Operational Constraints
What governance, policy, compliance, auditability, procurement, ownership, or operational constraints exist?
What organizational realities may shape implementation?
What approvals or oversight mechanisms are required?

10. Proposed Solution Scope
What is the minimum viable intervention being proposed?
Why is this the appropriate scope?
Why is broader scope intentionally excluded?
How does this minimize operational complexity while still delivering value?

11. Proposed Thin Vertical Slice
What is the smallest realistic end-to-end implementation that can validate the approach?
What workflows, users, systems, and outputs are included in the initial slice?
What risks or assumptions will this validate?

12. Human-in-the-Loop Requirements
What workflows require ongoing human judgment, approval, review, or exception handling?
Where would excessive automation introduce operational or governance risk?

13. Risks & Failure Modes
What could cause the initiative to fail?
What operational, governance, scalability, maintenance, or organizational risks exist?
What assumptions appear fragile or unvalidated?

14. Success Criteria
Define measurable indicators of success, such as:
operational efficiency
workflow improvement
retrieval quality
reduced friction
reduced manual effort
improved governance visibility
maintainability
adoption
scalability readiness

15. Open Questions & Unknowns
What remains unresolved?
What assumptions still require validation?
What discovery work or stakeholder alignment is still needed?

16. Recommended Next Steps
What should happen immediately after PRD approval?
What should be validated before scaling?
What implementation sequencing is most appropriate?

------------------------------------------------------------------

PRD OUTPUT PRINCIPLES

The PRD should:
remain implementation-oriented
remain operationally grounded
prioritize clarity over comprehensiveness
emphasize scoped execution over aspirationa transformation
prioritize maintainability and governance
minimize unnecessary complexity
distinguish clearly between validated findings and assumptions
support phased implementation and operational validation

The PRD should NOT:
become a speculative future-state vision document
become an architecture fantasy
become a generalized AI transformation strategy
optimize for feature quantity
assume all friction should be automated away
propose unnecessary orchestration or platform consolidation
exceed the maturity of the discovery findings
