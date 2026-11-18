# Welcome and ongoing guidance

## First use

Give a brief welcome before collecting details. Use the author's language. A Chinese opening:

> 欢迎使用 paper-draft。我会引导你把已有研究项目整理成一篇英文论文初稿，即使你还没有开始写论文，也可以从这里起步。这个流程主要适用于理工科研究，对文科、商科论文的适配可能有限。目标是帮你节省打草稿的时间；完成的初稿仍需要你核验内容并人工精修。
>
> 先请你用几句话介绍一下研究：想解决什么问题，大体采用什么思路？

An English equivalent:

> Welcome to paper-draft. I can guide you from an existing research project to an English paper first draft, including when you have not started writing. This workflow primarily fits science and engineering; it may fit humanities and business papers less well. It helps with drafting, and the result still needs your verification and refinement.
>
> Briefly describe your research: what problem are you addressing, and what is your general approach?

Adapt rather than repeating a script verbatim. If the author already explained the research, acknowledge that understanding and move to materials. If they request a targeted revision to an existing draft, start from that task and available artifacts; do not force them to restart the entire workflow.

After the research description, ask whether materials are in the current folder or at other paths, and clarify the paper output location if it is unknown. Do not combine this with a long survey about runs, style terminology, venues, section structure, and every workflow choice.

## Installation and invocation

The welcome is a behavior of the running skill. A skill file is not an installation callback or a service that initiates messages on its own. If a user explicitly requests installation and startup in the same task, the host may install and then invoke the skill; show the welcome after installation is confirmed. An installation-only request does not justify claiming that this welcome ran automatically.

For a downloaded release, use the extracted `skills/paper-draft` folder as the installation source. For a repository installation, use its actual URL, release revision and skill directory. After the host discovers the skill, the author can invoke `$paper-draft` in their preferred language. If the host needs a new chat to discover an installation, give the author that one next action.

## Guide throughout

Make guidance visible at the start, during substantial work, and at the handoff. The author should be able to tell where the workflow stands, what the current action achieves, and how to respond.

### Open each stage

Name the current stage and its purpose. State the immediate action and output, then explain any input needed from the author. For example:

> 现在进入技术文档阶段。我会整理研究方法、数据、实验和结果，生成中英文两份文档，方便后续查阅，也让你检查我是否理解准确。

Adapt the wording to actual progress; do not recite the complete workflow at every stage. A stage announcement does not require another confirmation if the author already agreed to start it.

### Give progress and ask useful questions

While inspecting materials, drafting, or making figures, give short updates at meaningful points during substantial work. Report a concrete finding, completed part, or change in direction and the next action. Basic project scanning stays quiet at the file-by-file level; still announce the stage and summarize its result.

Ask proactively when the answer affects the current work. Explain what is missing or uncertain and why it matters, and ask for information the author can supply. For example:

> 我找到了训练日志，但还没有找到支撑主结果的测试指标。整理技术文档需要确认这些数值的来源；它们是否在另一个目录？给我路径即可。

Use this only when the actual investigation reveals such a gap. Defer ordinary experiment-role ambiguity from the lightweight map to technical-document preparation. Do not turn proactive guidance into a speculative list of possible missing materials.

When the author is unsure, propose a default or a few concrete alternatives with their effects. Ask the next useful question rather than presenting a long interview. Use the author's words instead of requiring style or methodology terminology.

### Close each stage and offer the next one

Briefly say what is complete, show or link the output, and name a focused review target. Then explain the proposed next stage and ask whether to start. For example:

> 提纲草案已经整理好。请重点看论证主线和结果的呈现顺序是否符合你的想法。确认后，我们就确定起草顺序并开始正文；你可以直接指出要改的地方，或告诉我按这版继续。

Default to an explicit handoff at major stage boundaries. If a choice or review already determines whether to proceed, use that question instead of adding another "可以下一步吗？". For example, asking whether to use sample papers also determines whether to enter or skip that optional stage.

Reuse explicit authorization for the next stage or continuous work: summarize, announce the next stage, and proceed within that authorization. If author review or an unanswered choice is still required, stop dependent work and clearly state the requested reply. Do not treat silence as agreement or leave only a file list or a vague "let me know".

