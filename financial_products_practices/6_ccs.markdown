---
layout: page
title: Cross Currency Swaps
parent: Financial Products and Practices
nav_order: 6
---

# Cross Currency Swaps
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

<br />

## Introduction

A cross currency swap allows bilateral counterparties to exchange regular interest payments (coupons) of the two currencies during the life of the swap. The interest rates can be fixed or floating for one or both legs.

For example, Party A and Party B enters into a CCS, where Party A will pay a fixed rate of 5% on USD 10m notional, and Party B will pay a fixed rate of 4.5% on GBP 8m notional. The parties may choose to exchange the relevant notional at the start and end dates of the swap. 


<br />


## Notional Exchanges

Initial Exchange = counterparties exchange notionals, usually, on the first date of the first calculation period (Party A pays GBP 8m to, and receives USD 10m from Party B)

Final Exchange = counterprties re-exchange notionals, usuaully, along with the payment of the last coupons (Party A receives GBP 8m to, and pays USD 10m from Party B)

Inital and final exchanges do not necessarily happen however.


<br />

## Payment Date Offset

A Payment Date Offsets refer to the delay between the last day of the calculation period and the settlement date of the interest payment. There are usually no offsets for a CCS with both legs having fixed rates, i.e. each coupon is settled on the last day of each calculation period.


<br />


## Confirmation

CCS can be confirmed via paper confirmations or on MarkitWire / MarkitSERV Trade Manager.


<br />


## Day Count Convention

In calculating interest payments, we don't really take in the actual no. of days in the calculation period and actual no. of days in a year into the calculation, but normalized them to, say 30 days in a month or 360 days in a year.

There are different ways to do this normalization, i.e. there are many different Day Count Conventions. Common ones are 30E/360, Act/Act, Act/365, etc.

<br />

## Period End Date Adjustment

If a calculation period end date falls on a holiday, it can be adjusted accordingly or not. This is agreed per leg at trade.

Common parameters are: 
- None
- Following  (basically to use the following business day instead) 
- Modified Following  (same as Following if the following business day doesn't fall to the next month; if it does then use the preceding business day)