# SDQA-69: As a customer, I want to complete the checkout process so that I can finalize my purchase

| Field             | Detail |
|-------------------|--------|
| **Story ID**  | SDQA-69 |
| **Priority**      | High |
| **Story Points** | 3 |

## Test Cases
| ID           | Summary |
|-------------------|--------|
| [SDQA-71](../test-cases/checkout/SDQA-71-checkout-access.md) | SauceDemo \| Checkout \| Access from Cart Page |
| [SDQA-72](../test-cases/checkout/SDQA-72-checkout-not-accessible.md) | SauceDemo \| Checkout \| Checkout button is disabled when cart is empty |
| [SDQA-74](../test-cases/checkout/SDQA-74-cancel-from-information.md) | SauceDemo \| Checkout \| Cancel from Information Page |
| [SDQA-77](../test-cases/checkout/SDQA-77-cancel-from-overview.md) | Sauce Demo \| Checkout \| Cancel from Overview Page |
| [SDQA-82](../test-cases/checkout/SDQA-82-successfull-checkout.md) | SauceDemo \| Checkout \| Successful checkout with valid information |
| [SDQA-81](../test-cases/checkout/SDQA-81-firstname-required.md) | SauceDemo \| Checkout \| Server-side: First name is required input field |
| [SDQA-83](../test-cases/checkout/SDQA-83-lastname-required.md) | SauceDemo \| Checkout \| Server-side: Last name is required input field |
| [SDQA-84](../test-cases/checkout/SDQA-84-zipcode-required.md) | SauceDemo \| Checkout \| Server-side: Zip code is required input field |
| [SDQA-89](../test-cases/checkout/SDQA-89-firstname-spec-char.md) | SauceDemo \| Checkout \| Server-side: First name input does not accept special characters |
| [SDQA-93](../test-cases/checkout/SDQA-93-lastname-spec-char.md) | SauceDemo \| Checkout \| Server-side: First name input does not accept special characters |
| [SDQA-94](../test-cases/checkout/SDQA-94-zipcode-spec-char.md) | SauceDemo \| Checkout \| Server-side: Zip Code input does not accept special characters |
| [SDQA-101](../test-cases/checkout/SDQA-101-firstname-max-length.md) | SauceDemo \| Checkout \| Server-side: First name input really long string |
| [SDQA-102](../test-cases/checkout/SDQA-102-lastname-max-length.md) | SauceDemo \| Checkout \| Server-side: Last name input really long string |
| [SDQA-103](../test-cases/checkout/SDQA-103-zipcode-max-length.md) | SauceDemo \| Checkout \| Server-side: Zip code input really long string |
| [SDQA-104](../test-cases/checkout/SDQA-104-overview-content.md) | SauceDemo \| Checkout \| Overview page content |
| [SDQA-105](../test-cases/checkout/SDQA-105-complete-purchase.md) | SauceDemo \| Checkout \| Complete purchase |
| [SDQA-106](../test-cases/checkout/SDQA-106-complete-purchase-empty-cart-empty.md) | SauceDemo \| Checkout \| Cart is empty after purchase |
| [SDQA-108](../test-cases/checkout/SDQA-108-return-to-homepage.md) | SauceDemo \| Checkout \| Return back to homepage after purchase |
| [SDQA-109](../test-cases/checkout/SDQA-109-generate-pdf-receipt.md) | SauceDemo \| Checkout \| Generate PDF order receipt |
| [SDQA-112](../test-cases/checkout/SDQA-112-checkout-mouse-interactions.md) | SauceDemo \| Checkout \| UX \| Tab navigation on Information Page |
| [SDQA-113](../test-cases/checkout/SDQA-113-checkout-tab-navigation.md) | SauceDemo \| Checkout \| UX \| Tab navigation on Information Page |

## Business Value

The checkout flow is the final step of the user journey and directly impacts revenue. Without it, users cannot complete purchases, making the application unsuitable for e-commerce.

## Acceptance Criteria (AC)

### Access Checkout from Cart:

