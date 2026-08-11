# SDQA-21: As a customer, I want to browse through the product catalogue so that I can purchase the products

| Field             | Detail |
|-------------------|--------|
| **Story ID**  | SDQA-21 |
| **Priority**      | High |
| **Story Points** | 3 |

## Test Cases
| ID           | Summary |
|-------------------|--------|
| [SDQA-22](../test-cases/product-catalog/SDQA-22-view-catalog.md) | SauceDemo \| Product Catalog \| View product catalog |
| [SDQA-23](../test-cases/product-catalog/SDQA-23-sort-price-lth.md) | SauceDemo \| Product Catalog \| Sort products by price (low to high) |
| [SDQA-24](../test-cases/product-catalog/SDQA-24-sort-price-htl.md) | SauceDemo \| Product Catalog \| Sort products by price (high to low) |
| [SDQA-25](../test-cases/product-catalog/SDQA-25-sort-name-atz.md) | SauceDemo \| Product Catalog \| Sort products by name (A to Z) |
| [SDQA-26](../test-cases/product-catalog/SDQA-26-sort-name-zta.md) | SauceDemo \| Product Catalog \| Sort products by name (Z to A) |
| [SDQA-27](../test-cases/product-catalog/SDQA-27-refresh-sort.md) | SauceDemo \| Product Catalog \| Refresh page preserves applied sort |
| [SDQA-28](../test-cases/product-catalog/SDQA-28-product-details.md) | SauceDemo \| Product Catalog \| Navigate to product details page |



## Business Value

The product catalogue browsing is the main user experience. Without it, users cannot discover products, which directly impacts sales.

## Acceptance Criteria (AC)

### Page Loads:
*Given* I am on the product catalogue page (`/inventory.html`),
*When* the page loads,
*Then* I see 6 product cards with an image, name, description, price, and an  “Add to cart” button, and the shopping cart icon in the top right corner.

### Sorting by Price:

#### Ascending Order:
*Given* I am on the poduct catalogue page (`/inventory.html`),
*When* I sort products by price (low to high),
*Then* I see product cards ordered by price in ascending order.

#### Descending Order
*Given* I am on the product catalogue page (`/inventory.html`),
*When* I sort products by price (high to low),
*Then* I see product cards ordered by price in descending order.

### Sorting by Name:

#### Ascending Order
*Given* I am on the product catalogue page (`/inventory.html`),
*When* I sort products by their name (Z to A),
*Then* I see product cards ordered by name in alphabetical order from Z to A.

#### Descending Order
*Given* I am on the product catalogue page (`/inventory.html`),
*When* I sort products by their name (A to Z),
*Then* I see product cards ordered by name in alphabetical order from A to Z.

### Refresh the Page:

*Given* I am on the product catalogue page (`/inventory.html`) and have sorted products by price (low to high),
*When* I refresh the page,
*Then* I see that products remain sorted by price (low to high) and the sorting dropdown shows “Price (low to high)”.

### Individual Product Page:

*Given* I am on the product catalogue page (`/inventory.html`),
*When* I click on the product image or name,
*Then* I am redirected to the individual product page (`/inventory-item.html?id=X`) containing the image, name, price, description, and “Add to cart“ button.