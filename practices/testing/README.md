# Group `practices/testing`

This folder contains the source rules for one technology or engineering practice.
Read [_group.yaml](_group.yaml) first: its name and description define the group's scope, and whenToRead tells agents when to consider its rules.
Keep that metadata current when the group's scope changes.

## Instructions for agents

1. Read the group's metadata before adding or editing a rule. Put guidance here only when it fits that scope.
2. Keep each independently adoptable rule in its own Markdown file. Give it a clear title, reading cue, impact, and impact description.
3. Read each relevant or plausibly relevant rule completely, including its exceptions, before relying on it.
4. Complete unfinished drafts, validate the result, and inspect the changed files before reporting completion.

## Add or edit rules

Run commands from the library root, two directories above this folder.
Use `code-rules library add rule practices/testing/<rule-name>` to add a rule; run `code-rules library add rule --help` for metadata and body options.
Edit existing rule files directly, then run `code-rules library check`. Resolve errors before committing or publishing the library.

A consuming project selects this group in its configuration and runs sync. Its generated/RULES.md identifies the adopted rules after exclusions and replacements.

This README explains authoring; it is not an engineering rule and is not included in generated guidance. Keep group descriptions in _group.yaml.
