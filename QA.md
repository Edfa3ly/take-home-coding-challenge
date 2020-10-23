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

There’re some prohibited products that we can’t order from our site.

Edfa3ly cart functionalities
----------------------------

   1. Adding an item.
   1. Editing an item.
   1. Deleting an item.
   
Edfa3ly cart rules are
----------------------
   1. User can’t edit the automated details except for the item price.
   1. Product quantity mustn’t exceed 5.
   1. Item URL, name, category, price are required.


Edfa3ly Shopping Cart Link: https://www.edfa3ly.com/cart


Challenge Description
---------------------
1. Automated products links
	* https://www.6pm.com/p/product/9409514
	* https://www.shein.com/CUCCOO-The-Everyone-Sneakers-p-1187851-cat-1913.html
1. Non-automated products links
	* https://www.adidas.com/us/nite-jogger-shoes/CG5950.html
1. Prohibited product link
	* https://www.abercrombie.com/shop/wd/p/skinny-suede-belt-41330319?categoryId=12266&seq=02&faceout=prod1
    * https://www.goat.com/sneakers/shane-sb-premium-light-orewood-brown-cv5500-200
  
Expected Deliverables
---------------------

1. Create a detailed bug with clear and repeatable steps, if found.
1. Write test cases for the all above products for all cart functionalities scenarios:
1. Write automation test (recommended tool is Selenium WebDriver with any programming language) to simulate: 
	* Adding one of the automated products.
	* Adding one of the prohibited products.
1. Should be executed on Chrome.
1. README file for how to run.
 
How will we review?
-------------------
 
[Guidelines can be found here](README.md)

---
#### Frequently asked questions 

##### Q: I currently work at a full-time job/Is there a deadline to deliver it?
###### A: Although there's NO deadline, we endorse having you take a good look at the task, send us back your best estimate of delivery, which can show us your commitment level without putting any pressure on your schedules.
