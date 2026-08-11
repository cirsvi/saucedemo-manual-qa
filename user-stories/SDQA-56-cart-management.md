# SDQA-56: As a customer, I want to view and manage my shopping cart so that I can review my selected items before the checkout

| Field             | Detail |
|-------------------|--------|
| **Story ID**  | SDQA-56 |
| **Priority**      | High |
| **Story Points** | 2 |

## Test Cases
| ID           | Summary |
|-------------------|--------|
| [SDQA-62](../test-cases/cart/SDQA-62-access-cart-catalog.md) | Sauce Demo \| Shopping Cart \| Access cart page from Catalog Page |
| [SDQA-63](../test-cases/cart/SDQA-63-view-cart.md) | Sauce Demo \| Shopping Cart \| View items in cart |
| [SDQA-64](../test-cases/cart/SDQA-64-remove-item-from-cart.md) | Sauce Demo \| Shopping Cart \| Remove items from cart |
| [SDQA-65](../test-cases/cart/SDQA-65-navigate-details-cart.md) | Sauce Demo \| Shopping Cart \| Navigate to the Details Page from the cart |
| [SDQA-66](../test-cases/cart/SDQA-66-cart-continue-shopping.md) | Sauce Demo \| Shopping Cart \| Continue shopping |
| [SDQA-68](../test-cases/cart/SDQA-68-access-cart-details.md) | Sauce Demo \| Shopping Cart \| Access cart page from Product Details Page |

## Business Value

The Shopping Cart Page is where users review their selected items before the purchase. Without it, users cannot confirm their order, which directly impacts the checkout experience and revenue.

## Acceptance Criteria (AC)

### Access Cart Page:
*Given* that I am on the Product Catalog Page (`/inventory.html`) or the Product Details Page (`/inventory-item.html?id=X`),
*When* I click on the cart icon in the top right corner,
*Then* I am redirected to the Cart Page (`/cart.html`)

### View Items in Cart:

*Given* that I have item(s) in my cart and I am located on the Cart Page (`/cart.html`),
*When* I view the cart contents,
*Then* I can see a list of added items with their name, description, price, quantity, and “Remove” button for each item

### Remove Item from Cart Page:

*Given* that I have item(s) in my cart and I am located on the Cart Page (`/cart.html`),
*When* I click the “Remove” button for the selected item,
*Then* the selected item is removed from the cart

### Navigate to Detail from Cart Page:

*Given* that I have item(s) in my cart and I am located on the Cart Page (`/cart.html`),
*When* I click on the name of the selected item,
*Then* I am redirected to the Product Details Page (`/inventory-item.html?id=X`)

### Continue Shopping:

*Given* I am on the Cart Page (`/cart.html`),
*When* I click on the button “Continue Shopping”
*Then* I am redirected back to the Product Catalog Page (`/inventory.html`)