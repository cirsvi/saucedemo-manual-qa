# SDQA-138: Login error message is displayed

## Description:
The user is on the [login page](https://www.saucedemo.com/ ), an error message is displayed, and one or more input fields is highlighted in red.
- This state can be produced by submitting invalid credentials ([SDQA-6](../test-cases/login/SDQA-6-invalid-login.md)), submitting empty fields ([SDQA-9](../test-cases/login/SDQA-9-empty-username.md), [SDQA-10](../test-cases/login/SDQA-10-empty-password.md), [SDQA-11](../test-cases/login/SDQA-11-empty-input.md)), using locked-out user ([SDQA-12](../test-cases/login/SDQA-12-locked-out-user.md)), or accessing a protected page after logout ([SDQA-53](../test-cases/logout/SDQA-53-protected-pages.md)).