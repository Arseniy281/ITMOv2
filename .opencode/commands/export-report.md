---
description: Generate summary report from practice results and optional artifacts.
handoffs: []
---

## User Input

```text
$ARGUMENTS
```

You **MUST** consider the user input before proceeding (if not empty).

## Execution

This command invokes the Python script to generate the report according to the spec.

- Args:
  - `--format`: `md` or `html`
  - `--include-artifacts`: include prompts.md and REPORT.md
  - `--metrics-only`: exclude artifacts

### Run

```
python3 scripts/export_report.py --format md --include-artifacts
```

To generate HTML instead:

```
python3 scripts/export_report.py --format html --metrics-only
```

### Output

The script prints the result summary and writes the report to `reports/report-YYYY-MM-DD.{md|html}`.
