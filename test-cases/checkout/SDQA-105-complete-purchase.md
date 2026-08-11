# SDQA-105: SauceDemo | Checkout | Complete purchase

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-105 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Complete Purchase" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-78](../../preconditions/SDQA-78-on-checkout-overview.md): User is on the checkout overview page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks on the "Finish" button in the bottom right corner. | The user is redirected to "Checkout: Complete!" page (`/checkout-complete.html`). |
| 2 | User observes the "Checkout: Complete!" page. | The page displays "Thank you for your order!" message under check icon. |