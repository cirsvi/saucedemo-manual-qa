# SDQA-13: SauceDemo | Login | Client-side: Username input really long string

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-13 |
| **Priority**      | Low |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-login.md) |


## Preconditions
- [SDQA-4](../../preconditions/SDQA-4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User enters a very long string of characters (e.g., 'a' 200+ times) into username field. | The input field prevents the user from typing more than defined limit of characters (e.g., 50). |