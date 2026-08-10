# Test Scenarios – SauceDemo Web Application

## 1. Login

1. Verify that a user can log in with valid credentials.
2. Verify login behavior when the username field is blank.
3. Verify login behavior when the password field is blank.
4. Verify login behavior when spaces are entered in the username field.
5. Verify login behavior when spaces are entered in the password field.
6. Verify login using credentials containing numbers and special characters.
7. Verify that an appropriate error message is displayed when a user attempts to log in with invalid credentials.
8. Verify that the user is redirected to the Products page after successful login.
9. Verify that the user remains on the Login page after unsuccessful login.
10. Verify that the password is masked when entered.

## 2. Product Listing

1. Verify that all available products are displayed on the Products page.
2. Verify that products can be sorted by name.
3. Verify that products can be sorted by price from high to low.
4. Verify that products can be sorted by price from low to high.
5. Verify that the Add to Cart button adds the selected product to the cart.
6. Verify that clicking a product name redirects the user to the Product Details page.
7. Verify that the correct product image is displayed for each product.
8. Verify that the correct price is displayed for each product.
9. Verify that the shopping cart count is updated when a product is added.
10. Verify that clicking Back to Products from the Product Details page redirects the user to the Products page.

## 3. Product Details

1.Verify that the user is redirected to the correct Product Details page when a product is selected
2. Verify that the correct product image is displayed.
3. Verify that the correct product price is displayed.
4. Verify that the Add to Cart button is displayed.
5. Verify that clicking Add to Cart adds the selected product to the shopping cart.
6. Verify that the Remove button is displayed after the product is added to the shopping cart.
7. Verify that clicking Back to Products redirects the user to the Products page.
8. Verify that the correct product description is displayed.

## 4. Shopping Cart

1. Verify that all selected products are added to the shopping cart.
2. Verify that the correct quantity is displayed for each added product.
3. Verify that the correct price is displayed for each added product.
4. Verify that the Remove button is displayed for each product.
5. Verify that clicking Continue Shopping redirects the user to the Products page.
6. Verify that clicking Checkout redirects the user to the Checkout page.
7. Verify that the shopping cart badge displays the correct number of added products.
8. Verify that the cart badge count is updated when a product is removed.
9. Verify that removing all products results in the expected empty cart behavior.
10. Verify that each selected product retains its correct name, price, and quantity when multiple products are added to the cart.

## 5. Checkout & order Completion

1. Verify that clicking Checkout redirects the user to the Checkout Information page.
2. Verify that an appropriate error message is displayed when a mandatory field is left blank.
3. Verify that the user cannot continue when the First Name field is blank.
4. Verify that the user cannot continue when the Last Name field is blank.
5. Verify that the user cannot continue when the Postal Code field is blank.
6. Verify that clicking Cancel redirects the user to the Shopping Cart page.
7. Verify that clicking Continue redirects the user to the Checkout Overview page.
8. Verify that correct order details are displayed on the Checkout Overview page.
9. Verify that product and pricing information on the Checkout Overview page matches the selected items in the Shopping Cart.
10. Verify that the user can successfully complete the checkout process.
11. Verify that an appropriate confirmation message is displayed after clicking Finish.
12. Verify that clicking Back to Home redirects the user to the Products page.
13. Verify that clicking the Generate PDF button generates a valid PDF containing the correct order details.
14. Verify that the order details in the generated PDF match the order details displayed on the Checkout Overview page.
