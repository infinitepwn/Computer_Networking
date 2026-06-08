# Repository Guidelines

## Project Structure & Module Organization

This repository is an Obsidian-style collection of computer networking notes. Top-level Markdown files cover broad layers or review material, such as `网络层.md`, `运输层.md`, and `最后一节课复习.md`. Topic folders group related notes: `概述/` contains introductory concepts, and `物理层/` contains physical-layer notes and exercises. `.obsidian/` stores vault metadata and should only be edited when changing vault behavior. `计算机网络知识点总结.html` appears to be a generated or exported summary; update source Markdown first when possible.

## Build, Test, and Development Commands

There is no application build pipeline. Useful local commands:

- `rg "关键词"`: search notes quickly for a concept or duplicate wording.
- `rg --files -g '*.md'`: list Markdown source files.
- `git status --short`: review changed files before committing.
- `git diff -- '*.md'`: inspect note edits while ignoring unrelated binary or metadata changes.

Open the repository as an Obsidian vault for graph view and wiki-link validation.

## Coding Style & Naming Conventions

Write notes in Markdown using Chinese topic names that match the course vocabulary. Prefer concise headings with `##` and `###`, bullet lists for definitions, and tables for timelines or comparisons. Keep Obsidian wiki links in the form `[[分组交换]]` when linking to another note. Use spaces around English protocol names where readability improves, for example `TCP/IP 协议族`. Avoid renaming files casually because existing wiki links may depend on exact names.

## Testing Guidelines

No automated tests are configured. Before publishing changes, manually check that Markdown renders correctly in Obsidian or a Markdown preview. Verify that new wiki links resolve to real notes, images load, formulas render, and exported HTML is regenerated only when the source notes are complete.

## Commit & Pull Request Guidelines

Recent commits use short Chinese summaries, for example `物理层更新` and `上传笔记`. Follow that style with concise messages that identify the changed topic, such as `更新数据链路层习题`. Pull requests should include a short description, list the chapters or folders changed, mention any new generated files, and note whether Obsidian rendering was checked. Include screenshots only for visual changes such as diagrams, canvas files, or exported HTML.

## Agent-Specific Instructions

Keep edits scoped to requested notes or guide files. Do not modify `.obsidian/`, generated HTML, or image references unless the task explicitly requires it. Preserve user-authored wording where possible and improve structure without changing technical meaning.
