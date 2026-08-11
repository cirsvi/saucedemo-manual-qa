# SDQA-112: SauceDemo | Checkout | UX | Mouse interactions on Information Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-112 |
| **Priority**      | Low |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-75](../../preconditions/SDQA-75-on-checkout-information.md): User is on the checkout information page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User clicks on the "First Name" input field field. | The "First Name" input field is selected and has a visible visual highlight. |
| 2 | User clicks on the "Last Name" input field field. | The "Last Name" input field is selected and has a visible visual highlight. |
| 3 | User clicks on the "Zip/Postal Code" input field field. | The "Zip/Postal Code" input field is selected and has a visible visual highlight. |
| 4 | User hovers using mouse over the "<- Cancel" button. | The button changes its appearance by a distinct color; the cursor visibly changes to hand to indicate possible action. |
| 5 | User hovers using mouse over the "Continue" button. | The button changes its appearance by a distinct color; the cursor visibly changes to hand to indicate possible action. |