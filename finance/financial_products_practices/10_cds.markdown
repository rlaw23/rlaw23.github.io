---
layout: page
title: CDS
grand_parent: Finance
parent: Products and Practices
nav_order: 10
---

# CDS
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

<br />

A credit default swap (CDS) is a type of derivatives that pays the buyer if the bond issuer (reference entity) default on the underlying debt (reference obligation). In return, the buyer needs to make, e.g. quarterly fees, to the CDS seller. CDS underlying can be corporate or sovereign debts.

<br />

### RED code

RED code (Reference Entity Data) is what the code that refers to the reference entity to make sure financial institutions are talking about the same entities. 

<br />

CDS start dates are always 20 Mar, Jun, Sep, and Dec. In a rare case in 2022, where 20 Jun was a holiday, industry participants held a conference to explicitly agreed to make new trades to start on 21 Jun 2022 instead.

<br />

### Recovery Rate

This affects the CDS payoff in case of a default.

CDS Payoff = Notional x (1 - Recovery Rate)

<br />

### Trade confirmation

Apart from confirming on paper, CDS trades can also be validated on TradeSERV (part of Markit), previously on DSMatch.

<br />

### Upfront Payment and Quarterly Payment

Upfront payment is the amount the counterparties of the CDS settle at the start of the CDS. 

The CDS buyer also pays a fixed annual rate of notional, e.g. 1%, as premium to the seller each quarter.

<br />

CDS usually matures on the 20th of Mar / Jun / Sep / Dec.

<br />

### Credit events

Credit events are events that will trigger the CDS to settle:
- Bankruptcy events
- Failure to pay
- Obligation acceleration
- Obligation default
- Repudiation/moratorium
- Restructuring

<br />

### Markit pricing

The industry usually use 2003 and 2014 ISDA Credit Derivatives Definitions:
- 2003 curves marked under the DocClauses (CR, MM, MR, XR)
- 2014 curves marked under new DocClauses (CR14, MM14, MR14, XR14)

<br />

### 2014 Definitions

| Doc Clause   | Restructuring Type         |
|:-------------|:---------------------------|
| XR14         | No Restructuring           |
| CR14         | Old / FUll Restructuring   |
| MR14         | Modified Restructuring     |
| MM14         | Modified Modified Restructuring  |


<br />


### Context for Pre-2014 Definitions

The 2014 Definitions introduced the Standard Reference Obligation, the Governmental Intervention Credit Event, the Asset Package Delivery provisions and the Financial Reference Entity Terms, and the replacement of the Succession Event with the Steps Plan.

<br />


### Pre-2014

Full Restructuring (FR) : in 1999 ISDA credit derivatives definitions. It considers any restructuring event as a credit event and any bond with a maturity of up to 30 years is deliverable.

No restructuring (NR) : excludes all restructuring events as trigger events, preventing protection buyers from potentially engaging in opportunistic behavior during soft credit events that do not result in a true loss.


<br />

### Key market infrastructure 

The CDS market is signficantly centralized. Trades are confirmed via MarkitSERV. DTCC maintains the Trade Information Warehouse. 

The Trade Information Warehouse streamlines the handling of various CDS lifecycle events, including credit event processing, reference entity renaming, payment calculation, etc.