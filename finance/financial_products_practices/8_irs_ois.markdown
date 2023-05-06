---
layout: page
title: Interest Rate Swaps
grand_parent: Finance
parent: Products and Practices
nav_order: 8
---

# Interest Rate Swaps
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

<br />

## Introduction

An interest rate swaps (IRS) is a single currency swap of two legs, with one leg paying floating rate and another leg paying fixed rate.

For example, a 20-year USD IRS, where Party A paying a fixed rate of 4% to Party B, and receiving a floating rate of USD LIBOR 6 month with no spread from Party B.


<br />

## Mandatory Clearing

Cleared swaps mean that after an FI and a broker trades a swap, that swap is immediately given up to a clearing broker (e.g. MS, HSBC) that faces a central counterparty (e.g. CME, LCH SwapClear). All subsequent VM and activities will be done with the clearing broker.

Depending on jurisdictions, certain types of swaps have mandatory clearing obligations, e.g. USD, EUR, JPY, GBP & HKD basis swaps & fixed-to-floating IRS.


<br />


## Overnight Index Swaps

You can say Overnight Index Swaps (OIS) as a type of IRS, just that the floating rates will be overnight risk-free rates (RFRs) like SOFR, SORA, SONIA, etc.


<br />


## Notional Exchanges

IRS do not have notional exchanges.


<br />

## Payment Date Offset

If the floating rate is not an overnight rate but a term rate like 6-month LIBOR, then counterparties will have done rate fixing at the start of the calculation period which can be a quarter before the payment date. So there is usually no offset for payment date.

If the floating rate is an overnight rate, counterparties can only do fixing after the rate is published thus will cause, e.g. a 2-day delay, from the period end date to the payment date. 


<br />


## Confirmation

Many types of IRS / OIS (determined by notional currency and maturity) are mandated for central clearing on, e.g. LCH SwapClear or CME. In that case, these products will be cleared directly right after execution, and then reconciled on MarkitSERV (like trade matching). 

For bilateral IRS, they can be confirmed on MarkitWire or on paper.


<br />


## Day Count Convention

Day count conventions for IRS can vary but they are usually consistent for OIS.


<br />

## Period End Date Adjustment

Period end dates adjustmenets for IRS can vary but they are usually consistent for OIS.