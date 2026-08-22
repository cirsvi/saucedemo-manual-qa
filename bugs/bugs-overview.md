# Bug Report Overview - SauceDemo

All bug reports below are grouped by feature / user story. Click any ID to open the detailed bug report file with preconditions, steps, expected results, and actual results.

## Login
- User Story (Requirements): [SDQA-1](../user-stories/SDQA-1-Login.md)

| ID | Summary | Priority | Linked Test Case |
|----|---------|----------|------------------|
| [SDQA-118](bug-reports/SDQA-118-login-ux-keyboard.md) | SauceDemo \| Login \| UX \|  Input fields and button lack visible focus indicators for keyboard navigation | Low | [SDQA-16](../test-cases/login/SDQA-16-tab-navigation.md) |
| [SDQA-119](bug-reports/SDQA-119-login-ux-mouse.md) | SauceDemo \| Login \| UX \|  Input fields and button lack visible focus indicators for mouse navigation | Low | [SDQA-18](../test-cases/login/SDQA-18-mouse-interaction.md) |
| [SDQA-120](bug-reports/SDQA-120-login-password-long-input.md) | SauceDemo \| Login \| UX \|  Login password field accepts infinite number of characters | Low | [SDQA-14](../test-cases/login/SDQA-14-long-password.md) |
| [SDQA-121](bug-reports/SDQA-121-login-username-long-input.md) | SauceDemo \| Login \| UX \| Login username field accepts infinite number of characters | Low | [SDQA-13](../test-cases/login/SDQA-13-long-username.md) |

## Logout
- User Story (Requirements): [SDQA-50](../user-stories/SDQA-50-logout.md)

| ID | Summary | Priority | Linked Test Case |
|----|---------|----------|------------------|
| [SDQA-135](bug-reports/SDQA-133-login-error-ui.md) | SauceDemo \| Login \| UI \| Error message text overflows its container and is not fully readable | Low | [SDQA-53](../../test-cases/logout/SDQA-53-protected-pages.md) |

## Product Catalog
- User Story (Requirements): [SDQA-21](../user-stories/SDQA-21-product-catalog.md)

| ID | Summary | Priority | Linked Test Case |
|----|---------|----------|------------------|
| [SDQA-123](bug-reports/SDQA-123-sort-reset.md) | SauceDemo \| Product Catalog \| Applied sorting option resets to default after page refresh | Low | [SDQA-27](../test-cases/product-catalog/SDQA-27-refresh-sort.md) |

## Checkout
- User Story (Requirements): [SDQA-69](../user-stories/SDQA-69-checkout.md)

| ID | Summary | Priority | Linked Test Case |
|----|---------|----------|------------------|
| [SDQA-124](bug-reports/SDQA-124-empty-cart-checkout.md) | SauceDemo \| Checkout \| User can access checkout with an empty cart | Medium | [SDQA-72](../test-cases/checkout/SDQA-72-checkout-not-accessible.md) |
| [SDQA-125](bug-reports/SDQA-125-checkout-firstname-long-input.md) | SauceDemo \| Checkout \| UX \|  Checkout "First Name" field accepts infinite <br>amount of characters | Low | [SDQA-101](../test-cases/checkout/SDQA-101-firstname-max-length.md) |
| [SDQA-126](bug-reports/SDQA-126-checkout-lastname-long-input.md) | SauceDemo \| Checkout \| UX \|  Checkout "Last Name" field accepts infinite <br>amount of characters | Low | [SDQA-102](../test-cases/checkout/SDQA-102-lastname-max-length.md) |
| [SDQA-127](bug-reports/SDQA-127-checkout-zipcode-long-input.md) | SauceDemo \| Checkout \| UX \|  Checkout "Zip/Postal Code" field accepts infinite <br>amount of characters | Low | [SDQA-103](../test-cases/checkout/SDQA-103-zipcode-max-length.md) |
| [SDQA-128](bug-reports/SDQA-128-checkout-firstname-spec-char.md) | SauceDemo \| Checkout \| UX \|  Checkout "First Name" field accepts special characters | Low | [SDQA-89](../test-cases/checkout/SDQA-89-firstname-spec-char.md) |
| [SDQA-129](bug-reports/SDQA-129-checkout-lastname-spec-char.md) | SauceDemo \| Checkout \| UX \|  Checkout "Last Name" field accepts special characters | Low | [SDQA-93](../test-cases/checkout/SDQA-93-lastname-spec-char.md) |
| [SDQA-130](bug-reports/SDQA-130-checkout-zipcode-spec-char.md) | SauceDemo \| Checkout \| UX \|  Checkout "Zip/Postal Code" field accepts special characters | Low | [SDQA-94](../test-cases/checkout/SDQA-94-zipcode-spec-char.md) |
| [SDQA-131](bug-reports/SDQA-131-checkout-ux-mouse.md) | SauceDemo \| Checkout \| UX \|  Input fields and button lack visible focus indicators <br>for mouse navigation | Low | [SDQA-112](../test-cases/checkout/SDQA-112-checkout-mouse-interactions.md) |
| [SDQA-132](bug-reports/SDQA-132-checkout-ux-keyboard.md) |  SauceDemo \| Checkout \| UX \|  Input fields and button lack visible focus indicators <br>for keyboard navigation | Low | [SDQA-113](../test-cases/checkout/SDQA-113-checkout-tab-navigation.md) |