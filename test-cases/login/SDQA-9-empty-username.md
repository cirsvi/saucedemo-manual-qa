# SDQA-9: SauceDemo | Login | Empty username field

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-9 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-Login.md) (covers "Username Empty" AC) |


## Preconditions
- [SDQA-4](../../preconditions/SDQA4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User skips username field and types in password into the password field. | Password field displays masked password (e.g., ‘*******’) matching the length of the entered password. |
| 2 | User clicks the "Login" button. | The error message "Username is required" is displayed. Username input field is highlighted in red. User is not redirected to the `/inventory.html`. |