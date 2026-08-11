# SDQA-64: Sauce Demo | Shopping Cart | Remove items from cart

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-64 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-56](../../user-stories/SDQA-56-cart-management.md) (covers "Remove Item from Cart Page" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-67](../../preconditions/SDQA-67-on-cart-page.md): User is located on the cart page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates "Remove" button on the product card of an item of choice (e.g., "Sauce Labs Backpack") and click it. | The product card disappears from the card page instantly (without a full page reload). The cart icon count badge in the top right corner is updated to show the new item count (e.g., from 2 to 1). |
