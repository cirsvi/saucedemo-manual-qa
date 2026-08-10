# SDQA-52: SauceDemo | Logout | Successfull logout

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-52 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-50](../../user-stories/SDQA-50-logout.md) (covers "Successful Logout" AC) |


## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates a hamburger icon (3 horizontal lines) in the left top corner and clicks on it. | The hamburger icon expands into navigation column with following options: All Items, About, **Logout**, Reset App State. |
| 2 | User clicks on the "Logout" option. | The user gets redirected to the [login page](https://www.saucedemo.com/); the session is terminated. |