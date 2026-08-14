# SDQA-125: SauceDemo | Checkout | UX |  Checkout "First Name" field accepts infinite amount of characters

| Attribute          | Value |
|--------------------|-------|
| **Bug ID**         | SDQA-125 |
| **Priority**       | Low |
| **Severity**       | Low |
| **Build Version**  | V1.0 |
| **Environment**    | PROD |
| **Linked Test Case** | [SDQA-101](../../test-cases/checkout/SDQA-101-firstname-max-length.md) – SauceDemo \| Checkout \| Server-side: First name input really long string |

## Preconditions:
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-75](../../preconditions/SDQA-75-on-checkout-information.md): User is on the checkout information page.

## Steps & Results:

| Action | Expected Result | Actual Result |
|--------|-----------------|---------------|
| User inputs a really long string (e.g., letter a 200+ times) into the "First Name" input field. |The "First Name" input field displays entered string (e.g., letter a 200+ times). | - |
| User enters a valid Last Name (e.g., Doe) into the "Last Name" input field. |The "Last Name" input field displays the entered name (e.g., Doe). | - |
| User enters a valid Zip/Postal Code (e.g., LV0000) into the "Zip/Postal Code" input field. | The "Zip/Postal Code" input field displays the entered ZIP code (e.g., LV0000). | - |
| User clicks the "Continue" button in the bottom right corner. | The server rejects the request and displays an error message: "First Name must be under 50 characters." and the input field is highlighted in red color. | The "First Name" input of long string is accepted and the User is redirected to the "Checkout: Overview" page; no error message displayed (see video in Attachments). |

## Device Under Test (DUT):
- **DEVICE:** HP Victus 15 
- **OS:** Windows 11 Home, 25H2
- **BROWSER:** Google Chrome Version 150.0.7871.46

## Reproducibility & Account:
**Reproducibility:** 5/5 (consistently reproducible)
**Account used for testing:**  standard_user (password: secret_sauce)

## Attachments:
![First name with long input](../../evidence/firstname_long_input.gif)