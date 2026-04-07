[Registration / Login]

Title: Successful login with valid credentials  

Preconditions:
User is registered

Steps:
1. Open login page
2. Enter valid email and password
3. Click "Login"

Expected Result:
User is logged in
User is redirected to account or homepage

***

Title: Login with invalid password  

Preconditions:
User is registered

Steps:
1. Enter valid email
2. Enter incorrect password
3. Click "Login"

Expected Result:
Error message is displayed
User is not logged in

[Catalogue]

Title: Infinite scroll loads new products  

Steps:
1. Open catalogue page
2. Scroll down

Expected Result:
New products are loaded dynamically
No duplicates or empty placeholders

***

Title: Add product to favorites as guest  

Steps:
1. Open catalogue
2. Click "Add to favorites" on product

Expected Result:
Login popup is displayed
Product is not added without authentication

***

Title: Favorite button works after closing login popup  

Steps:
1. Click "Add to favorites"
2. Close login popup
3. Click "Add to favorites" again

Expected Result:
Button remains clickable
Login popup appears again or action proceeds correctly

[Product Page]

Title: Product page loads correctly  

Steps:
1. Open any product page

Expected Result:
Product name, price, and image are displayed
No broken UI elements

***

Title: Add product to cart from product page  

Preconditions:
Product is available

Steps:
1. Click "Buy" button

Expected Result:
Product is added to cart
Cart counter updates

***

Title: Add product to comparison  

Steps:
1. Click "Compare" button

Expected Result:
Product is added to comparison list

[Cart]

Title: Add product to cart and verify details  

Steps:
1. Add product to cart
2. Open cart

Expected Result:
Correct product name, price, and quantity displayed

***

Title: Increase product quantity  

Preconditions:
Product is in cart

Steps:
1. Click "+" button

Expected Result:
Quantity increases by 1
Total price updates correctly

***

Title: Decrease product quantity  

Preconditions:
Quantity > 1

Steps:
1. Click "-" button

Expected Result:
Quantity decreases by 1
Total price updates correctly

***

Title: Remove product from cart  

Steps:
1. Add product to cart
2. Click "Remove"

Expected Result:
Product is removed
Cart is updated

***

Title: Enter invalid quantity value  

Steps:
1. Add product to cart
2. Enter "0" or large value (e.g. 99999)

Expected Result:
System restricts invalid values
Allowed limits are enforced

[Checkout]

Title: Proceed to checkout  

Steps:
1. Open cart
2. Click "Checkout"

Expected Result:
User is redirected to checkout page

***

Title: Submit order with empty required fields  

Steps:
1. Open checkout
2. Leave required fields empty
3. Submit order

Expected Result:
Validation errors are displayed
Order is not created

***

Title: Successful order placement  

Preconditions:
Cart contains product

Steps:
1. Fill all required fields
2. Confirm order

Expected Result:
Order is created successfully
Confirmation message is displayed
