# SDQA-43: SauceDemo | Shopping Cart | Remove product from Product Detail Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-43 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-35](../../user-stories/SDQA-35-add-to-cart.md) (covers "Remove Item" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-38](../../preconditions/SDQA-38-product-details.md): User is on a product detail page.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks "Remove" button. | The button "Remove" is replaced with "Add to cart" button. |
| 2 | User observes the cart icon in the top right corner. | Cart icon displays the counter with the correct item count (e.g., from 2 to 1). If the count is 0, the counter badge disappears. |