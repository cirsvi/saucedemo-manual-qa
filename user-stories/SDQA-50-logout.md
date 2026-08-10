# SDQA-50: As a customer, I want to log out of my account so that I can securely terminate my session and prevent unauthorized access

| Field             | Detail |
|-------------------|--------|
| **Story ID**  | SDQA-50 |
| **Priority**      | High |
| **Story Points** | 2 |

## Test Cases
| ID           | Summary |
|-------------------|--------|
| [SDQA-52](../test-cases/logout/SDQA-52-logout.md) | SauceDemo \| Logout \| Successfull logout |
| [SDQA-6](../test-cases/login/SDQA-6-invalid-login.md) | SauceDemo \| Login \| Input invalid credentials |


## Business Value

Logging out is a critical security feature that allows users to safely end their session, especially on shared devices. Without this, user accounts remain vulnerable to unauthorised access.

## Acceptance Criteria (AC)

### Successful Logout:
*Given* I am logged in and the hamburger menu is open,
*When* I click the “Logout” option,
*Then* I am redirected to the [login page](https://www.saucedemo.com/ ), and my session is terminated.

### Protected Pages After Logout:
*Given* I have logged out,
*When* I try to navigate to the catalog page (`/inventory.html`),
*Then* I am redirected back to the login page with the error message “You can only access `/inventory.html` when you are logged in.“