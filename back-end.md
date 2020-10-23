# BE take-home coding challenge guidelines.
Please organize, design, test, document, and deploy your code as if it were
going into production.

## Challenge Description

***Write a program that can price a cart of products, accept multiple products, combine offers, and display a total detailed bill in different currencies (based on user selection).***

Available catalog products and their price in USD:

* T-shirt $10.99
* Pants $14.99
* Jacket $19.99
* Shoes $24.99

The program can handle some special offers, which affect the pricing.

Available offers:

* Shoes are on 10% off.
* Buy two t-shirts and get a jacket half its price.

The program accepts a list of products, outputs the detailed bill of the subtotal, tax, and discounts if applicable, bill can be displayed in various currencies.

*There is a 14% tax (before discounts) applied to all products.*

E.g.:

Adding the following products:

```
T-shirt
T-shirt
Shoes
Jacket
```

Outputs the following bill, the user selected the USD bill:

```
Subtotal: $66.96
Taxes: $9.37
Discounts:
	10% off shoes: -$2.499
	50% off jacket: -$9.995
Total: $63.8404
```

Another, e.g., If none of the offers are eligible, the user selected the EGP bill:

```
T-shirt
Pants
```

Outputs the following bill:

```
Subtotal: 409 e£
Taxes: 57 e£
Total: 467 e£
```
  
## Requirements
1. PHP
1. Stick to OO fundamentals in all aspects of your code. 
1. Stick to SOLID principles.
	1. Code should allow future extensibility by *strictly* follow the Open-closed Principle.
1. Use pre-defined [Design Patterns](https://en.wikipedia.org/wiki/Software_design_pattern) whenever needed in your code. 
1. Input should be via either (whatever suits you)
	1. The command line in the form `createCart --bill-currency=EGP T-shirt T-shirt shoes`.
	1. Or a simple REST API.
1. Write unit tests to cover your core code fully.
1. No pseudo-code allowed. 
  
## Expected Deliverables
1. Hosted repository for the program, link to it (e.g.
Github, Bitbucket, etc.).
1. Code should be well structured, suitably commented, have error handling, and be tested.
1. README file, where you describe your solution (design and architecture), how to run the program. You can use pseudo-code here.
 
### How will we review?
[Guidelines can be found here](README.md)

---
#### Frequently asked questions 

##### Q: I have a more robust background in other languages than PHP. Can I use it to complete the task?
###### A: Yes, although the task endorses PHP as a requirement, we still believe that the best engineers are language agnostic. PHP reflects the primary language in our stack, which you'll be using daily.

##### Q: Can I use framework X to implement the task, use external libraries/dependencies, or shall I write the code in plain PHP?
###### A: The task itself doesn't require a specific framework to complete the task, nor using a framework breaks the requirements; however, with a deeper understanding of the task, you can make this decision on your own. Also, your choice of using any external libraries is considered as a part of our code review (Refer to "How will we review?" section)

##### Q: I currently work at a full-time job/Is there a deadline to deliver it?
###### A: Although there's NO deadline, we endorse having you take a good look at the task, send us back your best estimate of delivery, which can show us your commitment level without putting any pressure on your schedules.

##### Q: Shall I use any persistent layer to manage stuff like products or currencies?
###### A: This doesn't come as a requirement; however, we value using practices like configurations/fixtures to control these stuff, rather than adding some admin panel to enter these data.

##### Q: Do I need to provide a working interface to represent the task? Can I use a ready-made library that implements all the required functionalities?
###### A: No, the task is clearly about assessing your technical knowledge and problem solving from a design and architecture point of view; not showing this means you are failing the task requirements.
