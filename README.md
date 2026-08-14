# SauceDemo Manual Testing

This repository contains a manual testing project for the [SauceDemo](https://www.saucedemo.com/) demo e-commerce application.

The testing initially was managed in **Jira** with **Xray Test Management**; however, to ensure the work can be permanently accessed outside of a private Jira setup, the main materials have been converted into Markdown format.

![Browsing test cases in Jira/Xray](evidence/jira-xray/saucedemo_board.gif)

## Execution Summary
The full regression cycle included all **53 test cases**. The smoke cycle covered a critical subset of 9 tests.


| Metric | Smoke | Regression | 
|--------|-------|------------|
| Total | 9 | 53 |
| Passed | 9 | 39 |
| Failed | 0 | 14 |
| Bugs Reported | 0 | 14 |

Xray test plan overview including both test executions:
![Xray test plan report](evidence/jira-xray/test_ex_overview.png)

**Reports:**
- **[Smoke Execution](test-executions/smoke-test-execution.md)**
- **[Regression Execution](test-executions/regression-test-execution.md)**

## Conclusions & Key Defects Found
Defects were clustered primarily in **Checkout** (9) and **Login** (4) features, with only 1 defect in **Product Catalog**. Most of the issues relate to missing input validation, both client-side and server-side, which could introduce data integrity or security vulnerabilities in a production environment.

Additionally, the website doesn't show clear focus indicators when users navigate by keyboard or mouse, making it harder to interact with.

**Example defects:**
- **[SDQA-124](bugs/bug-reports/SDQA-124-empty-cart-checkout.md)**: User can access checkout form with no items in the cart, which allows placing orders with no items.
- **[SDQA-123](bugs/bug-reports/SDQA-123-sort-reset.md)**: When user sorts products by price and refreshes the page, selected sort option resets to the default option.
- **[SDQA-125](bugs/bug-reports/SDQA-125-checkout-firstname-long-input.md)**: The "First Name" input field in Checkout accepts extremely long strings without visible limits. Without proper validation, malformed data can reach the backend.

Full list of bugs: **[Bug Report Overview](bugs/bugs-overview.md)**

## Repository Structure

- **`user-stories/`**: Requirements as user stories with acceptance criteria written in Gherkin format.
- **`preconditions/`**: Reusable setup states.
- **`test-cases/`**: Detailed test cases grouped by feature and an overview.
    - [`tests-overview.md`](test-cases/tests-overview.md) - Full list of test cases by feature.
- **`test-sets/`**: Smoke and regression test sets with ranked test cases.
- **`test-executions/`**: Execution reports with pass/fail results and linked bugs.
- **`bugs/`**: Detailed bug reports with evidence and an overview.
    - [`bugs-overview.md`](bugs/bugs-overview.md) - Full list of bugs by feature.
- **`evidence/`**: Screenshots, GIFs, and Jira/Xray visuals used across the repo.