# Lab 6 — Tennis Scoring: Code Coverage

This lab focuses on testing the `tennis_scoring.py` module using line coverage and branch coverage techniques.

## Overview

The test cases cover the following functionalities:

- **Game Scoring:** Normal scores, game wins, deuce, advantage, and invalid negative points.
- **Set Winner:** Undecided sets, two-game leads, and tiebreak scores.
- **Match Status:** Match wins, deciding stages, and matches in progress.
- **Branch Testing:** Boundary conditions and both outcomes of decision statements.

## Results

| Coverage Type | Result |
|---|---:|
| Line (Code) Coverage | **97%** |
| Branch Coverage | **100%** |

Terminal screenshots showing the coverage results are included below.

### Line Coverage

![Line Coverage Results](LAB_6code_coverage_screenshot.png)

### Branch Coverage

![Branch Coverage Results](LAB_6branch_coverage_screenshot.png)

## Files

- `LAB_6_CodeCoverageTest_tennis_scoring.py` — Line coverage tests.
- `LAB6_BranchCoverageTest_tennis_scoring.py` — Branch coverage tests.
- `tennis_scoring.py` — Source module being tested.
- `LAB_6code_coverage_screenshot.png` — Line coverage output.
- `LAB_6branch_coverage_screenshot.png` — Branch coverage output.

## How to Run

Run the following commands from the `lab6` directory.

**Line coverage:**

```bash
coverage run --source=. -m pytest LAB_6_CodeCoverageTest_tennis_scoring.py
coverage report -m
```

**Branch coverage:**

```bash
coverage run --branch --source=. -m pytest LAB6_BranchCoverageTest_tennis_scoring.py
coverage report -m
```

## Conclusion

The test suite exercises the main tennis scoring logic, including boundary cases and decision branches. The reported results are **97% line coverage** and **100% branch coverage**.
