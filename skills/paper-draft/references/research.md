# Research understanding, references, and template

## Brief project map

First obtain or reuse a short research description and material roots. Research sources may be outside the paper workspace. A supplied path still needs to be accessible through the host's permissions; a failed read is not evidence of deletion.

Quietly inspect basic directory organization and representative entry points. Save a short `project_map.md` with material roots and locations of source, configurations, experiment records, results, and existing manuscript artifacts. Record bulky data or checkpoint groups by location, without loading each item. The map is navigation, not a detailed experiment specification.

Only interrupt for severe gaps that prevent initial understanding, such as the entire specified core material being inaccessible with no usable alternative. Defer ordinary run ambiguities to the technical report. Summarize the research problem and approach in a short paragraph and let the author confirm or correct that understanding.

## Complete bilingual technical reports

After basic understanding is confirmed, explain that technical-document preparation is next and begin. Default to `technical_report_zh.md` and `technical_report_en.md` in the paper workspace. Preserve equivalent facts, numbers, and experiment associations across the two languages.

Cover the research as it exists, even material whose use in the paper is undecided. Adapt structure to the research, while covering applicable topics:

- Problem, motivation, hypotheses or research questions, and scope.
- Method, implementation, equations or design decisions, inputs and outputs.
- Data, splits, preprocessing, configurations, and evaluation protocol.
- Main experiments, baselines, ablations, other available experiments, and unsuccessful or incomplete investigations relevant to understanding the record.
- Results, units, aggregation/statistical conventions, and their actual source files.
- Concrete experiment/run associations, existing visualizations, and known limits or unresolved facts.

Inspect code and original result records when needed. Separate verified facts from unknowns, author statements, and interpretations. Do not derive experimental roles or values from a directory name alone. Keep potentially relevant facts here; select manuscript content later.

Produce a useful complete version before asking the author to check it. Bundle consequential factual questions rather than asking permission to inspect each file. Apply corrections to both reports. If a key run later becomes inaccessible, check access and likely relocation before asking the author about movement, deletion, or replacement; update the report's evidence location and the map if a root changed.

## Optional sample papers and style

Ask whether the author wants sample-paper guidance. If not, skip it. If yes, accept uploaded papers, local paths, links, or titles; disambiguate only when necessary. Store acquired papers in a dedicated folder within the paper workspace, or record pointers to existing materials.

If there are no samples, ask only missing information that affects selection: target journal/conference, audience, or length/article type. Do not repeat facts already known from the reports. "Not sure" is acceptable; propose concrete directions based on the research, such as more technical detail, more background explanation, or more emphasis on application. Offer a few candidates and say what each is useful for.

Read the actual paper before claiming to have analyzed its writing. Inspect rendered figures/PDF pages before describing visual style; text extraction alone does not reveal layout, typography, or color.

Keep `writing_style.md` concise and operational. Extract applicable choices rather than completing every category:

- Paragraph development, transitions, and explanation depth.
- Framing and chapter connections useful for this argument.
- Language, terminology, and treatment of uncertainty.
- Method exposition, notation, formula explanation, and placement of detail.
- Results narration and coordination with evidence.
- Figure layout, color semantics, labels, and captions.
- Table grouping, metric order, precision, emphasis, and notes.
- Citation and background organization.

For a useful rule, state its scope, action, source location, and adoption status: author preference, provisional default, or unresolved choice. Keep observations separate from adopted instructions. Common disciplinary conventions are not necessarily an individual paper's style. Do not imitate formula counts, reference counts, paragraph lengths, or figure quantities as quotas.

Different papers may guide different sections. Adapt to the research and venue; use short original illustrations rather than copied passages. Show a compact style summary and meaningful choices, without seeking approval for every observation. Apply these choices in actual drafting and plotting. Update ongoing author preferences, replace superseded rules, and retain a short explanation of material changes. A local sentence edit does not automatically become a global rule.

Judge this module through the resulting prose and figures. If abstract extraction adds little useful guidance or excessive work, simplify it after actual use.

## Template

Support a supplied template, a specified venue's official template, or an agent-selected provisional template. Reuse an earlier venue choice. Retrieve from official author guidance when possible, checking relevant year, article type, and submission versus publication settings. Ask only when an ambiguity affects which template is needed.

Keep needed editable source files and dependencies together in the paper workspace. Remove sample authors, article text, figures, and bibliography entries from the working manuscript; explicitly mark undecided fields as placeholders. Template example headings do not dictate the research outline.

Choose a simple provisional template if the author has no preference. Record its source, version and main file in the workspace notes. Use [the LaTeX guidance](latex.md) to verify the author's editing route and record the result before drafting.
