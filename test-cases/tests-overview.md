# Test Case Overview - SauceDemo

All tests cases below are grouped by feature / user story. Click any ID to open the detailed test case file with preconditions, steps, and expected results.

## Login
- User Story (Requirements): [SDQA-1](../user-stories/SDQA-1-Login.md)

| ID | Summary | Priority |
|----|---------|----------|
| [SDQA-3](login/SDQA-3-valid-login.md) | SauceDemo \| Login \| Input valid credentials | High |
| [SDQA-6](login/SDQA-6-invalid-login.md) | SauceDemo \| Login \| Input invalid credentials | High |
| [SDQA-9](login/SDQA-9-empty-username.md) | SauceDemo \| Login \| Empty username field | Medium |
| [SDQA-10](login/SDQA-10-empty-password.md) | SauceDemo \| Login \| Empty password field | Medium |
| [SDQA-11](login/SDQA-11-empty-input.md) |SauceDemo \| Login \| Both input fields empty | Medium |
| [SDQA-12](login/SDQA-12-locked-out-user.md) | SauceDemo \| Login \| Locked out user | High |
| [SDQA-13](login/SDQA-13-long-username.md) | SauceDemo \| Login \| Client-side: Username input really long string | Low |
| [SDQA-14](login/SDQA-14-long-password.md) | SauceDemo \| Login \| Client-side: Password input really long string | Low |
| [SDQA-16](login/SDQA-16-tab-navigation.md) | SauceDemo \| Login \| UX \| Tab navigation | Low |
| [SDQA-18](login/SDQA-18-mouse-interaction.md) | SauceDemo \| Login \| UX \| Mouse interaction | Low |

## Logout
- User Story (Requirements): [SDQA-50](../user-stories/SDQA-50-logout.md)

| ID | Summary | Priority |
|----|---------|----------|
| [SDQA-52](logout/SDQA-52-logout.md) | SauceDemo \| Logout \| Successful logout | High |
| [SDQA-53](logout/SDQA-53-protected-pages.md) | SauceDemo \| Logout \| Protected pages are inaccessible | High |

## Product Catalog
- User Story (Requirements): [SDQA-21](../user-stories/SDQA-21-product-catalog.md)

| ID | Summary | Priority |
|----|---------|----------|
| [SDQA-22](product-catalog/SDQA-22-view-catalog.md) | SauceDemo \| Product Catalog \| View product catalog | High |
| [SDQA-23](product-catalog/SDQA-23-sort-price-lth.md) | SauceDemo \| Product Catalog \| Sort products by price (low to high) | Medium |
| [SDQA-24](product-catalog/SDQA-24-sort-price-htl.md) | SauceDemo \| Product Catalog \| Sort products by price (high to low) | Medium |
| [SDQA-25](product-catalog/SDQA-25-sort-name-atz.md) | SauceDemo \| Product Catalog \| Sort products by name (A to Z) | Medium |
| [SDQA-26](product-catalog/SDQA-26-sort-name-zta.md) | SauceDemo \| Product Catalog \| Sort products by name (Z to A) | Medium |
| [SDQA-27](product-catalog/SDQA-27-refresh-sort.md) | SauceDemo \| Product Catalog \| Refresh page preserves applied sort | Medium |
| [SDQA-28](product-catalog/SDQA-28-product-details.md) | SauceDemo \| Product Catalog \| Navigate to product details page | High |

## Shopping Cart
- User Story (Requirements): [SDQA-35](../user-stories/SDQA-35-cart-functionality.md), [SDQA-56](../user-stories/SDQA-56-cart-management.md)

