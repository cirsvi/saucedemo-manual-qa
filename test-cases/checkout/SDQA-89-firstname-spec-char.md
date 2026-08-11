# SDQA-93: SauceDemo | Checkout | Server-side: First name input does not accept special characters

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-93 |
| **Priority**      | Low |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Validation - First Name No Special Characters" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-75](../../preconditions/SDQA-75-on-checkout-information.md): User is on the checkout information page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User inputs a string of special characters (e.g., "@&$^@%") into the "First Name" input field. | The "First Name" input field displays entered string (e.g., "@&$^@%"). |
| 2 | Enter a valid Last Name (e.g., Doe) into the "Last Name" input field. | The "Last Name" input field displays the entered name (e.g., Doe). |
| 3 | Enter a valid Zip/Postal Code (e.g., LV0000) into the "Zip/Postal Code" input field. | The "Zip/Postal Code" input field displays the entered ZIP code (e.g., LV0000). |
| 4 | Click the "Continue" button in the bottom right corner. | The server rejects the request and displays an error message: "First Name must contain only letters, spaces, and hyphens." and the input field is highlighted in red color. |