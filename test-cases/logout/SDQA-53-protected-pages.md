# SDQA-53: SauceDemo | Logout | Protected pages are inaccessible

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-53 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-50](../../user-stories/SDQA-50-logout.md) (covers "Protected Pages After Logout" AC) |


## Preconditions
- [SDQA-54](../../preconditions/SDQA-54-logged-out.md): UUser has successfully logged out.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User enters protected pages URL (e.g., https://www.saucedemo.com/inventory.html). | User is not redirected to entered URL (e.g., product catalog page). The user remains on the login page and the error message "You can only access 'XXX' when you are logged in." is displayed. |
