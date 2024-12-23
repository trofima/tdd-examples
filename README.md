# Clean Architecture Playground
Opinionated example of how you can apply SOLID principles and CA to UI Web development. Based on Uncle Bob Martin Clean Architecture and Functional Design books.
You will see UseCases, Entities, Presenters, Controllers, inverted dependencies etc.
<br>
And TESTS of course - simple, fast Developer tests (by Kent Beck).
<br>
Used `mocha/chai` for testing (you prefer `jest` - you are my enemy). 
<br>
<br>
The examples are not intended to be "true" FP, since true FP is readable only to chosen ones.
<br>
The examples are not intended to be "true" OOP. Because... because!
<br>
The intent is make it conceivable to everyone.

>[!CAUTION]
>**VERY DRAMATICALLY SUPER IMPORTANT NOTE:**
><br>
><span style="color:red">If you don't like something - I don't care...</span>
><br>
>If you have better ideas (unlikely) - create a PR and prepare to fight.

<br>
Stolen from net UI example (no, I'm not going to waste time on styles; only structure matters)
<img width="500" alt="image" src="https://github.com/user-attachments/assets/dc21ed21-7b9e-4e13-933c-b7f7001e9f23" />


## User Stories
In this example I implement part of backoffice for the online store. I do not intend to cover all edge cases and implement fully functional online store admin app. <b>I intend to implement practical example of several parts just as a showcase</b>. The following user stories will give you idea of what is or going to be covered.

### Render Order List
User should see list of the orders (first page) and total order count.
<br>Each order should contain id, created date, customer name, sum, payment status, fulfillment status.
<br>While loading the orders, user should see some indication of that.

### Open Order
User should be able to open the order to see its details.

### Remove Order
User should be able to remove order from the list.
<br>While removing, user should not be able to interact with the order.

### Change Order Payment status
User should be able to change an order payment status.
<br>While changing, user should not be able to interact with the order.

### Change Order Fulfillment status
User should be able to change an order fulfillment status.
<br>While changing, user should not be able to interact with the order.

### Render Next Page Of The Order List
User should be able to load next page to the the rest of the orders
<br>(It might be infinite scroll or pagination, decision has not been made yet)
