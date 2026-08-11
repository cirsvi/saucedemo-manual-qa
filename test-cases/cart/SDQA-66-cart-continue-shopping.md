# SDQA-66: Sauce Demo | Shopping Cart | Continue shopping

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-66 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-56](../../user-stories/SDQA-56-cart-management.md) (covers "Continue Shopping" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-67](../../preconditions/SDQA-67-on-cart-page.md): User is located on the cart page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates "<- Continue Shopping" in the left lower corner of the page and clicks it. | The user is redirected to the Product Catalog Page (`/inventory.html`). |
