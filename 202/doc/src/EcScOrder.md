---
name: EcScOrder
category: Front controllers
---

## Definition

PaypalEcScOrderModuleFrontController

This controller is used like handler. PayPal does the redirection to this controller when
the customer confirms the payment at the checkout flow of the paypal that is opened when
the customer press the button 'Express checkout' on the page of the product/cart

####  init()
This method call the `parent::init()` and set **payment token** that is necessary for correct 
work of the controller

#### postProcess()
This method call the `prepareProduct` method and handle the errors

#### prepareProduct()
Create or update the objects of the customer, the address and the cart

