# SDQA-10: SauceDemo | Login | Empty password field

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-10 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-Login.md) (covers "Password Empty" AC) |


## Preconditions
- [SDQA-4](../../preconditions/SDQA4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User enters username into the username field and skips password field. | Username field displays entered username. |
| 2 | User clicks the "Login" button. | The error message "Password is required" is displayed. Password input field is highlighted in red. User is not redirected to the `/inventory.html`. |