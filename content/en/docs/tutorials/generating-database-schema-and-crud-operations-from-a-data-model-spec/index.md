---
title: "Generating Database Schema and CRUD Operations from a Data Model Spec"
description: "Guide on using an LLM to create database schema definitions (SQL CREATE TABLE statements) and basic CRUD functions (e.g., Python with SQLAlchemy or TypeScript with Mongoose) based on a Data Model or relevant section of a Software Requirements Specification."
weight: 40
---

**Key Points:**  

* Identifying entities, attributes, relationships, and data types from the spec.  
* Representing data relationships (one-to-one, one-to-many, many-to-many) clearly in prompts.  
* Prompting for SQL schema definitions or ORM model classes.  
* Generating basic functions for Create, Read, Update, and Delete operations for one or more entities.  
* Choosing between generating raw SQL or ORM code based on project needs and prompting accordingly.

**Assets:**  

* Example Data Model snippet from an SRS or a dedicated Data Specification.  
* **Prompt Template:** "Generate Database Schema/CRUD from Spec" (Reusable Markdown template).  
* Example LLM interaction flow.  
* Code Snippets: Generated SQL schema, generated ORM models, generated CRUD function stubs.  
* *Callout (Inline Warning):* "Warning: Always review generated schema definitions and raw SQL for potential security vulnerabilities (e.g., lack of proper escaping, injection risks)."  
* *Callout (Inline Note):* "Note: LLMs are good at generating standard CRUD patterns, but complex query logic often requires significant human guidance or writing."
