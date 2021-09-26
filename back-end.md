# BE take-home coding challenge guidelines.
Please organize, design, test, document, and deploy your code as if it were
going into production.

## Challenge Description

***Write a program that can price a cart of products from different countries, accept multiple products, combine offers, and display a total detailed invoice in USD as well.***

**Available catalog products** and their respective price in USD (regardless of the shipping country):
**Hint**: [see below, how to calculate each item shipping fees](#q-i-got-confused-on-how-to-calculate-an-item-price-and-its-shipping-and-vat)

| Item type | Item price | Shipped from | Weight |
| -------- | -------- | -------- |  -------- | 
| T-shirt | **$30.99** | **US** | **0.2kg** |
| Blouse | **$10.99** | **UK** | **0.3kg** |
| Pants | **$64.99** | **UK** | **0.9kg** |
| Sweatpants | **$84.99** | **CN** | **1.1kg** |
| Jacket | **$199.99** | **US** | **2.2kg** |
| Shoes | **$79.99** | **CN** | **1.3kg** |

Each country has a shipping rate per 100 grams 

**Shipping rates**:
**Hint**: [see below, how to calculate each item shipping fees](#q-i-got-confused-on-how-to-calculate-an-item-price-and-its-shipping-and-vat)
| Country | Rate  | 
| -------- | -------- |
| US | $2 |
| UK | $3 |
| CN | $2 |

The program can handle some special offers, which affect the pricing.

**Available offers**:

* **Shoes** are on 10% off.
* Buy any **two** tops (t-shirt or blouse) and get any jacket **half** its price.
* Buy any **two** items or *more* and get a **maximum** of $10 off shipping fees.



**There is a 14% VAT (before discounts) applied to all products, whatever the shipping country is.**

The program **accepts** a list of products, **outputs** the detailed **invoice** of the subtotal (sum of items prices), shipping fees, VAT, and discounts if applicable.



**e.g.**

Adding the following products:

```
T-shirt
Blouse
Pants
Shoes
Jacket
```

Outputs the following invoice:

```
Subtotal: $386.95
Shipping: $110
VAT: $54.173
Discounts:
	10% off shoes: -$7.999
	50% off jacket: -$99.995
	$10 of shipping: -$10
Total: $433.129
```

Another, e.g., If none of the offers are eligible by adding one product:

```
Jacket
```

Outputs the following invoice:

```
Subtotal: $199.99
Shipping: $44
VAT: $27.9986
Total: $271.9886
```
  
## Requirements
1. PHP
1. Stick to OO fundamentals in all aspects of your code. 
1. Stick to SOLID principles.
1. Use pre-defined [Design Patterns](https://en.wikipedia.org/wiki/Software_design_pattern) whenever needed in your code. 
1. Input should be via either (whatever suits you)
	1. The command line in the form `createCart --product='T-shirt' --product='Blouse' --product='Pants' --product='Shoes' --product='Jacket'`.
	1. **Or** a simple REST API.
1. Write unit tests to cover your core code fully.
1. No pseudo-code allowed. 
  
## Expected Deliverables
1. Hosted repository for the program, link to it (e.g.
Github, Bitbucket, etc.). **Reply** with the repo link to the **email** we sent.
1. Code should be well structured, suitably commented, have error handling, and be tested.
1. README file, where you describe your solution (design and architecture), how to run the program. You can use pseudo-code here.

 
### How will we review?
[Guidelines can be found here](README.md)

---
#### Frequently asked questions 

##### Q: I got confused on how to calculate an item price and its shipping and VAT
###### A: You can use the following table as a complete reference (DO NOT HARDCODE ANY CALCULATED VALUES) 
|Item type|Country|Item price|Weight|Rate |Shipping|VAT|
| -------- | -------- | -------- | -------- | -------- | -------- |-------- |
|T-shirt |US|$30.99|0.2|$2|$4|$4.3386|
|Blouse |UK|$10.99|0.3|$3|$9|$1.5386|
|Pants|UK|$64.99|0.9|$3|$27|$9.0986|
|Sweatpants|CN|$84.99|1.1|$2|$22|$11.8986|
|Jacket|US|$199.99|2.2|$2|$44|$27.9986|
|Shoes|CN|$79.99|1.3|$2|$26|$11.1986|

##### Q: I have a more robust background in other languages than PHP. Can I use it to complete the task?
###### A: Yes, although the task endorses PHP as a requirement, we still believe that the best engineers are language agnostic. PHP reflects the primary language in our stack, which you'll be using daily.

##### Q: Can I use framework X to implement the task, use external libraries/dependencies, or shall I write the code in plain PHP?
###### A: The task itself doesn't require a specific framework to complete the task, nor does use a framework break the requirements; however, with a deeper understanding of the task, you can make this decision independently. Also, your choice of using any external libraries is considered as a part of our code review (Refer to the "[How will we review?](#How-will-we-review)" section)

##### Q: I currently work at a full-time job/Is there a deadline to deliver it?
###### A: Although there's NO deadline, we endorse having you take a good look at the task; send us back your best estimate of delivery, which can show us your commitment level without putting any pressure on your schedules. **Most candidates deliver it in a week**.

##### Q: Shall I use any persistent layer (database) to manage stuff like products or currencies?
###### A: This **doesn't** come as a requirement; however, we value using practices like configurations/fixtures to control these stuff, rather than adding some admin panel to enter these data.

##### Q: Do I need to provide a functional user interface to represent the task? Can I use a ready-made library that implements all the required functionalities?
###### A: No, the task is clearly about assessing your technical knowledge and problem solving from a design and architecture point of view; not showing this means you are failing the task requirements.
