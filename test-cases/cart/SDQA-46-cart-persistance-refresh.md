# SDQA-46: SauceDemo | Shopping Cart | Cart state persistence after page refresh

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-46 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-35](../../user-stories/SDQA-35-cart-functionality.md) (covers "Cart Persistence" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-31](../../preconditions/SDQA-31-catalog-page.md): User is located on the product catalog page.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User refreshes the product catalog page (`/inventory.html`). | The page reloads succesfully. |
| 2 | User observes the cart icon in the top right corner. | The cart counter badge displays the correct item count (e.g., 1). |
| 3 | User observes the product card(s) for the item(s) that were previously added (e.g., "Sauce Labs Backpack"). | The "Remove" button is still displayed on the product card (the button did not revert to the "Add to cart" button). |