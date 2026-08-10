# SDQA-12: SauceDemo | Login | Locked out user

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-12 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-Login.md) (covers "Locked-Out User" AC) |


## Preconditions
- [SDQA-4](../../preconditions/SDQA4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User enters username of locked out user (such as ‘locked_out_user’) into the username field. | Username field displays entered username (e.g., ‘locked_out_user’). |
| 2 | User enters valid password (such as 'secret_sauce') into the password field. | Password field displays masked password (e.g., ‘*******’) matching the length of the entered password. |
| 3 | User clicks the "Login" button. | The error message "Sorry, this user has been locked out." is displayed. Both input fields are highlighted in red. User is not redirected to the `/inventory.html`. |