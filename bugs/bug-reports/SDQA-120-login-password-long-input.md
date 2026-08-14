# SDQA-120: SauceDemo | Login | UX |  Login password field accepts infinite number of characters

| Attribute          | Value |
|--------------------|-------|
| **Bug ID**         | SDQA-120 |
| **Priority**       | Low |
| **Severity**       | Low |
| **Build Version**  | V1.0 |
| **Environment**    | PROD |
| **Linked Test Case** | [SDQA-14](../../test-cases/SDQA-14-long-password.md) – SauceDemo \| Login \| Client-side: Password input really long string |

## Preconditions:
- [SDQA-4](../../preconditions/SDQA-4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

## Steps & Results:

| Action | Expected Result | Actual Result |
|--------|-----------------|---------------|
| User inputs a very long string of characters (e.g., 'a' 200+ times) into password field. | The input field prevents the user from typing more than defined limit of characters (e.g., 100). | The " Password" input field accepts infinite amount of characters: ![Password field](../../evidence/password-long-input.png) |

## Device Under Test (DUT):
- **DEVICE:** HP Victus 15 
- **OS:** Windows 11 Home, 25H2
- **BROWSER:** Google Chrome Version 150.0.7871.46

## Reproducibility & Account:
**Reproducibility:** 5/5 (consistently reproducible)
**Account used for testing:**  N/A