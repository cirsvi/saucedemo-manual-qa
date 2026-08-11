# SDQA-41: SauceDemo | Shopping Cart | Remove product from Catalog Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-41 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-35](../../user-stories/SDQA-35-cart-functionality.md) (covers "Remove Item" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-31](../../preconditions/SDQA-31-catalog-page.md): User is located on the product catalog page.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks "Remove" button for a chosen product (e.g., "Sauce Labs Backpack"). | The button "Remove" is replaced with "Add to cart" button. |
| 2 | User observes the cart icon in the top right corner. | Cart icon displays the counter with the correct item count (e.g., from 2 to 1). If the count is 0, the counter badge disappears. |