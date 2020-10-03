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
	50% off jacket: -$12.495
Total: $61.336
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
