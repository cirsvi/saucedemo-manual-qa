# SauceDemo | Regression Tests | v1.0 | HP Victus 15 | Windows 11 Home 25H2 | Google Chrome V151.0.7922.108

| Item               | Detail |
|--------------------|--------|
| **Test Set**| [SDQA 20 - Login Regression](../test-sets/regression-login.md), [SDQA 34 - Product Catalog Regression](../test-sets/regression-product-catalog.md), [SDQA 49 - Shopping Cart Regression](../test-sets/regression-cart.md), [SDQA 55 - Logout Regression](../test-sets/SDQA-55-logout-regression.md), [SDQA 110 - Checkout Regression](../test-sets/regression-checkout.md) |
| **Build Version**  | V1.0 |
| **Environment** | PROD |
| **Device** | HP Victus 15  |
| **Operating System**  | Windows 11 Home, 25H2 |
| **Browser**        | Google Chrome Version 150.0.7871.46 |
| **Executed by**    | cirsvi |
| **Date**           | 2026-08-09 |

## Result Summary
- **Total:** 53
- **Passed:** 39
- **Failed:** 14

## Detailed Results by Feature

### Login
| Test ID | Summary | Result | Bug |
|---------|---------|--------|-----|
| [SDQA-3](../test-cases/login/SDQA-3-valid-login.md) | SauceDemo \| Login \| Input valid credentials | PASSED | - |
| [SDQA-6](../test-cases/login/SDQA-6-invalid-login.md) | SauceDemo \| Login \| Input invalid credentials | PASSED | - |
| [SDQA-9](../test-cases/login/SDQA-9-empty-username.md) | SauceDemo \| Login \| Empty username field | PASSED | - |
| [SDQA-10](../test-cases/login/SDQA-10-empty-password.md) | SauceDemo \| Login \| Empty password field | PASSED | - |
| [SDQA-11](../test-cases/login/SDQA-11-empty-input.md) |SauceDemo \| Login \| Both input fields empty | PASSED | - |
| [SDQA-12](../test-cases/login/SDQA-12-locked-out-user.md) | SauceDemo \| Login \| Locked out user | PASSED | - |
| [SDQA-13](../test-cases/login/SDQA-13-long-username.md) | SauceDemo \| Login \| Client-side: Username input really long string | FAILED | [SDQA-121](../bugs/bug-reports/SDQA-121-login-username-long-input.md) |
| [SDQA-14](../test-cases/login/SDQA-14-long-password.md) | SauceDemo \| Login \| Client-side: Password input really long string | FAILED | [SDQA-120](../bugs/bug-reports/SDQA-120-login-password-long-input.md) |
| [SDQA-16](../test-cases/login/SDQA-16-tab-navigation.md) | SauceDemo \| Login \| UX \| Tab navigation | FAILED | [SDQA-118](../bugs/bug-reports/SDQA-118-login-ux-keyboard.md) |
| [SDQA-18](../test-cases/login/SDQA-18-mouse-interaction.md) | SauceDemo \| Login \| UX \| Mouse interaction | FAILED | [SDQA-119](../bugs/bug-reports/SDQA-119-login-ux-mouse.md) |

### Logout
| Test ID | Summary | Result | Bug |
|---------|---------|--------|-----|
| [SDQA-52](../test-cases/logout/SDQA-52-logout.md) | SauceDemo \| Logout \| Successful logout | PASSED | - |
| [SDQA-53](../test-cases/logout/SDQA-53-protected-pages.md) | SauceDemo \| Logout \| Protected pages are inaccessible | PASSED | - |

