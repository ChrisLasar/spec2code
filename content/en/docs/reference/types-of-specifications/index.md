---
title: "Types of Specifications"
description: "A brief overview and characteristics of the different specification types featured in the guide, focusing on the kind of information they contain that is valuable for LLM-assisted code generation."
weight: 30
---

# Types of Specifications

**Description:** A brief overview and characteristics of the different specification types featured in the guide, focusing on the kind of information they contain that is valuable for LLM-assisted code generation.

**Key Points:**  
  * Business Requirements Specification (BRS): High-level goals, "Why". Useful for context.  
  * Software Requirements Specification (SRS): Functional and non-functional requirements. Detailed "What". Core input.  
  * Functional Specification Document (FSD): Detailed behavior, user interaction flows. "How it works". Core input.  
  * Technical Specification (TS): Implementation details, data structures, algorithms. "How it's built". Useful for guiding LLM implementation choices.  
  * System Design Specification (SDS): Architecture, component interaction. High-level "How". Useful for ensuring LLM output fits the design.  
  * Interface/API Specifications: Endpoints, data models, request/response formats. Precise input for API code.  
  * Product Requirements Documents (PRDs): Market context, user stories, features. Focus on user value. Useful for context and user stories.  
  * User Stories and Acceptance Criteria: User perspective, testable conditions. Excellent input for generating features and tests.  
  * Test Specifications: Detailed test cases, setup, expected results. Input for test automation or verifying generated tests.
  * Differences
    * Business vs. Technical vs. Functional Specs
    * User Stories vs. Acceptance Criteria
  * What makes a spec "LLM-friendly"?
    * Language modeling ≠ semantic understanding
    * Bias toward plausible completion
    * Clarity, atomicity, consistency
    * Examples of good vs. bad specs

**Assets:**
  * 📄 *Example spec snippets*
  * 📄 *Table of Spec Characteristics*
