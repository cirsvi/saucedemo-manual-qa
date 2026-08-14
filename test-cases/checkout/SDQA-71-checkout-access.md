# SDQA-71: SauceDemo | Checkout | Access from Cart Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-71 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Access Checkout from Cart" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-67](../../preconditions/SDQA-67-on-cart-page.md): User is located on the cart page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates "Checkout" button in the bottom right corner and clicks it. | The user is redirected to the "Checkout: Your Information" Page (`/checkout-step-one.html`). |