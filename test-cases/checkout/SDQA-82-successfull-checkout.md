# SDQA-82: SauceDemo | Checkout | Successful checkout with valid information

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-82 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Validation - Last Name is Required" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-75](../../preconditions/SDQA-75-on-checkout-information.md): User is on the checkout information page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a valid First Name (e.g., Jane) into the "First Name" input field. | The "First Name" input field displays the entered name (e.g., Jane). |
| 2 | Enter a valid Last Name (e.g., Doe) into the "Last Name" input field. | The "Last Name" input field displays the entered name (e.g., Doe). |
| 3 | Enter a valid Zip/Postal Code (e.g., LV0000) into the "Zip/Postal Code" input field. | The "Zip/Postal Code" input field displays the entered ZIP code (e.g., LV0000). |
| 4 | Click the "Continue" button in the bottom right corner. | User is redirected to the "Checkout: Overview" Page (`/checkout-step-two.html`). |