# paper-draft v1.0.0 · 英文论文初稿助手 / English paper drafting assistant

[中文](#中文) · [English](#english)

## 中文

带上已有的研究材料，用你习惯的语言讨论，逐步写出一篇可以自己修改的英文初稿。适合理工科研究。你可以从研究思路讲起，也可以带着已有提纲、初稿或待整理的实验结果开始。

可以用中文或英文开始和继续讨论。默认生成中英文各一份技术报告，论文正文默认用英文，也可以指定其他语言。在 Codex 的技能列表里，显示名称为“英文论文初稿助手”，调用名为 `$paper-draft`。

### 从 ZIP 开始

1. 解压分享包。打开 `skills/paper-draft/`，里面应直接看到 `SKILL.md`、`agents/` 和 `references/`。
2. 在能访问解压目录的本地 Codex 中，把下面提示里的路径替换成实际位置并发送。也可以手动将整个 `paper-draft` 文件夹复制到用户目录下的 `.agents/skills/`。安装后入口应为 `~/.agents/skills/paper-draft/SKILL.md`。

   > 请把我解压目录里的 `〈实际路径〉/skills/paper-draft` 安装为当前用户的 Codex skill。安装完成后，用中文引导我开始写英文论文初稿。

3. 如果安装完成后还没进入开场白，打开一个新对话，发送下面这句。

   > 使用 $paper-draft，开始引导我写英文论文初稿。

首次使用会先问你想解决什么问题、用了什么方法。如果研究材料放在其他目录，把可访问的路径和希望保存论文的目录一起告诉它。安装位置说明见 [OpenAI 的 skill 指南](https://learn.chatgpt.com/docs/build-skills)。

### 准备材料和选择节奏

研究代码、数据说明、实验配置和已有结果可以分开存放。结果表最好能对应回原始实验记录。你可以指定只读目录、输出位置、不能访问的子目录和审阅节奏，例如：

> 我的研究材料在当前项目的 `experiments/`。请把生成物放到 `draft/`，跳过 `old_manuscript/`。先和我核对研究问题和主实验。确定提纲后连续起草，我按章节审阅。

### 从研究到交付

1. 确认研究问题和方法，建立简短的材料地图。
2. 整理中英文技术报告，核对结果及其来源。
3. 按需选几篇范文，提炼具体的写作和制图偏好。
4. 准备期刊或临时 LaTeX 模板，在作者实际使用的编辑器或编译器里检查章节、图片和引用。
5. 提出论证提纲，说明每节回答什么问题、依据是什么。
6. 确定起草顺序，默认从结果开始。
7. 写正文，核对引用与表格，用实验记录制作结果图，保留图稿和绘图脚本。
8. 从头通读，核查数字、引用和图文关系，交付可编辑稿件及待作者核实的事项。

作者可以先精修文字再制图，也可以自己制图后交回整合。接着上一次工作时，论文目录中的 `paper_state.md` 记录当前阶段、已作的选择和下一步。

### 可以怎样判断产出

此次试用从研究说明走到了一份 13 页的英文图文初稿，包含 2 张图和 8 张表。该项目在测试的 Linux 桌面环境中通过了内置多文件 LaTeX 编译。其他编辑器和全新安装的运行环境，需要分别确认依赖和实际预览。初稿中的研究解释、引用支持范围和待补事实仍由作者核实。

## English

Use your existing research materials to write an editable first draft of a science or engineering paper. Start with a research question, an outline, a partial manuscript or a set of results you want to explain.

You can start and continue the conversation in English or Chinese. By default, the skill produces a technical report in each language and writes the manuscript in English. You can request another manuscript language. In the Codex skill selector, look for **英文论文初稿助手**, or invoke it by name with `$paper-draft`.

### Install from the ZIP

1. Unzip the release and open `skills/paper-draft/`. It should contain `SKILL.md`, `agents/` and `references/`.
2. In a local Codex session with access to the extracted folder, replace the example path in the following prompt with your own and send it. For manual installation, copy the entire `paper-draft` folder into `.agents/skills/` in your home directory. The resulting entry point should be `~/.agents/skills/paper-draft/SKILL.md`.

   > Please install the skill from `<extracted-folder>/skills/paper-draft` for my Codex user account. Once it is available, start guiding me through an English paper draft.

3. If the welcome message does not appear after installation, open a new chat and send this prompt.

   > Use $paper-draft to help me write the first draft of my paper. Guide me in English.

On first use, the assistant asks what problem you are studying and how you approached it. If the research materials live elsewhere, give it a path it can access and specify the folder where you want the paper saved. For installation locations, see the [OpenAI skills guide](https://learn.chatgpt.com/docs/build-skills).

### Choose your materials and review schedule

Your code, dataset descriptions, experiment configurations and results can live in different folders. Where possible, link each results table to the experiment record that produced it. You can specify read-only folders, directories to skip, the output location and when you want to review drafts.

> My research materials are in `experiments/`. Save generated files in `draft/` and skip `old_manuscript/`. First, check the research question and main experiment with me. Once we agree on an outline, continue drafting. I will review one section at a time.

### From research materials to a first draft

1. Confirm the research question and method, then map the source materials.
2. Prepare Chinese and English technical reports and check results against their sources.
3. Optionally select sample papers to guide writing and figure design.
4. Prepare a venue-specific or provisional LaTeX template. Test its sections, figures and citations in the editor or compiler you plan to use.
5. Propose an outline that identifies the question each section answers and the evidence behind it.
6. Choose a drafting order. The default is to start with the results.
7. Draft the text, check citations and tables, and prepare figures from experimental records. Keep editable figure sources and plotting scripts.
8. Read the manuscript in order, check numbers, citations and figure references, and deliver the editable draft with any facts that still need the author's attention.

You can refine the text before making figures or supply your own figures for integration. When you resume work, `paper_state.md` in the paper workspace records the current stage, your choices and the next action.

### What was tested

In one research project, the workflow took an initial research description through to a 13-page English draft with two figures and eight tables. The built-in compiler in the tested Linux desktop environment successfully compiled the multi-file LaTeX project. Other editors and fresh installations need their own dependency and preview checks. The author reviews the interpretation of the results, what each citation supports and any unresolved facts.
