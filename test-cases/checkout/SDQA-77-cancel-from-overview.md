# SDQA-77: SauceDemo | Checkout | Cancel from Overview Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-77 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Cancel from Overview Page" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-78](../../preconditions/SDQA-78-on-checkout-overview.md): User is on the checkout overview page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates "<- Cancel" button in the bottom left corner and clicks it. | The user is redirected to the Product Catalog page (`/inventory.html`). |