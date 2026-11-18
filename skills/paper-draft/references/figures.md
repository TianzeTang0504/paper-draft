# Figures for a paper

Work one figure at a time from existing outline plans and manuscript placeholders. Read the figure's purpose, real source materials, selected style rules, and intended manuscript size. Do not start another full figure-planning interview.

At the transition, briefly offer to finish text and citations first if the author has not chosen an order. They may keep placeholders and make figures later, including making them themselves. Reuse an existing decision. After figures are supplied, check the affected captions, references, result descriptions, and layout.

## Choose a suitable editable production method

### Results and experimental images

Generate curves, statistical comparisons, and similar plots from real research results using appropriate plotting tools, such as Matplotlib. Retain the plotting script and source location. If an existing result figure has source code, modify that code and regenerate to clean up log-style titles and apply consistent styling.

For existing experimental images, arrange panels and use appropriate cropping and labels while retaining original scientific content and its source. Use traceable processing and real results, not synthetic image generation to invent observations or modify the apparent experimental outcome. Preserve original materials.

### Method diagrams and pipelines

Prefer editable diagrams. draw.io is the suggested default when suitable: retain a valid `.drawio` source file and export the manuscript figure, usually PDF; a preview or SVG may also be useful. Verify that the actual file can be opened and rendered with available tooling. Do not label a raster image placed inside a diagram file as an editable set of modules.

The author can change modules, labels, arrows, and layout and continue from the same source. Other editable tools are acceptable when preferred or more suitable; a particular website is not required. An agent may generate the native diagram structure directly if it can validate the result, without requiring browser automation for every edit.

Show the mechanism needed for the paper: relevant inputs, core modules, meaningful connections, and outputs. Do not reproduce all function calls, implementation branches, and engineering steps merely because they exist in code. Distinguish stages or relationships when the method requires it, without inventing extra detail.

## Paper figure requirements

- Use short readable method, module, metric, and panel names consistent with the manuscript.
- Remove irrelevant run IDs, parameter encodings, file paths, and experiment dates from visible titles. Preserve times, conditions, and units that have scientific meaning.
- Keep visual text concise; use the caption for necessary reading instructions, setup, and observations. Do not move a log dump into the caption.
- Apply selected sample-paper preferences for layout, color meaning, typography, labels, and captions. Maintain consistency across figures and with template constraints.
- Keep data source and experiment associations in plotting scripts or research records. Preserve necessary comparison conditions in the actual figure/caption.
- Export vector drawings as suitable vector files where possible; keep experimental raster images at adequate quality. Use actual venue requirements for size and format, not a universal assumed resolution.

## Iterate and integrate

1. Use the existing purpose and sources to produce a first version.
2. Inspect the rendered result, then show it to the author for concrete changes.
3. Modify the current figure and source; preserve the author's chosen edits.
4. Save editable source or plotting script and the manuscript export. Replace the placeholder and update its caption and references.
5. Inspect the figure inside the compiled manuscript at intended single- or double-column size: text, legend, lines, arrows, spacing, and panels must remain readable.

After adding the first external image, or changing its format or path, also verify that the author's intended editor/compiler resolves it using the route in [latex.md](latex.md). Preserve the scientific figure's editable source and normal export; do not convert it into a large encoded TeX payload merely to force a standalone preview.

Check numerical and method consistency as well as appearance. If figure content changes the argument, revise the outline and related prose. Do not regenerate unrelated figures or repeat all review work without a concrete reason.
