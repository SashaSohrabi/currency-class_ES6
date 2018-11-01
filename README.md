# Currency-ES6

Create Currency Class with follow parameters:
property: quantity (default: 1)
property: ratioWithProto (default: 1)
property: sign (default: $)
method: sum
method: isCurrencyType
method: sum - Summarizes different currencies. 
Returns answer in a currency which method it was 
Use ratioWithProto
Create a Dollar class extending from Currency (ratioWithProto: 1)
Create a Canadian class extending from Dollar (ratioWithProto: 1.2)
Create a Hryvna class extending from Currency (ratioWithProto: 0.65)
Create instances from different classes and try to sum them
Create static property count for Dollar. Which will return a count of instances of this class
Create getter in Dollar class for quantity property
Summarize different currencies:
5 Hryvna + 5 Dollars
12 Canadian Dollars + 10 Hryvna
Example:

let pocketMoney = new Dollar(5);
pocketMoney.quantity; -> '5$';
let stash = new Hryvna(200); 
let total = pocketMoney.sum(stash);
total.quantity -> '135$';
total.isCurrencyType(Dollar); -> true;
Dollar.count() -> 2;
