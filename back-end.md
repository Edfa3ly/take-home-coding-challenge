Back-end take home coding challenge guidelines
==============================================

Please organize, design, test, document and deploy your code as if it were
going into production, then send us a link to the hosted repository (e.g.
Github, Bitbucket...).

Functional spec
---------------

Prototype *one* of the following projects:

1. Shipping couriers architecture
2. Data processor architecture 

### Shipping couriers architecture 

Furnish architecture that supports different type of integrations with multiple [couriers](https://en.wikipedia.org/wiki/Courier) each has its own API methods and workflow.
 
##### Background
* Your system (client) doesn't care of the internals of each courier.
* Adding a new courier in future is something that happens very often. Your system shouldn't change then.

##### API sampling figure
![Couriers figure](https://dl.dropboxusercontent.com/s/9q7lnl5ul8edme8/Task%20number%20one.png)

### Data processor architecture 

Furnish architecture that supports different type of integrations with multiple data provider each has its own API own data format.
 
##### Background
* Your system (client) doesn't care of the internals of each data provider.
* Each integration type provide specific data format which can change in future and not coupled the provider itself.
* Adding a new data provider in future is something that happens very often. Your system shouldn't change then.

##### API sampling figure

![Data processor figure](https://dl.dropboxusercontent.com/s/mu3uqy36re31wuv/Task%20number%20two.png)


Technical spec
--------------
* Stick to SOLID principles.
* Use at least one design principle to achieve your goal.
* We believe there is no one-size-fits-all technology. Feel free to use any techonology.
Here are some technologies we are more familiar with:
	* PHP
	* Python
	* JavaScript
	* Ruby
	* Java 

How will we review?
-------------------

[Guidelines can be found here](README.md)
