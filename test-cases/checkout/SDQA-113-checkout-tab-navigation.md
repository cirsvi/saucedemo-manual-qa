# SDQA-113: SauceDemo | Checkout | UX | Tab navigation on Information Page

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-113 |
| **Priority**      | Low |
| **Requirement / User Story** |  [SDQA-69](../../user-stories/SDQA-69-checkout.md) |

## Preconditions
- [SDQA-32](../../preconditions/SDQA-32-logged-in.md): User is logged in as standard_user.
- [SDQA-42](../../preconditions/SDQA-42-has-items.md): User has item(s) in the cart.
- [SDQA-75](../../preconditions/SDQA-75-on-checkout-information.md): User is on the checkout information page.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User presses the "Tab" key twice. | The cursor/focus moves to the "First Name" field. A visual highlight border appears. |
| 2 | User presses the Tab key again (3rd time). | The cursor/focus moves to the "Last Name" field. A visual highlight border appears. |
| 3 | User presses the Tab key again (4th time). | The cursor/focus moves to the "Zip/Postal Code" field. A visual highlight border appears. |
| 4 | User presses the Tab key again (5th time). | The cursor/focus moves to the "<- Cancel" button. The button is visually highlighted. |
| 5 | User presses the Tab key again (6th time). | The cursor/focus moves to the "Continue" button. The button is visually highlighted. |