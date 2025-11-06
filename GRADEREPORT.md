# Grading Report

**Final Grade: 4.00/10.00**

## Rubric

| Criterion | Points |
|-----------|--------|
| `extract_data` correctly slices, title-cases names, int conversion, extracts grades, and leaves input untouched | **1** |
| `curve_grades` applies the curve (while loop) and caps values at 100 | **1.5** |
| `print_top_performers` prints only qualifying `Name: Score` lines (>= 95) | **1.5** |
| Code quality (required loop choices, clear logic) | **0** |

## General Comments

Major syntax and logic errors prevent the script from running: fix record parsing in extract_data (use rec.split(':'), call .title() and int() with parentheses, and move the return outside the loop), then implement a proper while-loop in curve_grades with an initialized index and clamp logic. Also correct print_top_performers to iterate over names/grades and print exactly "Name: Score" using a proper f-string.

## Functionality

- tests/test_grader.py::RosterHelperTests::test_curve_grades_values_and_clamping: Failed (0.0 points)
