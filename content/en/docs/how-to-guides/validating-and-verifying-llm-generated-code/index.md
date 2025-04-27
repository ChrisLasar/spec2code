---
title: "Validating and Verifying LLM-Generated Code"
description: "Practical steps and recommended practices for ensuring the quality, correctness, security, and performance of code produced by LLMs before integrating it into your codebase."
weight: 20
---

# Validating and Verifying LLM-Generated Code

**Description:** Practical steps and recommended practices for ensuring the quality, correctness, security, and performance of code produced by LLMs before integrating it into your codebase.

**Key Points:**  
  * Implementing a structured manual code review process specifically for LLM output.  
  * Leveraging static analysis tools (linters, formatters like Black, ESLint, Prettier) to enforce code style and catch basic errors.  
  * Running and extending automatically generated tests (as shown in Tutorial 2.4).  
  * Using security scanning tools (SAST) on generated code snippets.  
  * Basic performance considerations and profiling generated code if necessary.  
  * **Reusable Template:** Code Review Checklist for LLM Output (Markdown template).  
  * Mapping output back to spec acceptance criteria
  * Writing lightweight validation prompts
  * Using checklists to catch missing functionality

**Assets:**  
  * Example configurations for linters/formatters.  
  * *Callout (Inline Warning):* "Warning: LLMs can confidently generate insecure code patterns. Security review is non-negotiable."  
  * *Callout (Inline Tip):* "Tip: Integrate linting and formatting into a pre-commit hook to automate checks."
  * 📄 *Mini flowchart: "Spec ➔ Code ➔ Review ➔ Confirm"*
