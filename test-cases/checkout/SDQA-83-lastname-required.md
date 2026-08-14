# SDQA-83: SauceDemo | Checkout | Server-side: Last name is required input field

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-83 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Validation - Last Name is Required" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-75](../../preconditions/SDQA-75-on-checkout-information.md): User is on the checkout information page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User enters a valid First Name (e.g., Jane) into the "First Name" input field. | The "First Name" input field displays the entered name (e.g., Jane). |
| 2 | User leaves "Last Name" input field empty. | The "Last Name" field is empty. |
| 3 | User enters a valid Zip/Postal Code (e.g., LV0000) into the "Zip/Postal Code" input field. | The "Zip/Postal Code" input field displays the entered ZIP code (e.g., LV0000). |
| 4 | User clicks the "Continue" button in the bottom right corner. | The input field is highlighted in red color and an error message "Last Name is required" is displayed in a red box below all the input fields. The user remains on the "Checkout: Your information" page. |