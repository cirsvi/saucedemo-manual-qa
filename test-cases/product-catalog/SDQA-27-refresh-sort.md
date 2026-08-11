# SDQA-27: SauceDemo | Product Catalog | Refresh page preserves applied sort

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-27 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-21](../../user-stories/SDQA-21-product-catalog.md) (covers "Refresh the Page" AC) |


## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-31](../../preconditions/SDQA-31-catalog-page.md): User is located on the product catalog page.
- [SDQA-33](../../preconditions/SDQA-33-products-sorted.md): User has sorted products by price (low to high).


## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User notes the sort option in the top right corner. | The sorting option in the top right corner under cart icon is set "Price (low to high)"; products are sorted in ascending order by price. |
| 2 | User refreshes the page. | The products remain sorted by price (low to high) and the dropdown still shows the previously selected option "Price (low to high)". |