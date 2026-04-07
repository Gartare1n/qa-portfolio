[Registration / Login]

- Submit empty phone field -> validation error displayed
- Enter phone number with fewer digits than required -> validation error displayed
- Enter phone number more than allowed length -> validation error displayed
- Enter invalid phone number format -> validation error displayed
- Enter valid phone number -> accepted successfully

- Submit empty email/password fields -> validation errors displayed
- Login with non-existing user -> error message displayed
- Login with valid email and valid password -> user logged in
- Login with valid email and invalid password -> error message displayed
- Login with invalid email and valid password -> error message displayed
- Login with invalid email and invalid password -> error message displayed
- Login field is not vulnerable to SQL injection (e.g. ' OR '1'='1)

- Error message text is displayed and readable
- Password field is case-sensitive (Caps Lock handling)
- Leading/trailing spaces in input fields are handled correctly
- Password field is not vulnerable to SQL injection (e.g. ' OR '1'='1)

- "Forgot password" flow is accessible
- Password reset flow works correctly
- Verification code resend functionality works

[Catalogue]

- Product list loads successfully
- Infinite scroll loads new products without duplicates
- Product card displays correct name, price, and image
- Clicking product opens product page

- Add product to favorites as guest -> login popup appears
- Close login popup -> favorite button remains functional
- Add product to favorites as logged-in user -> product saved

- Sorting updates product list correctly
- Filters apply correctly
- Filters reset correctly

[Product Page]

- Product page loads correctly
- Product name, price, and availability displayed correctly

- Product images load and can be switched
- Image gallery works without UI issues

- Add product to cart -> product added successfully
- Buy product in installments -> flow is accessible and works

- Add product to favorites -> product saved correctly
- Add product to compare -> product added to comparison list

- Installment options can be expanded and scrolled
- Additional product options can be selected

- "All products by this company" button works
- "About" and "Characteristics" tabs display correct content

- Navigation via suggested/recommended products works
- Switching between "Reviews" and "Questions" tabs updates content

- "Write a review" button is clickable and functional
- Upload additional materials works correctly

- Navigation via "Recently viewed" products works

[Cart]

- Product is added to cart successfully
- Cart displays correct product name, price, and quantity

- Increasing/Decreasing product quantity updates total price
- Quantity cannot be less than minimum allowed (<1)
- Quantity cannot exceed maximum allowed limit (>99999)
- Manual input validates numeric values only
- Special characters in quantity input are rejected

- Adding additional services updates total price correctly or handled as per logic

- Product can be removed from cart
- Cart updates correctly after item removal

- "Continue shopping" button redirects to catalogue page
- "Checkout" button redirects to checkout page
