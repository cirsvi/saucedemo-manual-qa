# SDQA-11: SauceDemo | Login | Both input fields empty

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-11 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-Login.md) (covers "Both Fields Empty" AC) |


## Preconditions
- [SDQA-4](../../preconditions/SDQA4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User skips both input fields and clicks "Login" button. | The error message "Username is required" is displayed. Both input fields are highlighted in red color. User is not redirected to the `/inventory.html`.|