# SDQA-37: SauceDemo | Shopping Cart | Add product from Product Details Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-37 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-35](../../user-stories/SDQA-35-cart-functionality.md) (covers "Add from the Product Details Page" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-38](../../preconditions/SDQA-38-product-details.md): User is on a product detail page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks "Add to cart" button. | The button "Add to cart" is replaced with "Remove" button. |
| 2 | User observes the cart icon in the top right corner. | Cart icon displays the counter with the correct item count (e.g., 1). |