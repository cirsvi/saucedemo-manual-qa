# SDQA-26: SauceDemo | Product Catalog | Sort products by name (Z to A)

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-26 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-21](../../user-stories/SDQA-21-product-catalog.md) (covers "Sorting by Name" AC) |


## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-31](../../preconditions/SDQA-31-catalog-page.md): User is located on the product catalog page.


## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates the sorting dropdown in the top right corner and clicks on it. | Sorting option dropdown is located in the top right corner, under the shopping cart icon; dropdown has a funnel icon. The dropdown contains different options: **Name (Z to A)**, Name (A to Z) (default option), Price (high to low), Price (low to high). |
| 2 | User selects sorting option "Name (Z to A)". | Product catalog updates instantly (no page refresh) and products are ordered by name in alphabetical order from Z to A. |