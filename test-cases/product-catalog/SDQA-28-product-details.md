# SDQA-28: SauceDemo | Product Catalog | Navigate to product details page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-28 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-21](../../user-stories/SDQA-21-product-catalog.md) (covers "Individual Product Page" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-31](../../preconditions/SDQA-31-catalog-page.md): User is located on the product catalog page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks on the name or image of a specific product (e.g., Sauce Labs Backpack). | User is redirected to the single product detail page (`/inventory-item.html?id=X`). |
| 2 | User verifies that the product details displayed on the product detail page. | The displayed product information matches the image, name, price, and description that were displayed for that product on the catalog page (`/inventory.html`). An "Add to cart" button is visible. |