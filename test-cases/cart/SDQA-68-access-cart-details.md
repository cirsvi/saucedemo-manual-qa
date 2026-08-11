# SDQA-68: Sauce Demo | Shopping Cart | Access cart page from Product Details Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-68 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-56](../../user-stories/SDQA-56-cart-management.md) (covers "Access Cart Pagee" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-38](../../preconditions/SDQA-38-product-details.md): User is on a product detail page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates cart icon in the top right corner and clicks on it. | User is succesfully redirected to the cart page (`/cart.html`). |
