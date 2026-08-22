# SDQA-104: SauceDemo | Checkout | Overview page content

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-104 |
| **Priority**      | High |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Overview Page Content" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-78](../../preconditions/SDQA-78-on-checkout-overview.md): User is on the checkout overview page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User observes the list of items being purchased. | The page lists all the items being purchased showing quantity, name, description, and price for each item. |
| 2 | User observes the "Payment Information" section. | The section displays "Payment Information" title followed by "SauceCard #31337". |
| 3 | User observes the "Shipping Information" section. | The section displays "Shipping Information" title followed by "Free Pony Express Delivery!". |
| 4 | User observes the "Price Total" section. | The section displays "Item total: $X" followed by "Tax: $X" and "Total: $X", which is a sum of item(s) and applied tax. |