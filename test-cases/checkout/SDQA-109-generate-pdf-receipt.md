# SDQA-109: SauceDemo | Checkout | Generate PDF order receipt

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-109 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) (covers "Generate PDF Order Receipt" AC) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-107](../../preconditions/SDQA-107-completed-purchase.md): User has successfully completed a purchase.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks on the "Generate PDF order" button in the bottom center of the page. | The download of the PDF order receipt starts. |