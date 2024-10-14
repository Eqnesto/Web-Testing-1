# Web Automation 1

This repository contains automated tests for the SwagLabs e-commerce site using Playwright and TypeScript. It follows the Page Object Model (POM) for modular and maintainable test scripts.

## How to Run
1. Install packages:
   ```shell
   npm install
   ```
2. Install Playwright (if needed):
   ```shell
   npx playwright install --with-deps
   ```
3. Run tests:
   ```shell
   npx playwright test --ui
4. View report:
   ```shell
   npx playwright show-report
   ```

## Test Cases
The tests are located in the `tests` directory and cover the following scenarios:

1. **Login Tests**
   - **Invalid User Login**: Verifies error message upon failed login. (Defined in `pages/login.pom.ts`)
   - **Valid User Login**: Verifies successful login and visibility of the inventory page. (Defined in `pages/inventory.pom.ts`)

2. **Filter Tests**
   - **Filter by Name (Z to A)**: Verifies products are sorted in descending order by name.
   - **Filter by Price (Low to High)**: Verifies products are sorted in ascending order by price.

3. **Checkout Tests**
   - **Add Items to Cart**: Verifies items are added to the cart and checks the number and names of added products. (Defined in `pages/checkout-your-info.pom.ts`)
   - **Complete Checkout**: Tests the checkout process, including filling out personal info and verifying products. (Defined in `pages/checkout-overview.pom.ts` and `pages/checkout-complete.pom.ts`)