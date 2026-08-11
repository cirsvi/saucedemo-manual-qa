# SDQA-44: SauceDemo | Shopping Cart | Verify "Remove" button appears on Catalog Page after adding from the Product Details Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-44 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-35](../../user-stories/SDQA-35-add-to-cart.md) (covers "Global State Consistency" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-38](../../preconditions/SDQA-38-product-details.md): User is on a product detail page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks "Add to cart" button. | The button "Add to cart" is replaced with "Remove" button. |
| 2 | User clicks on the "Back to products" link in the top left corner. | User is redirected to the product catalog page (`/inventory.html`). |
| 3 | User observes the button displayed for previously added product. | On the catalog page, the "Add to cart" button is also replaced with "Remove" button. |