---
title: "Managing Changes and Spec Evolution"
description: "Strategies and techniques for handling updates and changes to specifications over time and aligning them with previously generated and potentially human-modified code. Addresses the 'lifecycle management challenge'. Strategies for uncertainty."
weight: 30
---

# Managing Changes and Spec Evolution

**Description:** Strategies and techniques for handling updates and changes to specifications over time and aligning them with previously generated and potentially human-modified code. Addresses the "lifecycle management challenge". Strategies for uncertainty.

**Key Points:**  
  * Identifying and assessing the impact of changes in an updated specification.  
  * Deciding whether to attempt regenerating the affected code section or manually modifying the existing code.  
  * Using version control (Git) and diffing tools effectively to understand changes.  
  * Strategies for merging LLM-generated code updates with existing human-written code, minimizing conflicts.  
  * Documenting which parts of the codebase originated from LLM generation and which were human-modified.
  * Triaging missing information
  * Hypothesis-driven prompting
  * Annotating assumptions

**Assets:**  
  * **Flowchart:** "Spec Change Handling Workflow with LLMs" (Placeholder for a visual diagram).  
  * *Callout (Inline Note):* "Note: Regenerating large sections of code can be faster initially but may lead to more complex merges later."  
  * *Callout (Inline Tip):* "Tip: Use clear commit messages indicating when code was LLM-generated vs. human-written."
  * ⚡ *Callout: Risk of hallucinations when specs are weak*
  * 📄 *"Assumption Tracker" Template*
