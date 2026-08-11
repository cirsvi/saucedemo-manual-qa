# SDQA-108: SauceDemo | Checkout | Return back to homepage after purchase

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-108 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Back Home After Purchase" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-107](../../preconditions/SDQA-107-completed-purchase.md): User has successfully completed a purchase.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks on the "Back Home" button. | The user is redirected back to the homepage of the website, the Product Catalog page (`/inventory.html`). |