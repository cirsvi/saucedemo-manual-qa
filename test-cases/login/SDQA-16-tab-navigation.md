# SDQA-16: SauceDemo | Login | UX | Tab navigation

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-16 |
| **Priority**      | Low |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-login.md) |

## Preconditions
- [SDQA-4](../../preconditions/SDQA-4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

**Note:** This test assumes the user has just navigated to the login page and fields are not currently selected or focused.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User presses the "Tab" key once. | The cursor/focus moves to the "Username" field. A visual highlight border appears. |
| 2 | User presses the Tab key again (2nd time). | The cursor/focus moves to the "Password" field. A visual highlight border appears. |
| 3 | User presses the Tab key again (3rd time). | The cursor/focus moves to the "Login" button. The button is visually highlighted. |