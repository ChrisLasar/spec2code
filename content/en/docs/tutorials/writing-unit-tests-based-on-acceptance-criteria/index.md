---
title: "Writing Unit Tests Based on Acceptance Criteria"
description: "Guide on using an LLM to generate unit tests (e.g., Jest for JS/TS, Pytest for Python) for existing code based on User Stories and their associated Acceptance Criteria."
weight: 50
---

**Key Points:**  

* Understanding how Acceptance Criteria translate into test cases (Given-When-Then).  
* Providing the LLM with the code to be tested and the relevant User Story/Acceptance Criteria.  
* Prompting for specific test functions or methods covering each criterion.  
* Refining generated test code, adding necessary setup/teardown, and ensuring assertions are correct.  
* Running the generated tests and verifying their correctness and coverage against the criteria.

**Assets:**  

* Example User Story and Acceptance Criteria.  
* Example code snippet (e.g., a function or class) to be tested.  
* **Prompt Template:** "Generate Unit Tests from Acceptance Criteria" (Reusable Markdown template).  
* Example LLM interaction flow.  
* Code Snippets: Generated unit test code.  
* *Callout (Inline Tip):* "Tip: Provide the LLM with the signature or interface of the code being tested for better results."  
* *Callout (Inline Note):* "Note: LLMs can generate test *structures* and *ideas* based on criteria, but human expertise is vital for ensuring comprehensive test coverage and correct assertions."
