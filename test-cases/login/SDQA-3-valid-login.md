# SDQA-3: SauceDemo | Login | Input valid credentials

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-3 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-login.md) (covers "Valid Login" AC) |


## Preconditions
- [SDQA-4](../../preconditions/SDQA-4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User enters valid username (such as 'standard_user') into the username field. | Username field displays entered username (e.g., 'standard_user'). |
| 2 | User enters valid password (such as 'secret_sauce') into the password field. | Password field displays masked password (e.g., '*******') matching the length of the entered password. |
| 3 | User clicks the "Login" button. | User is redirected to the inventory page (`/inventory.html`) and the product list is displayed. |