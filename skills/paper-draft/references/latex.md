# LaTeX editing and reliable delivery

Read during template preparation, when the editing environment changes, or when
compilation or preview fails. Reuse the verified route during normal drafting.

## Establish the actual entry point

Use the author's existing editor and project choice when known. Inspect available
tool descriptions to learn whether that surface accepts a local project,
standalone source, or an externally compiled PDF. Local, remote and cloud routes
may differ. A filesystem mount's appearance alone does not prove which route the
host will use. Test the intended entry point before describing it as supported.

When local project compilation is supported, maintain one project directory with
an explicit main file, supporting sections, ordinary figure exports and the
bibliography. Use project-relative paths. Preserve an existing project's layout
and venue template. For a new project, use the host's project-creation tool when
available; do not recreate an existing project or replace the author's sources.
Resolve main-file ambiguity from existing project instructions first; ask only
when the intended entry remains ambiguous.

For Codex/Work hosts exposing these capabilities, `create_latex_project` creates
a new local project, `compile_latex_document` checks its main file, and
`open_in_codex` opens it for editing. Read their current schemas before use. These
tools are optional host adapters, not requirements for using this skill. Other
editors and command-line compilers are suitable when they match the chosen route.

## Validate the dependencies the paper will use

Check a small representative template through the intended editor/compiler:
math, a table, cross-references, a citation using the chosen bibliography system,
and an external figure when images will be part of the paper. Include a section
file if the project uses separate sections. A clearly labelled diagnostic image
is acceptable for this check; it is not a research result or a final figure.
An already-existing manuscript can serve as the check instead of creating a
second document. Recheck after adding dependencies or changing the template.

Inspect diagnostics for missing sources, styles, bibliography support and image
files. Confirm the compiler actually succeeded on the saved current source.
Opening a tab is a separate action. Some viewers retain the last successful PDF
after a later failure, so the visible page alone does not prove freshness.

## Diagnose without damaging a valid project

- **Source or missing-file error:** use the named location and actual project
  contents to fix the source or dependency path. A file present in the project
  but absent in the compiler can indicate a standalone-only route. Recheck that
  route before rewriting the manuscript.
- **Compiler, package download, cache or network failure:** record the diagnostic
  and use supported host setup or an available alternate compiler. An installed
  terminal TeX distribution does not necessarily configure the native editor.
  Do not turn a particular user's cache path, bundle version, application binary
  or manual runtime modification into a universal skill prerequisite.
- **Busy or stale project:** follow the tool's bounded retry guidance.
- **Unknown status or unavailable diagnostics:** retain the source and report
  that this entry point is unverified. Retry only when new evidence or a changed
  state makes it useful; do not alter valid TeX or loop indefinitely to obtain a
  success response. Follow any more specific tool retry limits.

A skill can choose a compatible route and detect failure early; it cannot
guarantee that every host compiler or dependency service is available.

## Use a fallback that preserves the paper

If only standalone compilation is available, a small document may use a
self-contained source. For a project whose figures, styles or bibliography do
not fit that route, retain the normal project and provide a verified PDF from an
available compiler, with concise build instructions. Explain the editor
limitation and continue writing work that does not depend on it.

Do not routinely rasterize vector figures, encode research images in TeX
primitives, or invent a new compiler workaround to satisfy a restricted preview.
If a generated compatibility copy is useful and verified, identify the maintained
source, regeneration process and how edits return to it. Check that scientific
content and references agree; avoid silently maintaining two divergent drafts.

Record only the useful delivery facts in the paper workspace: project root and
main file, editing route, date and result for the current source, PDF build status,
and whether the live preview was actually observed. Keep detailed diagnostics in
a separate log when needed. A success from another compiler is a useful fallback,
not proof that the native editor succeeded.
