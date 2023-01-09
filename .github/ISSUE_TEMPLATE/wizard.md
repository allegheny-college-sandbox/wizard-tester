---
name: Wizard
about: Template for Wizard reports
title: Assignment Progress
labels: bug
assignees: ''

---

# `TODO`s

{{#checks}}
{{#todos}}
Based on the GatorGrader report for this run, here's a summary of what you've got left to do.
{{/todos}}
{{/checks}}

{{#checks}}
{{^todos}}
The latest run of the GatorGrader on this assignment says you've finished all the tasks!
{{/todos}}
{{/checks}}

{{#checks}}
{{#category}}
## {{category}}

{{#specifications}}
{{#description}}
- [{{#status}}x{{/status}}{{^status}} {{/status}}] {{.}}
{{/description}}
{{/specifications}}
{{/category}}

{{/checks}}

## Percent complete

Based on the checks achieved, this assignment is `{{#checks}}{{pct}}{{/checks}}%` complete.
