---
layout: page
title: SWIFT
grand_parent: Finance
parent: Financial Systems
nav_order: 9
---

## SWIFT

<br />

_Note: There is a SWIFT ISO20022 migration that sees MT messages to be replaced with MX messages. MT messages are expected to retire in 2025. I will write on this later. For now, the below focuses on MT messages which are still the mainstream._

<br />

When people in finance operations say SWIFT, they are most likely referring to the SWIFT messaging network.

If you are a financial institution and you need to pay your counterparty for a trade settlement, you will send a SWIFT message to your bank to instruct them to pay your counterparty's bank.

SWIFT messages are standardized messages. And there are a number of formats for different purposes.

The commonly used ones are :

- MT103 Single Customer Credit Transfer 
  - some people treat this as payment proof, the originating bank send this to the beneficiary bank to tell them their client's account will get credited, but the beneficiary bank won't credit the beneficiary's account before they really receive the money through MT202COV
- MT202 General Financial Institution Transfer 
  - when banks pay to banks
- MT202COV Cover Payment
  - still when banks pay to banks, but they are doing so for cover payments, i.e. moving money in order to fulfill your payment to another bank's client
- MT210 Preadvice of Funds
  - you send this to your bank to tell them you are going to receive money
- MT540 Receive Free
  - when you receive some bonds from your counterparty as collateral, so receive free
- MT541 Receive Against Payment
  - still to receive a bond, but you need to pay in order to receive the bond
- MT542 Deliver Free
- MT543 Deliver Against Payment
- MT910 Confirmation of Credit
  - banks use this to tell you when they actually receive the money from other banks and credit to your account
- MT950 Statement Message

<br />

There are many fields in an MT message. Though the fields for different format are not the same, the fields usually include:
- message type
- sender and receiver
- message reference
- payment amount, currency
- payment date
- ordering customer
- ordering institution
- correspondent banks
- beneficiary bank
- beneficiary name
- charge payor
