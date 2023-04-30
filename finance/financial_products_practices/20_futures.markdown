---
layout: page
title: Futures
grand_parent: Finance
parent: Products and Practices
nav_order: 20
---

# Futures
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

<br />

## Introduction

Equity futures, bond futures, commodity futures

<br />

## BBG Ticker Convention

BBG futures ticker consist of 4 characters, for example, "XPM3" would indicate the Australia SPI 200 index futures expiring in Jun 2023. XP doesn't change and means "Australia SPI 200". "M" refers to the month June and "3" is the year 2023. 

Similarly "HIJ3" would indicate the HSI futures April 2023.

Common tickers:

| Ticker | Product |
|:-------|:---------------|
|HI|Hang Seng Index|
|HU|Mini Hang Seng Index|
|NK|Nikkei 225|
|NO|Mini Nikkei 225|

<!-- |XP| |
|VG| |
|FV| |
|TY| |
|TH| |
|RTY| | -->



Month codes:

| MONTH  |CODE|
|:-------|:---------------|
|Jan|	F|
|Feb|	G|
|Mar|	H|
|Apr|	J|
|May|	K|
|Jun|	M|
|Jul|	N|
|Aug|	Q|
|Sep|	U|
|Oct|	V|
|Nov|	X|
|Dec|	Z|


<br />

## Give-up Trades

Due to cost or other considerations, some investment managers may want to use one (or multiple) broker as execution broker and another as clearing broker. That would require a give-up agreement between the client and both brokers to be signed.

Each day, after the executing broker executes a trade of the client, they will need to offer the trades to the clearing broker before the timeline set by each futures exchange, usually some time after the market close.

Executing brokers should not sit on the positions themselves, in particular when it is a long deliverable position and after the first notice date. Otherwise the executing broker may risk physical delivery.

While it is easy for both brokers to give in and accept the give-ups at filled prices (i.e. the actual prices that each lot gets filled), some investment managers require averaged price give-ups to be booked on statements. 

In such case, there tend to be complexity as some markets (usually Asia markets) do not allow averaged price give-up trades on exchange. The clearing broker would need to check and book in the trades after calculating the averaged price themselves.



<br />


## Commissions and Fees

There are several commissions and fees related to a futures trade:
- Execution commission: (1) voice or (2) electronic
- Clearing commission
- Market fee
- NFA fee (depends)

<br />

<!-- ## Secured vs Segregated Accounts

<br />

## First Notice Date -->



<br />

## Futures Margin

### Initial Margin vs Maintenance Margin

Initial margin is what clients need to pay up when the position is opened. While retail clients can only pay this up in cash, institutional clients may fund this with bonds as collaterals. 

Maintenance margin is usually a bit lower than the initial margin. It is the minimum level of net equity that clients need to maintain in their account. When net equity falls below the maintenance margin, a margin call will be issued and clients need to pay up to restore the margin in their account to the initial margin level (**not** the maintenance margin level).


### Single Currency Margining vs Multi Currency Margining

<br />

## Futures Position Porting

If a client has two clearing brokers, they can port (i.e. migrate) their positions from one clearing broker to another. This usually would require internal approvals, such as from Compliance, within the brokers so would take usually a couple of days from receiving the request to completion.

