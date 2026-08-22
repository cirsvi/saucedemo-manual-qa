# SDQA-137: SauceDemo | Login | Closing error message clears message and input highlight

| Field             | Detail |
|-------------------|--------|
| **Test Case ID**  | SDQA-137 |
| **Priority**      | Medium |
| **Requirement / User Story** |  [SDQA-1](../../user-stories/SDQA-1-login.md) (covers "Error Dismissal" AC) |

## Preconditions
- [SDQA-138](../../preconditions/SDQA-138-login-error.md): Login error message is displayed.

## Test Steps
| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | User locates small close (X) button in the upper right corner of the error message box and clicks it. | The error message disappears, the input fields highlighted in red return to their standard (non-error) state. |