| ID | Summary | Priority |
|----|---------|----------|
| [SDQA-36](cart/SDQA-36-add-from-catalog.md) | SauceDemo \| Shopping Cart \| Add product from Catalog Page | High |
| [SDQA-37](cart/SDQA-37-add-from-details.md) | SauceDemo \| Shopping Cart \| Add product from Product Details Page | High |
| [SDQA-41](cart/SDQA-41-remove-from-catalog.md) | SauceDemo \| Shopping Cart \| Remove product from Catalog Page | High |
| [SDQA-43](cart/SDQA-43-remove-from-details.md) | SauceDemo \| Shopping Cart \| Remove product from Product Detail Page | High  |
| [SDQA-44](cart/SDQA-44-remove-btn-persistance-details.md) | SauceDemo \| Shopping Cart \| Verify "Remove" button appears on Catalog Page <br>after adding from the Product Details Page | Medium |
| [SDQA-45](cart/SDQA-45-remove-btn-persistance-catalog.md) | SauceDemo \| Shopping Cart \| Verify "Remove" button appears on  Product Details Page <br>after adding from the Catalog Page | Medium |
| [SDQA-46](cart/SDQA-46-cart-persistance-refresh.md) | SauceDemo \| Shopping Cart \| Cart state persistence after page refresh | Medium |
| [SDQA-62](cart/SDQA-62-access-cart-catalog.md) | SauceDemo \| Shopping Cart \| Access cart page from Catalog Page | High |
| [SDQA-63](cart/SDQA-63-view-cart.md) | SauceDemo \| Shopping Cart \| View items in cart | High |
| [SDQA-64](cart/SDQA-64-remove-item-from-cart.md) | SauceDemo \| Shopping Cart \| Remove items from cart | High |
| [SDQA-65](cart/SDQA-65-navigate-details-cart.md) | SauceDemo \| Shopping Cart \| Navigate to the Details Page from the cart | Medium |
| [SDQA-66](cart/SDQA-66-cart-continue-shopping.md) | SauceDemo \| Shopping Cart \| Continue shopping | Medium |
| [SDQA-68](cart/SDQA-68-access-cart-details.md) | SauceDemo \| Shopping Cart \| Access cart page from Product Details Page | Medium |


## Checkout
- User Story (Requirements): [SDQA-69](../user-stories/SDQA-69-checkout.md)

| ID | Summary | Priority |
|----|---------|----------|
| [SDQA-71](checkout/SDQA-71-checkout-access.md) | SauceDemo \| Checkout \| Access from Cart Page | High |
| [SDQA-72](checkout/SDQA-72-checkout-not-accessible.md) | SauceDemo \| Checkout \| Checkout button is disabled when cart is empty | Medium |
| [SDQA-74](checkout/SDQA-74-cancel-from-information.md) | SauceDemo \| Checkout \| Cancel from Information Page | Medium |
| [SDQA-77](checkout/SDQA-77-cancel-from-overview.md) | SauceDemo \| Checkout \| Cancel from Overview Page | Medium |
| [SDQA-82](checkout/SDQA-82-successfull-checkout.md) | SauceDemo \| Checkout \| Successful checkout with valid information | High |
| [SDQA-81](checkout/SDQA-81-firstname-required.md) | SauceDemo \| Checkout \| Server-side: First name is required input field | High |
| [SDQA-83](checkout/SDQA-83-lastname-required.md) | SauceDemo \| Checkout \| Server-side: Last name is required input field | High |
| [SDQA-84](checkout/SDQA-84-zipcode-required.md) | SauceDemo \| Checkout \| Server-side: Zip code is required input field | High |
| [SDQA-89](checkout/SDQA-89-firstname-spec-char.md) | SauceDemo \| Checkout \| Server-side: First name input does not accept special characters | Low |
| [SDQA-93](checkout/SDQA-93-lastname-spec-char.md) | SauceDemo \| Checkout \| Server-side: Last name input does not accept special characters | Low |
| [SDQA-94](checkout/SDQA-94-zipcode-spec-char.md) | SauceDemo \| Checkout \| Server-side: Zip Code input does not accept special characters | Low |
| [SDQA-101](checkout/SDQA-101-firstname-max-length.md) | SauceDemo \| Checkout \| Server-side: First name input really long string | Low |
| [SDQA-102](checkout/SDQA-102-lastname-max-length.md) | SauceDemo \| Checkout \| Server-side: Last name input really long string | Low |
| [SDQA-103](checkout/SDQA-103-zipcode-max-length.md) | SauceDemo \| Checkout \| Server-side: Zip code input really long string | Low |
| [SDQA-104](checkout/SDQA-104-overview-content.md) | SauceDemo \| Checkout \| Overview page content | High |
| [SDQA-105](checkout/SDQA-105-complete-purchase.md) | SauceDemo \| Checkout \| Complete purchase | High |
| [SDQA-106](checkout/SDQA-106-complete-purchase-empty-cart-empty.md) | SauceDemo \| Checkout \| Cart is empty after purchase | High |
| [SDQA-108](checkout/SDQA-108-return-to-homepage.md) | SauceDemo \| Checkout \| Return back to homepage after purchase | Medium |
| [SDQA-109](checkout/SDQA-109-generate-pdf-receipt.md) | SauceDemo \| Checkout \| Generate PDF order receipt | Medium |
| [SDQA-112](checkout/SDQA-112-checkout-mouse-interactions.md) | SauceDemo \| Checkout \| UX \| Mouse interactions on Information Page | Low |
| [SDQA-113](checkout/SDQA-113-checkout-tab-navigation.md) | SauceDemo \| Checkout \| UX \| Tab navigation on Information Page  | Low |