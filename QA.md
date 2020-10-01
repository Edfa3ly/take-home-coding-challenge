QA take home coding challenge guidelines
===============================================

Please organize, design, test, document and deploy your code as if it were
going into production, then send us a link to the hosted repository (e.g.
Github, Bitbucket...).


Cart Business Overview
----------------------

The Edfa3ly shopping cart is your way to submit an order, by adding product URL which has been gotten from any store like Amazon, eBay, etc… to the cart then check out the cart.

There’re two types of stores, automated stores, and non-automated ones.
* Automated stores like (Amazon, eBay, Ralph Lauren, GAP …etc.) by adding product URL from one of these stores, the product details like price, name, color, etc… will be filled automatically in the cart fields.

* Non-automated stores like (Adidas) after adding product URL from one of these stores, the user has to fill all product required details in cart fields.

There’re some prohibited products that we can’t order from our site. Also, there’re some products which take delivery time than the expected to the customer.


Edfa3ly cart functionalities
----------------------------

   1- Adding an item.
   
   2- Editing an item.
   
   3- Deleting an item.
   
Edfa3ly cart rules are
----------------------

   1- User can’t edit the automated details except for the item price with only some stores.
   
   2- Product quantity mustn’t exceed 5.
   
   3- Item URL, name, category, price are required.



Edfa3ly Shopping Cart Link: https://www.edfa3ly.com/cart


Challenge Description
---------------------

1- Write test cases for each of the following scenarios:

*  Adding two automated products, then deleting one of them.
    * https://www.6pm.com/p/product/9409514
    * https://www.shein.com/CUCCOO-The-Everyone-Sneakers-p-1187851-cat-1913.html
    
*  Adding non-automated products, then editing in the products details.
    * https://www.adidas.com/us/nite-jogger-shoes/CG5950.html

2- Write an automation test to simulate the below scenarios functionality.

* Add the below item
    * https://www.6pm.com/p/product/9409514

* Assert the message that will be shown while trying to add the below link
    * https://www.etsy.com/listing/721419995/square-metal-coffee-table-legs-metal?ref=hp_prn&bes=1

  
Expected Deliverables
---------------------

1- Write test cases for the above scenarios.

2- Recommended tool is Selenium WebDriver with any programming language.

3- A documentation of the code workflow is mandatory.

4- Should be executed on Chrome, Firefox and Safari.

5- README file for how to run.
 
How will we review?
-------------------
 
[Guidelines can be found here](README.md)
