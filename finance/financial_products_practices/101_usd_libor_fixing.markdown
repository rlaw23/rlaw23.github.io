---
layout: page
title: USD LIBOR Fixing
grand_parent: Finance
parent: Products and Practices
nav_order: 101
---

# USD LIBOR Fixing
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}


## Introduction

LIBOR is ending (or already ended when you read this). But I just want to note this down.

Most of the USD floating rate legs would have a floating rate option of USD-LIBOR or USD-LIBOR-BBA.

According to the [ISDA documentation](/assets/2006-FRO-Mapping-to-2021-FROs-Version-3.pdf), USD-LIBOR-BBA (defined in 2006) and USD-LIBOR (defined in 2021) actually refer to the same thing. And that is the USD LIBOR rate shown on some mystic telerate page **2 London banking days** preceding the reset date. The reset date is usually the first day of a calculation period.


## Fixing Source

Certainly we will not be looking at a telerate page to do our fixing. In a Bloomberg terminal (or Reuters), we will go to the relevant page, e.g. for a 6-month USD libor, we will go to US0006M<GO> and HP<GO> to see its historical prices.


## Example

If a calculation period is from 10 Feb 2023 (Fri) to 10 August 2023, the reset date would be 10 Feb 2023 (the first day of a calculation period). 

Then we would look at Bloomberg and take the rate as of 8 Feb 2023 (Wed) as the fixing rate of this whole period.