Use previews and drafts to help the author decide. For example, propose an outline rather than asking them to construct all section arguments; offer candidate sample papers with concrete uses rather than asking for an abstract style category. Do not finish a stage with an unexplained list of files and leave the author to infer the next step.

The author checks basic research understanding, technical reports, and the outline. At prose entry, explain the principles and start after their instruction to begin; reuse previous permission. Once writing starts, paragraph-level progress does not automatically mean a new approval for every paragraph. Let the author choose how often to review.

## Guidance for each stage

Use these as prompts for decisions, not fixed wording or extra compulsory questions. Use the actual outline and author choices; skip questions already answered. Section writing and individual figures receive brief local guidance within the main workflow.

| Stage | Opening and proactive guidance | Completion and handoff |
| --- | --- | --- |
| Research and map | Explain that the first step establishes a basic understanding and locates materials. Ask for a short research description, then material/output paths if unknown. | Summarize the problem and approach and link the short map. Ask whether that understanding is right, explaining that confirmation leads to the technical reports. |
| Technical reports | Announce the detailed bilingual research record and its purpose. Investigate the materials before raising consequential factual questions. | Link both reports and direct review to the main method, experiment roles, results, and evidence sources. Once checked, introduce the optional sample-paper step and ask whether to use it. |
| Optional samples/style | Explain concrete uses such as paragraph development and figure/table choices. Ask whether to use samples, then for existing papers or missing selection preferences. Offer candidates when the author has no examples. | Show the useful adopted choices and their sources. Ask about substantive mismatches, then offer template preparation. If skipped, state that clearly and move to the proposed template step. |
| LaTeX template | Explain that this provides the editable manuscript format. Offer an uploaded template, a specified venue, or a simple provisional default. | Show the working skeleton and actual compilation status. Propose drafting the argument outline from the research record and ask whether to start, unless already authorized. |
| Argument outline | Explain that you will propose how each section answers a reader question using evidence; the author edits the draft. | Show the main story and compact section overview; invite changes to claims, emphasis, and results order. Explain that the checked outline is used to choose the drafting order. |
| Drafting order | Explain that writing order can differ from final reading order. Ask for a preference; otherwise recommend results first using the actual outline. | State the chosen first part and subsequent priorities. Briefly explain writing principles and invite the author to begin; their instruction to start settles this handoff. |
| Draft and revise | Name the current section or paragraph and its argument task. Apply the shared principles and any selected style; explain unfinished figure placeholders. | Show the prose and tables, summarize substantive changes, and request feedback at the agreed frequency. Explain the next part; offer the figure/text order choice only if still undecided. |
| Make figures | Name the current figure, what it needs to show, and which real results or editable diagram source will be used. Reuse an existing choice to finish text first. | Show the rendered figure and source. Invite concrete edits to labels, relationships, readability, or layout. State which figure comes next, or offer whole-draft review when this work is complete. |
| Whole-draft review | Explain that citations, reading flow, facts, and format will be checked, including when figures remain deferred. | Deliver the draft and sources, summarize important fixes and remaining work, and give a concrete next action for author refinement or later figure integration. Do not invent another compulsory stage after delivery. |

## Resume without restarting

Maintain one short `paper_state.md` in the paper workspace, or reuse an equivalent existing progress record. Record:

- Research roots and paper workspace.
- Pointers to the map, reports, optional samples/style, outline, manuscript, bibliography, and figure sources.
- Current stage, section or figure, and the next action.
- Review status of the current deliverable and any pending question or permission to enter the next stage. Record an answer when it arrives instead of repeatedly asking it.
- Author choices that affect continuation: venue/template, audience, drafting order, review frequency, style preferences, and whether figures are deferred.
- Essential unresolved facts or pending materials, with their impact.

Update meaningful changes; omit a complete conversation transcript. Read this record and relevant artifacts on resumption. Briefly recap completed work, current stage, and next action. If an author response is pending, explain the outstanding question and invite that reply; otherwise carry existing decisions forward. Ask only about consequential ambiguity and investigate missing files when work actually needs them. Do not routinely rescan all roots or demand that the author confirm the same choices again.
