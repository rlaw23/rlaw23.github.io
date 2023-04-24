---
layout: page
title: ISDA Master Agreement and CSA
grand_parent: Finance
parent: Documentation
nav_order: 3
---

# ISDA Master Agreement and CSA
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}


## Introduction

The ISDA Master Agreement:

- is executed between two counterparties for OTC derivatives transactions, e.g. swaps, forwards, etc
- is commonly used by banks and financial institutions
- reduces documentation burdens, as long confirmations are no more required for all the OTC derivatives transactions
- allows parties to only confirm the material terms of each transaction
- provides standard terms to aid in reducing disputes, improving risk and credit management

<br />

## ISDA Versions

There are 2 main versions of ISDA agreements:

- 1992 ISDA Master Agreement (Multicurrency - Cross Border)
- 2002 ISDA Master Agreement

<br />

## Crucial sections

Two crucial sections in an ISDA:

- Section 5 - Events of Default and Termination Events: lists various events, such as bankruptcy, that may lead to the termination of transactions
- Section 6 - Early Termination and Close-out Netting: outlines how transactions will be closed out in an early termination scenario.

<br />

## VM CSA - Paragraph 11

I usually find paragraph 11 to be the meat. You can find these in the CSA:
- What collateral are accepted (eligible credit support (vm)) (e.g. government bonds, cash, etc) and respective haircuts
- Base and eligible currency 
- Covered transactions (often exclude spot fx) 
- minimal transfer amount (MTA)
- Delivery amount (round up), return amount (round down), i.e. always over collateralized 
- Threshold
- Notification time (e.g. 4pm each business day)


<br />

## VM CSA Versions

There are English Law CSA, New York Law CSA, and English Law CSD. English Law CSA should be the most common.

English Law CSA is a title transfer arrangement. This means when the collaterals are delivered to the transferee, they become the tranferee's absolute property. In this sense, there is no question of reuse / retypothecation.

New York Law CSA and English Law CSD only create a security interest on the collateral in favor of the secured party. The pledgor still owns the legal title to the collateral and the secured party only holds the collateral in custody but not owns it.

Mind that though under the English Law CSA a transferee owns the collateral, it needs to return "equivalent credit support" to the other party in a margin call.


<br />

## Reference Recommendation

If you want to go into details, I recommend:
[Jolly Contrarian](https://jollycontrarian.com/index.php?title=Main_Page).
This very readable site is created by a lawyer who has years of experience in structured products, ISDA negotiation, equity derivatives and the like. You will have fun reading it.