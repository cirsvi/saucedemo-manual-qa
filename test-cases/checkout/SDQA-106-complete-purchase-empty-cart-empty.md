# SDQA-106: SauceDemo | Checkout | Cart is empty after purchase

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-106 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Cart is Empty After Purchase" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-107](../../preconditions/SDQA-107-completed-purchase.md): User has successfully completed a purchase.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User observes the cart icon in the top right corner. | The cart badge is not visible and the cart is empty. |