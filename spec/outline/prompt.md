# Prompt

I am creating a **practical public-facing guide**, published as a **website**, about how to **transform technical specifications into software solutions** using **LLM-based coding assistance**. The guide emphasizes **specification-centered development** — *the specification is primary; code is secondary* — and should balance **conceptual understanding** with **hands-on guidance**.

## Goal

Generate a **comprehensive, logically structured outline** following the **Diátaxis documentation framework**, clearly dividing the content into:

- **Tutorials** (guided learning experiences),
- **How-to Guides** (goal-driven instructions),
- **Reference** (technical facts and descriptions),
- **Explanations** (concepts, context, rationale).

## Target Audience

- **Roles:** Software engineers, software architects, product owners, product managers
- **Experience Level:** Intermediate familiarity with AI tools; ad-hoc experience with coding assistants

## Tone and Style

- **Professional yet accessible**, similar to **Stripe Docs**: clear, structured, lightly casual without being informal.
- Maintain a strong **balance between "understanding" and "doing."**

---

## Output Requirements

- **Section Titles** and **Subsection Titles** for each Diátaxis category
- **Short Descriptions** and **Key Bullet Points** (specific sub-tasks, concepts, learning goals)
- **Reusable Templates**: Markdown templates for prompts, spec-to-code conversions, review checklists
- **Prompt Engineering Examples** embedded in Tutorials and How-to sections
- **Spec-to-Code Conversion Techniques** suggested throughout
- **Integration Points** for:
  - **Diagrams** (e.g., workflows, model architecture choices)
  - **Flowcharts** (e.g., spec validation pipelines)
  - **Example Specifications** (for different spec types)
  - **Code Snippets** (for sample outputs)
  - **Callout Boxes** (tips, warnings, notes, common misconceptions — *embedded inline* rather than as standalone chapters)

---

## Specific Areas to Cover

- **Lifecycle Management Challenges**: How to align evolving specs with LLM-generated code
- **Common Pitfalls and Misconceptions**: Embedded naturally via inline callouts
- **Platform Differences**:
  - Classic IDE extensions (e.g., GitHub Copilot in VSCode)
  - AI-native IDEs (e.g., Cursor, Windsurf)
  - Local LLM deployments (e.g., via Ollama)
- **Recommended Practices**:
  - Effective prompt engineering for spec-to-code
  - Selecting tools/libraries (including checking for `llm.txt` or `llmd.txt` metadata — *define these if they're not standard*)
  - Validating, testing, and reviewing LLM output

---

## Technologies and Context to Assume

- **Primary Languages:** Python, TypeScript, React, Tailwind
- **Key LLM Tools/Platforms:** GitHub Copilot, Cursor, Windsurf, Local models via Ollama
- **Typical Project Types:** REST APIs, CRUD apps, Web applications
- **Assumed Human-Led Workflow:** Specifications and verifications are performed by humans; code generation is accelerated by LLMs.

---

## Types of Specifications to Feature

- Business Requirements Specification
- Software Requirements Specification
- Functional Specification Document
- Technical Specification
- System Design Specification
- Interface/API Specifications
- Product Requirements Documents (PRDs)
- User Stories and Acceptance Criteria
- Test Specifications

---

> ⚡ **Important**: Optimize for **immediate usability**. Make it easy to imagine how each section becomes an actual page on a public guide site.

---

## ✅ Deliverable

A clean, organized outline — fully populated with:

- Logical flow across Tutorials, How-To Guides, Reference, and Explanations
- Practical assets embedded (templates, examples, callouts, diagrams)
- Clear mapping from specification types to learning activities
