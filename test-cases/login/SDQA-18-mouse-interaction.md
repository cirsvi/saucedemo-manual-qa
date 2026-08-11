# SDQA-18: SauceDemo | Login | UX | Mouse interaction

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-18 |
| **Priority**      | Low |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-login.md) |

## Preconditions
- [SDQA-4](../../preconditions/SDQA-4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

**Note:** This test assumes the user has just navigated to the login page and fields are not currently selected or focused.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks on the "Username" input field field. | The "Username" input field is selected and has a visible visual highlight. |
| 2 | User clicks on the "Password" input field field. | The "Password" input field is selected and has a visible visual highlight. |
| 3 | User hovers using mouse over the "Login" button. | The button changes its appearance by a distinct color; the cursor visibly changes to hand to indicate possible action. |