# SDQA-65: Sauce Demo | Shopping Cart | Navigate to the Details Page from the cart

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-65 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-56](../../user-stories/SDQA-56-cart-management.md) (covers "Navigate to Detail from Cart Page" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-67](../../preconditions/SDQA-67-on-cart-page.md): User is located on the cart page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks on the name on the product card of an item of choice (e.g., "Sauce Labs Backpack"). | User is redirected to Product Details Page (`/inventory-item.html?id=X`). |
| 2 | User verifies the content on the Product Details page (`/inventory-item.html?id=X`). | The content on the Product Details Page: name, description, price matches the values presented in the Cart Page (`/cart.html`). |
