# SDQA-62: Sauce Demo | Shopping Cart | Access cart page from Catalog Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-62 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-56](../../user-stories/SDQA-56-cart-management.md) (covers "Access Cart Pagee" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-31](../../preconditions/SDQA-31-catalog-page.md): User is located on the product catalog page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates cart icon in the top right corner and clicks on it. | User is succesfully redirected to the cart page (`/cart.html`). |
