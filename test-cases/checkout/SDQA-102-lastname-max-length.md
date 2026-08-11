# SDQA-102: SauceDemo | Checkout | Server-side: Last name input really long string

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-102 |
| **Priority**      | Low |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Validation - Last Name Maximum Length" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-75](../../preconditions/SDQA-75-on-checkout-information.md): User is on the checkout information page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a valid First Name (e.g., Jane) into the "First Name" input field. | The "First Name" input field displays the entered name (e.g., Jane). |
| 2 | User inputs a really long string (e.g., letter a 200+ times) into the "Last Name" input field. | The "Last Name" input field displays entered string (e.g., letter a 200+ times). |
| 3 | Enter a valid Zip/Postal Code (e.g., LV0000) into the "Zip/Postal Code" input field. | The "Zip/Postal Code" input field displays the entered ZIP code (e.g., LV0000). |
| 4 | Click the "Continue" button in the bottom right corner. | The server rejects the request and displays an error message: "Last Name must be under 50 characters." and the input field is highlighted in red color. |