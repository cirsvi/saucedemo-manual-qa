# SDQA-36: SauceDemo | Shopping Cart | Add product from Catalog Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-36 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-35](../../user-stories/SDQA-35-cart-functionality.md) (covers "Add from Catalog Page" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-31](../../preconditions/SDQA-31-catalog-page.md): User is located on the product catalog page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks "Add to cart" button for a chosen product (e.g., "Sauce Labs Backpack"). | The button "Add to cart" is replaced with "Remove" button. |
| 2 | User observes the cart icon in the top right corner. | Cart icon displays the counter with the correct item count (e.g., 1). |