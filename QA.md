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

* Non-automated stores like (Addidas) after adding product URL from one of these stores, the user has to fill all product required details in cart fields.

There’re some prohibited products that we can’t order from our site. Also, there’re some products which take delivery time than the expected to the customer.

The user can pay the whole order once, by choosing to apply the final cost feature (We give him full up-front calculations including shipping price) form the cart. Otherwise, the user can pay shipping fees when receiving.


Edfa3ly cart functionalities
----------------------------

   1- Adding an item.
   
   2- Editing an item.
   
   3- Deleting an item.
   
   4- Applying the final cost or not.

Edfa3ly cart rules are
----------------------

   1- User can’t edit the automated details except for the item price with only some stores.
   
   2- Product quantity mustn’t exceed 5.
   
   3- Item URL, name, category, price are required.



Edfa3ly Shopping Cart Link: https://www.edfa3ly.com/cart


Challenge Description
---------------------

1- Write test cases for each of the following scenarios (BDD technique is preferred):

*  Adding two automated products, then deleting one of them.
    * http://www.amazon.com/dp/B01DBGVB7K/ref=twister_dp_update?ie=UTF8&psc=1
    * http://www.amazon.com/dp/B07MTLF74C/ref=twister_dp_update?ie=UTF8&psc=1
    
*  Adding non-automated products, then editing in the products details.
    * https://www.adidas.com/us/nite-jogger-shoes/CG5950.html

2- Write an automation test to simulate the blew scenarios functionality.

* Adding only two items from the blew list
    * http://www.amazon.com/dp/B01DBGVB7K/ref=twister_dp_update?ie=UTF8&psc=1
    * http://www.amazon.com/dp/B07MTLF74C/ref=twister_dp_update?ie=UTF8&psc=1
    * http://www.amazon.com/dp/B06XK2SVFP/ref=twister_dp_update?ie=UTF8&psc=1
    * http://www.amazon.com/dp/B07C1LPMRQ/ref=twister_dp_update?ie=UTF8&psc=1

* Assert the message that will be shown while trying to add the below link
    * https://www.nike.com/t/air-max-deluxe-se-mens-shoe-TLtmJ0/AO8284-001

  
Expected Deliverables
---------------------

1- Recommended tool is Selenium WebDriver with any programming language.

2- A documentation of the code workflow is mandatory.

3- Should be executed on Chrome, Firefox and Safari (two of them is minimum).

4- README file for how to run.
 
How will we review?
-------------------
 
[Guidelines can be found here](README.md)