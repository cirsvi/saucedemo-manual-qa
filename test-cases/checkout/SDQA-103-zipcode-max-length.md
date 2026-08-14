# SDQA-103: SauceDemo | Checkout | Server-side: Zip code input really long string

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-103 |
| **Priority**      | Low |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Validation - Zip Code Maximum Length" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-75](../../preconditions/SDQA-75-on-checkout-information.md): User is on the checkout information page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User enters a valid First Name (e.g., Jane) into the "First Name" input field. | The "First Name" input field displays the entered name (e.g., Jane). |
| 2 | User enters a valid Last Name (e.g., Doe) into the "Last Name" input field. | The "Last Name" input field displays the entered name (e.g., Doe). |
| 3 | User inputs a really long string (e.g., letter a 200+ times) into the "Zip/Postal Code" input field. | The "Zip/Postal Code" input field displays entered string (e.g., letter a 200+ times). |
| 4 | User clicks the "Continue" button in the bottom right corner. | The server rejects the request and displays an error message: "Zip code must be under 10 characters." and the input field is highlighted in red color. |