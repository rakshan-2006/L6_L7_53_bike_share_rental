# Bike Share Rental – Lab 6

A Python-based Bike Share Rental application used to practice **Code Coverage and Branch Coverage** analysis through automated testing with `pytest` and `coverage.py`.

## Features

- Ride cost calculation based on bike type, duration and subscription.
- Dock availability and status checking.
- Bike unlocking eligibility based on age, account balance and active rides.
- Automated tests for normal cases, edge cases and decision branches.
- Code and branch coverage analysis.

## Project Structure

```text
L6_L7_53_bike_share_rental/
│
├── LAB6/
│   ├── bike_share_rental.py
│   ├── test_bike_share_rental.py
│   ├── CodeCoverageTest_bike_share_rental_application.py
│   ├── BranchCoverageTest_bike_share_rental_application.py
│   │
│   └── evidence/
│       ├── Code_Coverage_Terminal.png
│       └── Branch_Coverage_Terminal.png
│
└── .gitignore
```

## Technologies Used

- Python 3
- pytest
- coverage.py

## Setup and Execution

Install dependencies:

```bash
pip install pytest coverage
```

Navigate to the LAB6 directory:

```bash
cd LAB6
```

### Code Coverage

```bash
coverage run --source=bike_share_rental -m pytest CodeCoverageTest_bike_share_rental_application.py
coverage report -m
```

### Branch Coverage

```bash
coverage erase
coverage run --branch --source=bike_share_rental -m pytest BranchCoverageTest_bike_share_rental_application.py
coverage report -m
```

## Test Results

| Metric | Achieved |
|---|---:|
| Code Coverage | 100% |
| Branch Coverage | 100% |
| Statements Missed | 0 |
| Partial Branches | 0 |

## Objective

To understand the difference between code coverage and branch coverage, identify untested execution paths, and improve software test completeness through systematic test case design.