*Given* that I am on the Cart Page (`/cart.html`) and I have item(s) in the cart,
*When* I click on the “Checkout” button in the bottom right corner,
*Then* I am redirected to the “Checkout: Your Information” Page (`/checkout-step-one.html`)

### Checkout Button Disabled When Cart is Empty:

*Given* that I am on the Cart Page (`/cart.html`) and I have no items in the cart,
*When* I click on the “Checkout” button in the bottom right corner,
*Then* the button is disabled (greyed out) and cannot be clicked

### Cancel from Information Page:

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I click the “<- Cancel” button,
*Then* I am redirected to the Cart page (`/cart.html`)

### Cancel from Overview Page:

*Given* that I am on the “Checkout: Overview” Page (`/checkout-step-two.html`),
*When* I click the “<- Cancel” button,
*Then* I am redirected to the Product Catalog page (`/inventory.html`)

### Successful Checkout with Valid Information:

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I input all needed information (First Name, Last Name, ZIP code) and click the “Continue” button,
*Then* I am redirected to the “Checkout: Overview” Page (`/checkout-step-two.html`)

### Validation - First Name is Required: 

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I do not input “First Name” and click the “Continue” button,
*Then* the error message “First Name is required” is displayed

### Validation - First Name No Special Characters:

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I enter special characters (e.g., “!&!$!@") in the First Name field and click the “Continue” button,
*Then* the field should reject the input, and a hint message appears: "First Name must contain only letters, spaces, and hyphens."

### Validation - First Name Maximum Length:

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I enter a 200-character string in the First Name field and click the “Continue” button and click the “Continue” button,
*Then* the error message is displayed (e.g., “First Name must be under 50 characters.”)

### Validation - Last Name is Required: 

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I do not input “Last Name” and click the “Continue” button,
*Then* the error message “Last Name is required” is displayed

### Validation - Last Name No Special Characters:

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I enter special characters (e.g., “!&!$!@") in the Last Name field and click the “Continue” button,
*Then* the field should reject the input, and a hint message appears: "Last Name must contain only letters, spaces, and hyphens."

### Validation - Last Name Maximum Length:

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I enter a 200-character string in the Last Name field and click the “Continue” button,
*Then* the error message is displayed (e.g., “Last Name must be under 50 characters.”)

### Validation - Zip Code is Required: 

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I do not input “Zip/Postal Code” and click the “Continue” button,
*Then* the error message “ Postal Code is required” is displayed

### Validation - Zip Code No Special Characters:

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I enter special characters (e.g., “!&!$!@") in the ZIP code field and click the “Continue” button,
*Then* the field should reject the input, and a hint message appears: “Zip code must contain only letters and numbers.”

### Validation - Zip Code Maximum Length:

*Given* that I am on the “Checkout: Your Information” Page (`/checkout-step-one.html`),
*When* I enter a 200-character string in the Zip code field and click the “Continue” button,
*Then* the error message is displayed (e.g., “Zip code must be under 10 characters.”)

### Overview Page Content:

*Given* that I am on the “Checkout: Overview” Page (`/checkout-step-two.html`),
*When* I overview the page,
*Then* it displays the payment information, shipping information, and price total (item total and tax)

### Complete Purchase:

*Given* that I am on the “Checkout: Overview” Page (`/checkout-step-two.html`),
*When* I click the “Finish” button,
*Then* I am redirected to the “Checkout: Complete!” page (`/checkout-complete.html`)

### Cart is Empty After Purchase:

*Given* I have successfully completed a purchase,
*When* I observe the cart icon in the top right corner,
*Then* the cart count badge is not shown anymore, and the cart is empty

### Back Home After Purchase:

*Given* that I am on the “Checkout: Complete!” page (`/checkout-complete.html`),
*When* I click the “Back Home” button,
*Then* I am redirected to the Product Catalog page (`/inventory.html`)

### Generate PDF Order Receipt:

*Given* that I am on the “Checkout: Complete!” page (`/checkout-complete.html`),
*When* I click the “Generate PDF order” button,
*Then* a download of “Order Receipt” in PDF file format starts