### Product Catalog
| Test ID | Summary | Result | Bug |
|---------|---------|--------|-----|
| [SDQA-22](../test-cases/product-catalog/SDQA-22-view-catalog.md) | SauceDemo \| Product Catalog \| View product catalog | PASSED | - |
| [SDQA-23](../test-cases/product-catalog/SDQA-23-sort-price-lth.md) | SauceDemo \| Product Catalog \| Sort products by price (low to high) | PASSED | - |
| [SDQA-24](../test-cases/product-catalog/SDQA-24-sort-price-htl.md) |  SauceDemo \| Product Catalog \| Sort products by price (high to low) | PASSED | - |
| [SDQA-25](../test-cases/product-catalog/SDQA-25-sort-name-atz.md) | SauceDemo \| Product Catalog \| Sort products by name (A to Z) | PASSED | - |
| [SDQA-26](../test-cases/product-catalog/SDQA-26-sort-name-zta.md) | SauceDemo \| Product Catalog \| Sort products by name (Z to A) | PASSED | - |
| [SDQA-27](../test-cases/product-catalog/SDQA-27-refresh-sort.md) | SauceDemo \| Product Catalog \| Refresh page preserves applied sort | FAILED | [SDQA-123](../bugs/bug-reports/SDQA-123-sort-reset.md) |
| [SDQA-28](../test-cases/product-catalog/SDQA-28-product-details.md) | SauceDemo \| Product Catalog \| Navigate to product details page | PASSED | - |

### Shopping Cart
| Test ID | Summary | Result | Bug |
|---------|---------|--------|-----|
| [SDQA-36](../test-cases/cart/SDQA-36-add-from-catalog.md) | SauceDemo \| Shopping Cart \| Add product from Catalog Page | PASSED | - |
| [SDQA-37](../test-cases/cart/SDQA-37-add-from-details.md) | SauceDemo \| Shopping Cart \| Add product from Product Details Page | PASSED | - |
| [SDQA-41](../test-cases/cart/SDQA-41-remove-from-catalog.md) | SauceDemo \| Shopping Cart \| Remove product from Catalog Page | PASSED | - |
| [SDQA-43](../test-cases/cart/SDQA-43-remove-from-details.md) | SauceDemo \| Shopping Cart \| Remove product from Product Detail Page | PASSED | - |
| [SDQA-44](../test-cases/cart/SDQA-44-remove-btn-persistance-details.md) | SauceDemo \| Shopping Cart \| Verify "Remove" button appears on Catalog Page after adding from the Product Details Page | PASSED | - |
| [SDQA-45](../test-cases/cart/SDQA-45-remove-btn-persistance-catalog.md) | SauceDemo \| Shopping Cart \| Verify "Remove" button appears on  Product Details Page after adding from the Catalog Page | PASSED | - |
| [SDQA-46](../test-cases/cart/SDQA-46-cart-persistance-refresh.md) | SauceDemo \| Shopping Cart \| Cart state persistence after page refresh | PASSED | - |
| [SDQA-62](../test-cases/cart/SDQA-62-access-cart-catalog.md) | SauceDemo \| Shopping Cart \| Access cart page from Catalog Page | PASSED | - |
| [SDQA-63](../test-cases/cart/SDQA-63-view-cart.md) | SauceDemo \| Shopping Cart \| View items in cart | PASSED | - |
| [SDQA-64](../test-cases/cart/SDQA-64-remove-item-from-cart.md) | SauceDemo \| Shopping Cart \| Remove items from cart | PASSED | - |
| [SDQA-65](../test-cases/cart/SDQA-65-navigate-details-cart.md) | SauceDemo \| Shopping Cart \| Navigate to the Details Page from the cart | PASSED | - |
| [SDQA-66](../test-cases/cart/SDQA-66-cart-continue-shopping.md) | SauceDemo \| Shopping Cart \| Continue shopping | PASSED | - |
| [SDQA-68](../test-cases/cart/SDQA-68-access-cart-details.md) | SauceDemo \| Shopping Cart \| Access cart page from Product Details Page | PASSED | - |

