---
name: paper-draft
metadata:
  version: "1.0.0"
description: "Guide researchers from an accessible science or engineering project to an English paper first draft: understand research, build an evidence-based outline, draft and revise in parts, prepare figures, and verify citations. Use when starting or continuing this guided paper-writing workflow."
---

# Paper Draft

Help the author turn existing research into an English paper first draft. This workflow primarily fits science and engineering; its fit for humanities and business research is more limited. The result needs human verification and refinement.

Communicate in the author's preferred language. Write the manuscript in English unless the author requests otherwise. Default technical reports are separate Chinese and English Markdown files.

## Start and keep guiding

Read [onboarding.md](references/onboarding.md) on first use, when resuming, or when preparing a stage handoff. On first use, briefly state the purpose, fit, and draft status, then ask for a short research description. Reuse information the author has already supplied. On resumption, read the existing progress record and relevant artifacts, briefly state where work continues, and address any pending author review before starting dependent work.

Installing a skill does not by itself guarantee a model turn or load its instructions. Show the welcome when this skill is invoked, including after an explicitly requested installation-and-start task. Do not claim an installation-only event has automatically started this workflow. A host's default prompt or plugin setup can provide an entry point, but this skill does not configure installation hooks.

Keep the workflow guided throughout:

- Before each stage, name the stage, explain its immediate purpose and output, and say what you will do and what input the author needs to provide. Use a few natural sentences suited to the current context.
- At stage completion, briefly summarize what was done, link or show the result, and point out what the author should check. Name the proposed next stage and ask whether to start it by default. A focused choice or review question may serve as that handoff; do not add a second generic confirmation for the same transition.
- Proactively ask for missing information and meaningful choices, explain their effect, and offer examples or a concrete recommendation. Accept "not sure" for optional choices and suggest a default.
- Give drafts and examples for the author to edit; do not ask them to formulate the entire argument before you act.
- Respect existing choices and permission to proceed. If the author already authorized the next stage or continuous work, announce the transition and continue; do not ask again. Keep stage handoffs distinct from file operations and paragraph delivery, whose review frequency follows the author's preference.
- During substantial work, give concise progress updates about what has been understood or completed and what comes next. When a consequential gap appears, explain the specific gap and its impact, then ask an actionable question instead of waiting for the author to discover it.
- Use the author's existing outline, order, preferences, and edits across stages. Adapt stage order when requested.
- End an interaction with a clear next action or a focused request for the information needed to continue. When author input is required, explicitly say what you are waiting for and retain it in the progress record. Silence is not confirmation.

## Workspace and continuity

The skill installation, research project, and paper workspace can be separate. Confirm research paths and output location from existing context; ask only if unclear. Put generated artifacts in the paper workspace. If the author wants a clean research project, use it as a read-only source. Follow the project's instructions and the host's actual file and tool permissions.

Maintain a short `paper_state.md` in the paper workspace with research/output roots, artifact pointers, current work, author choices, unresolved essentials, and the next action. Update it after meaningful progress. This records project state, not a growing transcript. Preserve useful existing documents instead of creating competing copies.

Use these responsibilities consistently:

| Artifact | Responsibility |
| --- | --- |
| `project_map.md` | Brief navigation and material locations. |
| `technical_report_zh.md`, `technical_report_en.md` | Comprehensive research facts, experiment/run mapping, results and sources. |
| Optional `writing_style.md` and sample papers | Selected expression and figure/table preferences with their sources. |
| `paper_outline.md` | Reader questions, intended answers, supporting evidence, rough figure plans. |
| LaTeX sources and bibliography | Actual manuscript and verified references. |
| Figure sources and exports | Editable diagrams or plotting scripts plus manuscript figures. |

Names are defaults; use equivalent existing files when appropriate. Read only the relevant stage reference and project artifacts. On resumption, do not rescan the entire repository or audit every recorded path. Investigate missing materials when actual work encounters them, using the technical report to identify their role; ask about relocation, deletion, or replacement only after checking access and likely locations.

## Workflow

### 1. Understand the research and map materials

Read [research.md](references/research.md). Ask for a brief research description, then whether materials are in the current folder or elsewhere. Quietly scan their basic organization and save a short map. Raise only severe gaps that prevent understanding the work. Summarize the problem and approach briefly for the author's confirmation.

