# Digital invoicing - Assignment
---

Implement a REST service and a web application to manage invoices.

## Terminology
---

- **Cutommer** - A customer can have many invoices
- **Invoice** - An invoice belong to one and only one Customer
- **Address** - Holds address informations

## Requirements
---
### Backend
The service should implement the following fonctionalities:
- Create **[Customer, Invoice, Address]**
- Update **[Customer, Invoice, Address]**
- Delete **[Customer, Invoice, Address]**
- Get all/paginated/partially(search, filter) **[customers, invoices, addresses]**

### Frontend
The frontend app should implememt the following features:
- Manage **[customers, invoices, addresses]** according to provided service(backend)
- Display a paginated data(particularly invoices) with filter support
- Add the possbility to print invoices.

## Minimum entities Schema
---
### Invoice
-  invoiceNumber : a string representing the invoice number 
-  customer : a  Customer  object representing the customer associated with the invoice 
-  items : a list of  InvoiceItem  objects representing the items included in the invoice 
-  billingAddress : an Address  object representing the billing address associated with the invoice 
-  totalAmount : a double representing the total amount charged for the invoice 
### Customer
-  name : a string representing the name of the customer 
-  email : a string representing the email address of the customer 
-  phone : a string representing the phone number of the customer 
-  address : an Address  object representing the address of the customer 
### Address
-  street : a string representing the street address 
-  city : a string representing the city 
-  state : a string representing the state 
-  zipCode : a string representing the zip code 
-  country : a string representing the country 
### InvoiceItem
-  name : a string representing the name of the item 
-  quantity : an integer representing the quantity of the item included in the invoice 
-  price : a double representing the price of the item 
-  total : a double representing the total price charged for the item in the invoice 

## Notes
- The previous schema ist just an minimal schema, then you could complete it if necessary.
- Our tech stack is mostly Java with Spring framework and React for front-end.
- Please create a 'production-ready' service as you see it (documentation / tests / logs / exception handling).
- Please provide an instruction on how to run the app.
- Submit your solution either as a public repository (github, bitbucket, etc.) or as a zip archive.
