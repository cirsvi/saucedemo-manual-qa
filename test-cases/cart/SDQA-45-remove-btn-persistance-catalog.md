# SDQA-45: SauceDemo | Shopping Cart | Verify "Remove" button appears on Product Details Page after adding from the Catalog Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-45 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-35](../../user-stories/SDQA-35-cart-functionality.md) (covers "Global State Consistency" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-31](../../preconditions/SDQA-31-catalog-page.md): User is located on the product catalog page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks "Add to cart" button for a chosen product (e.g., "Sauce Labs Backpack"). | The button "Add to cart" is replaced with "Remove" button. |
| 2 | User clicks on the name or image on the product card of added item. | User is redirected to the product details page (`/inventory-item.html?id=X`). |
| 3 | User observes the button displayed. | On the product details page, the "Add to cart" button is also replaced with "Remove" button. |