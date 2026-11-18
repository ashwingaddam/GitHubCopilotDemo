<!-- PROJECT-CONTEXT:START -->
<!-- discovery-metadata: cs=0 xaml=1 deps=1 -->

## CSV row totals project context

- UiPath Windows project using Visual Basic expressions; entry point: `CsvRowTotals/Main.xaml`.
- Dependency: `UiPath.System.Activities` 26.10.1.
- The workflow reads a headerless CSV from the current user's Documents folder at `GitHubCopilot\UpdateInputcsv\input.csv`.
- It preserves each input row, appends the invariant-culture sum of its numeric fields as a final column, and overwrites `GitHubCopilot\UpdateInputcsv\output.csv`. The source file is not modified.
- Validation and build pass. Headless `run` currently fails in `WorkflowLoader.GetWorkflowActivity` with a null reference, including on an untouched BlankTemplate scaffold, so runtime output has not been verified in this environment.

<!-- PROJECT-CONTEXT:END -->
