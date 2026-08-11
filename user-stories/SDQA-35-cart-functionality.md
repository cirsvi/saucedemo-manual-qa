# SDQA-35: As a customer, I want to add products to my cart so that I can purchase them

| Field             | Detail |
|-------------------|--------|
| **Story ID**  | SDQA-35 |
| **Priority**      | High |
| **Story Points** | 3 |

## Test Cases
| ID           | Summary |
|-------------------|--------|
| [SDQA-36](../test-cases/cart/SDQA-36-add-from-catalog.md) | SauceDemo \| Shopping Cart \| Add product from Catalog Page |
| [SDQA-37](../test-cases/cart/SDQA-37-add-from-details.md) | SauceDemo \| Shopping Cart \| Add product from Product Details Page |
| [SDQA-41](../test-cases/cart/SDQA-41-remove-from-catalog.md) | SauceDemo \| Shopping Cart \| Remove product from Catalog Page |
| [SDQA-43](../test-cases/cart/SDQA-43-remove-from-details.md) | SauceDemo \| Shopping Cart \| Remove product from Product Detail Page |
| [SDQA-44](../test-cases/cart/SDQA-44-remove-btn-persistance-details.md) | SauceDemo \| Shopping Cart \| Verify "Remove" button appears on Catalog Page after adding from the Product Details Page |
| [SDQA-45](../test-cases/cart/SDQA-45-remove-btn-persistance-catalog.md) | SauceDemo \| Shopping Cart \| Verify "Remove" button appears on Product Details Page after adding from the Catalog Page |
| [SDQA-46](../test-cases/cart/SDQA-46-cart-persistance-refresh.md) | SauceDemo \| Shopping Cart \| Cart state persistence after page refresh |

## Business Value

Adding a product to the cart is one of the main functionalities, which will further allow customers to purchase items directly, affecting the sales.

## Acceptance Criteria (AC)

### Add from Catalog Page:

*Given* I am on the product catalogue page (`/inventory.html`),
*When* I click the “Add to cart” button  on a product card,
*Then* the cart icon updates to show the new item quantity (e.g., from none to 1, or from 1 to 2) and the “Remove” button replaces the “Add to cart” button on that product card.

### Add from the Product Details Page:

*Given* I am on the product details page (`/inventory-item.html?id=X`),
*When* I click the “Add to cart” button,
*Then* the cart icon updates to show the new item quantity and the “Remove” button replaces the “Add to cart” button on the detail page.

### Global State Consistency:

*Given* I have added an item to the cart from the details page (`/inventory-item.html?id=X`),
*When* I navigate back to the catalogue page, 
*Then* the “Remove“ button is displayed on the product card for that item.

### Remove Item:

*Given* I have at least one item in the cart,
*When* I click the “Remove” button on a product card or product detail page,
*Then* the cart icon updates to show the new item quantity (e.g., from 1 to none, or from 2 to 1) and the “Add to cart” button replaces the “Remove” button.

### Cart Persistence:

*Given* I have item(s) in the cart,
*When* I refresh the page,
*Then* the added items and cart icon quantity remain unchanged.