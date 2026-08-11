# SDQA-22: SauceDemo | Product Catalog | View product catalog

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-22 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-21](../../user-stories/SDQA-21-product-catalog.md) (covers "Page Loads" AC) |


## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-31](../../preconditions/SDQA-31-catalog-page.md): User is located on the product catalog page.



## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User scrolls through the product page and observes product cards. | Each product card contains image, name of a product, price, description, and "Add to cart" button; the products are sorted alphabetically from A to Z by default .The shopping cart icon is visible in top right corner. |