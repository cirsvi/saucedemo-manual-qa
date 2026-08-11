# SDQA-72: SauceDemo | Checkout | Checkout button is disabled when cart is empty

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-72 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Checkout Button Disabled When Cart is Empty" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-67](../../preconditions/SDQA-67-on-cart-page.md): User is located on the cart page.
- [SDQA-73](../../preconditions/SDQA-73-no-items-in-cart.md): User has no items in the cart.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates "Checkout" button in the bottom right corner and attempts to click it. | The "Checkout" button is grayed out/disabled and cannot be clicked; the user is not redirected to the "Checkout: Your Information" page (`/checkout-step-one.html`). |