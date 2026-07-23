---
name: Samiyah Customer ID Rules

description:
Customer identification standard defining how Samiyah manages
customer records, sales conversations, quotations, and follow-up history.

version: 1.0

---

# Samiyah Customer ID Rules


## Purpose


Every customer must have a unique Customer ID.


Customer ID connects:


Customer Information

↓

Conversation History

↓

Quotation Records

↓

Follow-up Actions

↓

Sales Results



# Customer ID Format


Format:


C + Year + Serial Number



Example:


C20260036



Meaning:


C

Customer


2026

Creation Year


0036

Customer sequence number



# Number Rules


## New Customer


When a new customer appears:


Create a new Customer ID.



Example:


First customer in 2026:


C20260001



Thirty-sixth customer:


C20260036



---

# Customer ID Principles


## Unique


One customer:

One Customer ID



Do not create duplicate IDs.



---

## Permanent


Once assigned:

Customer ID never changes.



Even if:


- Customer stops communication
- Customer changes products
- Customer returns later



---

## Central Reference


All customer-related information should reference Customer ID.


Example:


Quotation:


C20260036 - Toilet quotation


Conversation:


C20260036 - WhatsApp discussion


Follow-up:


C20260036 - Distributor development



# Customer Record Structure


Each customer record should include:


Customer ID


Company Name


Contact Person


Country


Market


Customer Type


Products Interested


Purchase Volume


Communication History


Quotation History


Follow-up Status


Next Action



# Customer Type Classification


## Importer


Customer buying products for import business.



## Distributor


Customer building local sales channels.



## Wholesaler


Customer purchasing for wholesale distribution.



## Project Buyer


Customer purchasing for projects.


Examples:


- Hotels
- Developers
- Contractors



## Retailer


Customer selling directly to end users.



## OEM Partner


Customer requiring customized products.



# Customer Status


New Lead


↓

Contacted


↓

Qualified


↓

Quotation Sent


↓

Negotiation


↓

Sample


↓

Order


↓

Repeat Customer



# AI Sales Agent Rules


When receiving customer information:


Step 1:


Check existing Customer ID.



Step 2:


If exists:

Continue existing record.



Step 3:


If not exists:

Create new Customer ID.



Step 4:


Save all future interactions under this ID.



# Customer Data Separation


Rules:


Customer management rules:

Stored here.


Customer individual information:

Stored separately.



Example:


Rule:


customer-id-rules.md



Customer:


C20260036.md



# Privacy Principle


Only store business-related customer information.


Focus on:


- Business needs
- Products
- Orders
- Communication history
- Cooperation opportunities
