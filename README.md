# Web Testing 1

This repository contains automated tests for the [Swag Labs Store](https://www.saucedemo.com) using [Playwright](https://playwright.dev) and TypeScript. It follows the Page Object Model (POM) for modular, maintainable test scripts, with each test including assertions to validate functionality.

## 🔧 How to Run

1. Clone repository:
   ```shell
   git clone https://github.com/Eqnesto/Web-Testing-1
   ```
1. Open repository in [Visual Studio Code](https://code.visualstudio.com/download).
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

## 📄 Test Cases

1. **Login Tests**
   - **Invalid User Login**: Tests error message upon failed login.
   - **Valid User Login**: Tests successful login and visibility of the inventory page.

2. **Filter Tests**
   - **Filter by Name (Z to A)**: Tests products are sorted in descending order by name.
   - **Filter by Price (Low to High)**: Tests products are sorted in ascending order by price.

3. **Checkout Tests**
   - **Add Items to Cart**: Tests items are added to the cart and checks the number and names of added products.
   - **Complete Checkout**: Tests the checkout process, including filling out personal info and verifying products.