### Checkout
| Test ID | Summary | Result | Bug |
|---------|---------|--------|-----|
| [SDQA-71](../test-cases/checkout/SDQA-71-checkout-access.md) | SauceDemo \| Checkout \| Access from Cart Page | PASSED | - |
| [SDQA-72](../test-cases/checkout/SDQA-72-checkout-not-accessible.md) | SauceDemo \| Checkout \| Checkout button is disabled when cart is empty | FAILED | [SDQA-124](../bugs/bug-reports/SDQA-124-empty-cart-checkout.md) |
| [SDQA-74](../test-cases/checkout/SDQA-74-cancel-from-information.md) | SauceDemo \| Checkout \| Cancel from Information Page |  PASSED | - |
| [SDQA-77](../test-cases/checkout/SDQA-77-cancel-from-overview.md) | SauceDemo \| Checkout \| Cancel from Overview Page |  PASSED | - |
| [SDQA-82](../test-cases/checkout/SDQA-82-successfull-checkout.md) | SauceDemo \| Checkout \| Successful checkout with valid information | PASSED | - |
| [SDQA-81](../test-cases/checkout/SDQA-81-firstname-required.md) | SauceDemo \| Checkout \| Server-side: First name is required input field | PASSED | - |
| [SDQA-83](../test-cases/checkout/SDQA-83-lastname-required.md) | SauceDemo \| Checkout \| Server-side: Last name is required input field | PASSED | - |
| [SDQA-84](../test-cases/checkout/SDQA-84-zipcode-required.md) | SauceDemo \| Checkout \| Server-side: Zip code is required input field | PASSED | - |
| [SDQA-89](../test-cases/checkout/SDQA-89-firstname-spec-char.md) | SauceDemo \| Checkout \| Server-side: First name input does not accept special characters | FAILED | [SDQA-128](../bugs/bug-reports/SDQA-128-checkout-firstname-spec-char.md) |
| [SDQA-93](../test-cases/checkout/SDQA-93-lastname-spec-char.md) | SauceDemo \| Checkout \| Server-side: Last name input does not accept special characters | FAILED | [SDQA-129](../bugs/bug-reports/SDQA-129-checkout-lastname-spec-char.md) |
| [SDQA-94](../test-cases/checkout/SDQA-94-zipcode-spec-char.md) | SauceDemo \| Checkout \| Server-side: Zip Code input does not accept special characters | FAILED | [SDQA-130](../bugs/bug-reports/SDQA-130-checkout-zipcode-spec-char.md) |
| [SDQA-101](../test-cases/checkout/SDQA-101-firstname-max-length.md) | SauceDemo \| Checkout \| Server-side: First name input really long string | FAILED | [SDQA-125](../bugs/bug-reports/SDQA-125-checkout-firstname-long-input.md) |
| [SDQA-102](../test-cases/checkout/SDQA-102-lastname-max-length.md) | SauceDemo \| Checkout \| Server-side: Last name input really long string |  FAILED | [SDQA-126](../bugs/bug-reports/SDQA-126-checkout-lastname-long-input.md) |
| [SDQA-103](../test-cases/checkout/SDQA-103-zipcode-max-length.md) | SauceDemo \| Checkout \| Server-side: Zip code input really long string | FAILED | [SDQA-127](../bugs/bug-reports/SDQA-127-checkout-zipcode-long-input.md) |
| [SDQA-104](../test-cases/checkout/SDQA-104-overview-content.md) | SauceDemo \| Checkout \| Overview page content | PASSED | - |
| [SDQA-105](../test-cases/checkout/SDQA-105-complete-purchase.md) | SauceDemo \| Checkout \| Complete purchase | PASSED | - |
| [SDQA-106](../test-cases/checkout/SDQA-106-complete-purchase-empty-cart-empty.md) | SauceDemo \| Checkout \| Cart is empty after purchase | PASSED | - |
| [SDQA-108](../test-cases/checkout/SDQA-108-return-to-homepage.md) | SauceDemo \| Checkout \| Return back to homepage after purchase | PASSED | - |
| [SDQA-109](../test-cases/checkout/SDQA-109-generate-pdf-receipt.md) | SauceDemo \| Checkout \| Generate PDF order receipt | PASSED | - |
| [SDQA-112](../test-cases/checkout/SDQA-112-checkout-mouse-interactions.md) | SauceDemo \| Checkout \| UX \| Mouse interactions on Information Page | FAILED | [SDQA-131](../bugs/bug-reports/SDQA-131-checkout-ux-mouse.md) |
| [SDQA-113](../test-cases/checkout/SDQA-113-checkout-tab-navigation.md) | SauceDemo \| Checkout \| UX \| Tab navigation on Information Page | FAILED | [SDQA-132](../bugs/bug-reports/SDQA-132-checkout-ux-keyboard.md) |