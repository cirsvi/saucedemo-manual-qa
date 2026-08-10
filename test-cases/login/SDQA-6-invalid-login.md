# SDQA-6: SauceDemo | Login | Input invalid credentials

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-6 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-login.md) (covers "Invalid Login" AC) |


## Preconditions
- [SDQA-4](../../preconditions/SDQA-4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User enters invalid username (such as ‘standard_user1’) into the username. | Username field displays entered username (e.g., ‘standard_user1’). |
| 2 | User enters invalid password (such as 'secret_sauce1') into the password field. | Password field displays masked password (e.g., ‘*******’) matching the length of the entered password. |
| 3 | User clicks the "Login" button. | The error message "Username and password do not match any user in this service" is displayed. Both input fields are highlighted in red. User is not redirected to the `/inventory.html`. |