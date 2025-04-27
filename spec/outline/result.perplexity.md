Here’s a structured outline for your specification-centered LLM coding guide, following the Diátaxis framework:

---

## Tutorials  
*Guided learning paths for core workflows*  

**Quickstart: From Spec to Deployed Feature**  
- Build a REST API endpoint using a functional spec  
- Key steps: Spec drafting → LLM prompt design → code generation → testing → deployment  
- Includes:  
  - Sample spec template (Markdown)  
  - Copilot/Cursor setup checklist[4][6]  
  - Common pitfall callout: *"Ambiguous requirements → hallucinated code"*

**Writing LLM-Friendly Specifications**  
- Tutorial on creating machine-parsable specs:  
  - Atomic user stories  
  - Testable acceptance criteria  
  - API contract syntax examples (OpenAPI/YAML)[3]  
- Hands-on: Convert vague requirements into structured prompts  

**Generating Code with Progressive Prompting**  
- Walkthrough of arXiv paper's iterative method[3]:  
  1. Extract functional requirements  
  2. Create UML diagrams  
  3. Generate unit tests  
  4. Implement code  
- Embedded workflow diagram: *Spec → Object Model → Tests → Code*

---

## How-to Guides  
*Task-specific instructions*  

**Setting Up Your LLM Coding Environment**  
- Platform comparisons:  
  | **IDE Type**       | **Example Tools**       | **Best For**            |  
  |---------------------|-------------------------|-------------------------|  
  | Classic Extensions  | GitHub Copilot          | Lightweight assistance  |  
  | AI-Native IDEs      | Cursor, Windsurf        | Full workflow integration[4] |  
  | Local LLMs          | Ollama + VS Code        | Privacy-sensitive projects |  

**Converting Specification Types to Code**  
- Recipes for:  
  - User Stories → Python FastAPI endpoints  
  - API Specs → TypeScript interfaces  
  - System Design Docs → React component trees  
- Prompt template:  
  ```markdown  
  Given this {spec_type}, generate {language} code that:  
  1. Implements {key_functionality}  
  2. Uses {required_libraries}  
  3. Follows {coding_standard}  
  ```

**Validating LLM Output**  
- Adaptation of TICK checklist method[6]:  
  - Requirement traceability matrix  
  - AI-generated validation questions:  
    *"Does the code implement all acceptance criteria from section 2.3?"*  
    *"Are there proper error handlers for API edge cases?"*  

---

## Reference  
*Technical specifications and templates*  

**LLM Tool Directory**  
- Categorized list from Awesome Code LLM[2]:  
  - **Code Generation**: Codex, StarCoder  
  - **Testing**: CodiumAI, TestPilot  
  - **Refactoring**: Smol AI  

**Specification Templates**  
- Markdown skeletons for:  
  - Software Requirements Spec (SRS)  
  - API Contract  
  - User Story + Acceptance Criteria  
  - System Design Doc (with architecture decision records)  

**Prompt Engineering Cookbook**  
- Reusable patterns:  
  ```python  
  # Context injection  
  "Given {spec_excerpt}, write {language} code that..."  
  
  # Chain-of-thought  
  "First, identify required components. Then..."  
  ```

---

## Explanations  
*Core concepts and rationale*  

**Why Specification-Centered Development?**  
- Comparative analysis:  
  - Traditional workflow: Code → Docs  
  - LLM-era workflow: Specs → Code → Auto-docs[3][4]  
- Diagram: *Virtuous cycle of spec-driven development*

**Lifecycle Management Strategies**  
- Techniques for:  
  - Version-locking specs and code[4]  
  - Drift detection between docs/implementations  
  - Retrofitting legacy code with specs  

**Prompt Engineering Principles**  
- Cognitive load reduction methods:  
  - Chunking complex specs  
  - Leveraging UML as intermediate representation[3]  
  - Checklist-driven generation[6]  

---

## Embedded Assets  

**Workflow Diagrams**  
- Mermaid.js flowcharts for:  
  - Spec validation pipeline  
  - CI/CD integration points  

**Code Snippets**  
- TypeScript example:  
  ```typescript  
  // Generated from API spec  
  interface UserEndpoint {  
    GET: (id: string) => User;  
    POST: (user: User) => ApiResponse;  
  }  
  ```

