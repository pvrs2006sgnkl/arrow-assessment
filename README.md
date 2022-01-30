1. Checkout the assessment from github ()
2. Locate the folder and run composer install
3. Run the php artisan ser --port=7000
4. Proceed to verify the cart product price calculate via postman
   - endpoint : http://127.0.0.1:8989/api/cart/total
   - method : post
   - payload: json (body param, choose raw option)
    
    sample payload:
    {"products":[{"name":"Product 1","price":"10.00","quantity":5},{"name":"Product 2","price":"39.9","quantity":2},{"name":"Product 3","price":"89.00","quantity":1}],"shipping":"10.00","tax":{"rate":"7.00","shipping_incl":true}}

5. For Api testing via test scripts you can run via command line using 

php artisan test
