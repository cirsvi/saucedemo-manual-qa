# SDQA-63: Sauce Demo | Shopping Cart | View items in cart

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-63 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-56](../../user-stories/SDQA-56-cart-management.md) (covers "View Items in Cart" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-67](../../preconditions/SDQA-67-on-cart-page.md): User is located on the cart page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User verifies the cart content. | For the added items, the product list displays item(s) cards with: quantity, name, description, price, "Remove" button. |