**Callout Boxes**  
- ![](https://via.placeholder.com/20/ffd700/Pro Tip**:  
  *"Maintain a `llmd.txt` file with model temperatures/stop sequences for reproducible generations"*  

---

This structure enables progressive learning while maintaining quick reference utility, addressing both strategic (architects/pm) and tactical (developers) needs. Each section contains actionable templates and real-world examples drawn from cited research[3][4][6].

Citations:
[1] https://diataxis.fr
[2] https://github.com/codefuse-ai/Awesome-Code-LLM
[3] https://arxiv.org/html/2406.10101v2
[4] https://ghuntley.com/specs/
[5] https://www.pinecone.io/learn/series/langchain/langchain-prompt-templates/
[6] https://arxiv.org/html/2410.03608v1
[7] https://stephencollins.tech/posts/crafting-prompt-templates-for-code-generation
[8] https://www.getambassador.io/blog/openapi-integration-turn-specs-into-code
[9] https://www.archbee.com/blog/diagrams-in-developer-documentation
[10] https://nulab.com/learn/design-and-ux/keep-it-simple-follow-flowchart-rules-for-better-diagrams/
[11] https://help.obsidian.md/Editing+and+formatting/Callouts
[12] https://docs.oracle.com/en/java/javase/18/code-snippet/index.html
[13] https://www.scrumlaunch.com/blog/ai-coding-assistants-and-ides-you-might-have-missed-challenges-and-future-potential/
[14] https://www.builder.io/blog/cursor-vs-windsurf-vs-github-copilot
[15] https://www.e2enetworks.com/blog/top-8-open-source-llms-for-coding
[16] https://arxiv.org/html/2408.05002v5
[17] https://orq.ai/blog/managing-the-ai-lifecycle
[18] https://www.linkedin.com/pulse/llm-myths-separating-reality-from-bs-david-berigny-qcirc
[19] https://www.confident-ai.com/blog/llm-testing-in-2024-top-methods-and-strategies
[20] https://idratherbewriting.com/blog/what-is-diataxis-documentation-framework
[21] https://www.sonarsource.com/learn/ai-assisted-software-development/
[22] https://pieces.app/blog/llm-prompt-engineering
[23] https://www.gliffy.com/blog/diagrams-as-code
[24] https://technicalwritingmp.com/docs/technicalwritingcourse/use-of-diagrams/
[25] https://quarto.org/docs/authoring/callouts.html
[26] https://blog.n8n.io/best-ai-for-coding/
[27] https://www.qodo.ai/blog/best-ai-coding-assistant-tools/
[28] https://www.linkedin.com/pulse/8-most-common-mistakes-building-llm-applications-2024-guy-korland-jmz6f
[29] https://arxiv.org/html/2503.06327v2
[30] https://www.reddit.com/r/AskProgramming/comments/1j8lnn7/a_genuine_question_to_people_who_work_as_software/
[31] https://danielsieger.com/blog/2023/04/24/framework-for-better-documentation.html
[32] https://swimm.io/learn/ai-tools-for-developers/ai-code-assistants-key-capabilities-and-5-tools-to-know-about
[33] https://dev.to/documatic/user-guides-in-code-documentation-empowering-users-with-usage-instructions-3lmo
[34] https://eclipsesource.com/blogs/2025/01/21/using-starcode-for-ai-code-completion-in-theia-ide/
[35] https://arxiv.org/html/2503.05012v1
[36] https://ubuntu.com/blog/diataxis-a-new-foundation-for-canonical-documentation
[37] https://www.tabnine.com/blog/ai-code-assistant-guide/
[38] https://www.katara.ai/blog/diataxis
[39] https://nix.dev/contributing/documentation/diataxis.html
[40] https://www.reddit.com/r/technicalwriting/comments/n4irfk/di%C3%A1taxis_a_pragmatic_system_for_technical/
[41] https://diataxis.fr/how-to-guides/
[42] https://fachglossar.platinus.at/docs/Glossar/D-Glossar/Diataxis-Framework/
[43] https://discuss.ocaml.org/t/diataxis-documentation-structure/7750
[44] https://www.youtube.com/watch?v=hdjb4rffEjM
[45] https://docs.gitbook.com/guides/best-practices/documentation-structure-tips
[46] https://news.ycombinator.com/item?id=42325011
[47] https://artificialintelligenceact.eu/introduction-to-code-of-practice/
[48] https://www.publicissapient.com/insights/guide-to-ai-assisted-software-development
[49] https://www.computerweekly.com/feature/LLMs-explained-A-developers-guide-to-getting-started
[50] https://arxiv.org/pdf/2406.10101.pdf
[51] https://arxiv.org/html/2412.05299v2
[52] https://www.eficode.com/guides/using-genai-in-software-development
[53] https://vlinkinfo.com/blog/guide-to-llm-product-development/
[54] https://www.bsi.bund.de/SharedDocs/Downloads/EN/BSI/KI/ANSSI_BSI_AI_Coding_Assistants.pdf?__blob=publicationFile&v=7
[55] https://arxiv.org/html/2409.17434v1
[56] https://www.appgambit.com/guide/enhancing-software-spec-process-with-agents-tools-and-llm
[57] https://semaphoreci.com/blog/selfhosted-llm-coding-assistants
[58] https://www.cs.wm.edu/~dcschmidt/PDF/LLM-chapter-2024-12-15.pdf
[59] https://www.reddit.com/r/ChatGPTCoding/comments/1f51y8s/a_collection_of_prompts_for_generating_high/
[60] https://www.promptingguide.ai/models/mistral-7b
[61] https://github.com/dair-ai/Prompt-Engineering-Guide
[62] https://learnprompting.org/docs/basic_applications/coding_assistance
[63] https://openreview.net/forum?id=1dUdNzLJRF
[64] https://python.langchain.com/docs/concepts/prompt_templates/
[65] https://platform.openai.com/docs/guides/prompt-engineering
[66] https://www.blazemeter.com/blog/openapi-spec-from-code
[67] https://ubc-mds.github.io/fixml/
[68] https://github.com/f/awesome-chatgpt-prompts
[69] https://dev.to/shannonlal/improving-llm-code-generation-with-prompt-engineering-43b9
[70] https://www.globalspec.com/reference/58763/203279/5-5-code-conversion
[71] https://www.modlee.ai/blog/ticking-all-the-boxes-generated-checklists-improve-llm-evaluation-and-generation
[72] https://community.openai.com/t/prompt-preamble-prompt-template-for-virtual-assistant/309524
[73] https://www.archbee.com/blog/software-documentation-diagrams
[74] https://www.yworks.com/pages/software-documentation-with-uml-diagrams
[75] https://www.reddit.com/r/embedded/comments/v4f69b/draw_a_flow_chart_before_writing_code_for_a_new/
[76] https://preethac.github.io/files/SANER17.pdf
[77] https://www.embeddedrelated.com/showarticle/1685.php
[78] https://clickhelp.com/clickhelp-technical-writing-blog/using-diagrams-in-it-documentation-best-practices/
[79] https://docs.splunk.com/Documentation/StyleGuide/current/StyleGuide/Notesandcautions
[80] https://learn.microsoft.com/en-us/visualstudio/ide/code-snippets?view=vs-2022
[81] https://help.hcl-software.com/unica/Campaign/en/12.1.7/Campaign/Introduction/unica_campaign_integration_with_callout_process_box.html
[82] https://www.contentful.com/blog/how-to-design-technical-flowcharts/
[83] https://jamesg.blog/2023/12/25/callout-boxes/
[84] https://swimm.io/learn/code-documentation/code-documentation-examples-and-lessons-learned
[85] https://www.shakudo.io/blog/best-ai-coding-assistants
[86] https://www.pragmaticcoders.com/resources/ai-developer-tools
[87] https://www.infralovers.com/blog/2024-06-13-ai-powered-programming/
[88] https://www.reddit.com/r/devsarg/comments/1jf8ax7/cursor_windsurf_copilot_trae_veni_te_cuento_mis/?tl=en
[89] https://theia-ide.org/docs/user_ai/
[90] https://www.reddit.com/r/ChatGPTCoding/comments/1gwghx1/i_tried_cursor_vs_windsurf_with_a_medium_sized/
[91] https://www.techradar.com/computing/artificial-intelligence/best-large-language-models-llms-for-coding
[92] https://www.bitdoze.com/ai-coading-tools/
[93] https://dev.to/builderio/best-ai-code-editors-in-2025-4kaf
[94] https://www.zdnet.com/article/the-best-ai-for-coding-in-2025-and-what-not-to-use-including-deepseek-r1/
[95] https://www.reddit.com/r/ChatGPTCoding/comments/1gstryh/are_ai_assistant_llms_worse_than_their_native/
[96] https://www.geuni.tech/en/deepseek-r1-ollama-vscode-setup
[97] https://dev.to/hackmamba/these-are-the-best-large-language-models-for-coding-1co2
[98] https://kaiomagalhaes.com/blog/personal-experience-with-ai-first-ides
[99] https://cohere.com/blog/5-challenges-of-working-with-large-language-models-and-how-to-cope-with-them
[100] https://publications.rwth-aachen.de/record/994149/files/994149.pdf
[101] https://www.linkedin.com/posts/luminousmen_hidden-pitfalls-of-llm-in-education-activity-7254559751877873664-qr4G
[102] https://www.evidentlyai.com/llm-guide/llm-as-a-judge
[103] https://www.sciencedirect.com/science/article/abs/pii/S0950584925000369
[104] https://www.computer.org/publications/tech-news/trends/large-language-model-lifecycle/
[105] https://masterofcode.com/blog/llms-myths-vs-reality-what-you-need-to-know-before-the-invest
[106] https://www.confident-ai.com/blog/llm-evaluation-metrics-everything-you-need-for-llm-evaluation
[107] https://www.frontiersin.org/journals/medicine/articles/10.3389/fmed.2025.1527864/full
[108] https://www.deepchecks.com/question/what-are-the-challenges-of-ml-lifecycle-management/
[109] https://community.openai.com/t/llms-seem-to-be-flawed-at-the-core-for-real-programming-help-needed/1128555
[110] https://www.kaggle.com/code/youssef19/llm-output-validation-evaluation
[111] https://diataxis.fr/how-to-use-diataxis/
[112] https://docs.readthedocs.com/platform/stable/explanation/documentation-structure.html
[113] https://discuss.python.org/t/diataxis-and-python-documentation/41836
[114] https://www.frontiersin.org/journals/computer-science/articles/10.3389/fcomp.2025.1519437/pdf
[115] https://www.turing.com/resources/llm-coding-assistants-increase-software-development-productivity
[116] https://www.clouddefense.ai/code/javascript/example/swagger2openapi

---
Antwort von Perplexity: pplx.ai/share