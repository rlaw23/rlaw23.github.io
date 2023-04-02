---
layout: page
title: SSI
parent: Financial Systems
nav_order: 6
---

## SSI

<br />

SSI stands for Standing (or Standard) Settlement Instructions.

Simply it is the bank name, account number and account name of your counterparty when you send money to them. For each currency, there would be a different SSI. 

Not just cash, if you are trading bonds, you will also have SSI for your safekeep accounts.


<br />

### Structure of SSI

Simply speaking, your SSI consists of usually 2 layers, i.e. (1) your account at your bank, and (2) your bank's account at their correspondent bank. 

Banks don't have presence in every country to receive every currency. E.g. If you are in Hong Kong and you want to receive JPY through your custodian in Hong Kong (e.g. HSBC HK), most likely it will have to receive the JPY through their correspondent bank in Japan first (it can be HSBC Japan or any other Japanese banks) and then credit that to your account.

To make a fictional example, a cash account SSI would look like:

- Correspondent Bank Name: HSBC Japan
- Correspondent Bank BIC: HSBCJPJT
- Account Number at Correspondent Bank: 123456
- Beneficiary Bank: HSBC HK
- Account Number at Beneficiary Bank: 3456789
- Beneficiary Name / FFC (for further credit): Fictional Fund