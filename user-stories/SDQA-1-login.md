# SDQA-1: As a registered customer, I want to log in with my username and password so that I can access the product catalogue

| Field             | Detail |
|-------------------|--------|
| **Story ID**  | SDQA-1 |
| **Priority**      | High |
| **Story Points** | 3 |

## Test Cases
| ID           | Summary |
|-------------------|--------|
| [SDQA-3](../test-cases/login/SDQA-3-valid-login.md) | SauceDemo \| Login \| Input valid credentials |
| [SDQA-6](../test-cases/login/SDQA-6-invalid-login.md) | SauceDemo \| Login \| Input invalid credentials |
| [SDQA-9](../test-cases/login/SDQA-9-empty-username.md) |  SauceDemo \| Login \| Empty username field |
| [SDQA-10](../test-cases/login/SDQA-10-empty-password.md) |  SauceDemo \| Login \| Empty password field |
| [SDQA-11](../test-cases/login/SDQA-11-empty-input.md) |  SauceDemo \| Login \| Both input fields empty |
| [SDQA-12](../test-cases/login/SDQA-12-locked-out-user.md) |  SauceDemo \| Login \| Locked out user |
| [SDQA-13](../test-cases/login/SDQA-13-long-username.md) |  SauceDemo \| Login \| Client-side: Username input really long string |
| [SDQA-14](../test-cases/login/SDQA-14-long-password.md) |  SauceDemo \| Login \| Client-side: Password input really long string |
| [SDQA-16](../test-cases/login/SDQA-16-tab-navigation.md) |  SauceDemo \| Login \| UX \| Tab navigation |
| [SDQA-18](../test-cases/login/SDQA-18-mouse-interaction.md) |  SauceDemo \| Login \| UX \| Mouse interaction |

## Business Value

Allows registered users to access the main functionality of the website: browsing the products and completing the purchase. This is the entry point of the entire application and a critical path for revenue generation.

## Acceptance Criteria (AC)

### Valid Login:
*Given* I am on the [login page](https://www.saucedemo.com/ ),
*When* I enter a valid username and a valid password,
*Then* I should be redirected to the /inventory.html page and see the product list.

### Invalid Login:
*Given* I am on the [login page](https://www.saucedemo.com/ ),
*When* I enter an invalid username or/and invalid password,
*Then* I see the error message “Username and password do not match any user in this service“

### Locked-Out User:
*Given* I am on the [login page](https://www.saucedemo.com/ ),
*When* I enter a locked-out username (locked_out_user) with a valid password,
*Then* I see the error message “Sorry, this user has been locked out.“

### Empty Field Validation:

#### Both Fields Empty
*Given* I am on the [login page](https://www.saucedemo.com/ ),
*When* I leave both the username and password fields empty and click the login button,
*Then* I see the error message “Username is required“

#### Password Empty
*Given* I am on the [login page](https://www.saucedemo.com/ ),
*When* I enter the username but leave the password empty and click the login button,
*Then* I see the error message “Password is required“

#### Username Empty
*Given* I am on the [login page](https://www.saucedemo.com/ ),
*When* I enter the password but leave the username empty and click the login button,
*Then* I see the error message “Username is required“