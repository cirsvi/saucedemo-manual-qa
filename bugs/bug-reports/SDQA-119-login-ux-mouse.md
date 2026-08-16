# SDQA-119: SauceDemo | Login | UX |  Input fields and button lack visible focus indicators for mouse navigation

| Attribute          | Value |
|--------------------|-------|
| **Bug ID**         | SDQA-119 |
| **Priority**       | Low |
| **Severity**        | Low |
| **Build Version**        | V1.0 |
| **Environment**        | PROD |
| **Linked Test Case** | [SDQA-18](../../test-cases/login/SDQA-18-mouse-interaction.md) – Login \| UX \| Mouse interaction |

## Preconditions:
- [SDQA-4](../../preconditions/SDQA-4-on-login-page.md): User is located on the [login page]( https://www.saucedemo.com/).

## Steps & Results:

| Action | Expected Result | Actual Result |
|--------|-----------------|---------------|
| User clicks on the "Username" input field. | The cursor/focus moves to the "Username" field. A visual highlight border appears. | The cursor appears in the “Username” input field, **but there is no visual highlight:** ![Username field](../../evidence/username_field.png) |
| User clicks on the "Password” input field. | The cursor/focus moves to the "Password" field. A visual highlight border appears. | The cursor moves to the “Password” input field, **but there is no visual highlight:** ![Password field](../../evidence/password_field.png) |
| User hovers using mouse over the "Login" button. | The button changes its appearance by a distinct color; the cursor visibly changes to hand to indicate possible action. | **The button does not visually highlight for the user:** ![Login Button](../../evidence/login_hover.gif) |

## Device Under Test (DUT):
- **DEVICE:** HP Victus 15 
- **OS:** Windows 11 Home, 25H2
- **BROWSER:** Google Chrome Version 150.0.7871.46

## Reproducibility & Account:
- **Reproducibility:** 5/5 (consistently reproducible)
- **Account used for testing:**  N/A