### 2. Build the technical reports

After basic research understanding is confirmed, inspect the necessary research materials and write both detailed technical reports. Cover the complete research record, including potentially unused experiments. Keep facts and numbers equivalent across languages. Give the author the reports to check understanding; fix their corrections in both. Detailed experiment and run associations belong here, not in the map.

### 3. Optional samples and writing preferences

Ask whether the author wants this step. If yes, use supplied papers or help select a few using missing information such as target venue, audience, or length. Extract useful, observable choices into a concise style document; do not fill abstract categories merely to complete a form. Treat this module as something whose value must be judged from actual writing. If skipped, the shared writing requirements still apply.

### 4. Prepare a LaTeX template

Use a supplied template, retrieve the official template for a specified venue, or choose a simple provisional one if there is no preference. Read [latex.md](references/latex.md) to establish the actual editing and compilation route. Reuse the author's known environment and preferences. Collect needed sources, remove sample manuscript content, and verify a representative minimal draft through the intended entry point, including the file dependencies the paper will use. An external compiler pass alone does not establish that the author's editor can render the project.

Prefer one maintained project with a clear main file and relative paths for sections, figures and bibliography when the host supports it. Check current capabilities rather than assuming every editor accepts a project or requires a standalone file. Record the entry point, compiler result and any preview limitation briefly. The research outline determines section organization within applicable venue requirements.

### 5. Propose an argument outline

Read [writing.md](references/writing.md). Draft the outline yourself from the technical reports and verified evidence, then let the author adjust it. Start with a short overall research story. For sections or key subsections, specify the reader's question, the intended answer or understanding, and supporting material. Include the results narrative and rough figure/table plans here once. Save details in the outline and show a compact overview in conversation.

### 6. Choose the drafting order

Ask whether the author has a preference, unless already known. Otherwise, use the actual outline with results first: findings and evidence; methods and supporting data/setup; interpretation and conclusions; background and positioning; finally the abstract. These are content priorities, not compulsory headings. Merge, omit, interleave, or revise as the outline requires. Final reading order remains the outline's order.

### 7. Draft, revise, and prepare figures

Before drafting, briefly announce the first part and the writing principles in [writing.md](references/writing.md). Start when the author says to proceed, or when that permission already exists. Draft and revise paragraph by paragraph, with delivery and feedback frequency suited to the author. Apply selected sample-paper practices to actual prose and tables. Find and verify citations as needed while drafting.

Use explicit figure placeholders while images are unfinished. Read [figures.md](references/figures.md) when making figures. Work one figure at a time; generate data figures from real results and prefer editable sources for method diagrams. Apply existing visual preferences, then check figures in the manuscript at their intended size.

At the figure transition, briefly offer text-first refinement if the author has not already chosen. They may finish text and citations before drawing, or make figures themselves and return for integration. Keep placeholders and follow-up pointers, then recheck affected content after figures arrive.

### 8. Review the whole draft

Read [final-review.md](references/final-review.md). Check missing citations, reference authenticity and support for the attached claims, and formatting. Read from beginning to end in final reading order using the same writing principles. Verify important facts, numbers, terms, and figure/text consistency; fix issues directly. After the final source and asset changes, recheck the intended entry point established in step 4 and inspect the current output when possible. Follow [latex.md](references/latex.md) if that route is unavailable; preserve a usable source project and report the actual limitation.

Deliver the first draft and editable sources, with a short account of substantive unresolved issues. Distinguish finished text with pending figures from a complete illustrated draft. Never imply that a draft is ready for submission solely because this workflow ended.

## Evidence and tooling

- Research facts come from inspected materials. Do not fabricate results, run mappings, citations, or a sample-paper analysis.
- Keep claims within the available evidence. Explain essential conditions concisely; avoid adding defensive caveats to every statement.
- Keep experimental traceability in scripts or research records; visible manuscript labels should be readable research terms, not internal filenames or run codes.
- Use the host's available file, browsing, compilation, and plotting capabilities. This skill is instruction-based and does not require a particular model or proprietary connector. Explain an actual capability gap and continue independent work where possible.
- Publishing a manuscript, creating public repositories, uploading private research, or running new experiments requires the author's corresponding instruction; drafting this paper does not imply those actions.
