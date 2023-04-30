---
layout: page
title: SOFR and Other ARR
grand_parent: Finance
parent: Products and Practices
nav_order: 105
---

# SOFR and Other ARR
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}


## Introduction

LIBOR are calculated for 5 currencies. And they are now (have been) replaced by their respective ARR (Alternative Reference Rates). 

| Country    | LIBOR   | ARR   |
|:---------------|:---------------|:--------------|
| Japan  | JPY LIBOR / TIBOR        | TONA   |
| Europe  | EURO LIBOR / EURIBOR        | ESTR   |
| UK  | GBP LIBOR        | SONIA   |
| US  | USD LIBOR        | SOFR   |
| Swizterland  | CHF LIBOR        | SARON   |


Singapore and Hong Kong have also transitioned from the similar SIBOR and HIBOR to SORA and HONIA respectively. However, Hong Kong has no plan to discontinue HIBOR, so HIBOR and HONIA will be published in parallel.

-----

## SOFR

At 8am ET each business day, the New York Fed publishes [here](https://www.newyorkfed.org/markets/reference-rates/sofr) a daily SOFR, three compounded SOFR averages with tenors of 30-, 90-, and 180- calendar days, and a SOFR Index that enables the calculation of compounded average rates over custom time periods.

Daily SOFR is published for the previous business day, e.g. on 25 Apr 2023, you will see a rate of value date 24 Apr 2023. However SOFR averages and index are published for the same day, e.g. on 25 Apr 2023, you will see these averages of value date 25 Apr 2023.

### Daily SOFR 

Published on 25 Apr 2023

![image](/assets/images/SOFR_20230425.jpg)


### SOFR Averages

Published on 25 Apr 2023

![image](/assets/images/SOFR_Avg_20230425.jpg)

------


## Calculating Compounded SOFR Averages

You can refer to the New York Fed's SOFR methodology [here](https://www.newyorkfed.org/markets/reference-rates/additional-information-about-reference-rates#sofr_ai_calculation_methodology).

The official SOFR average formula from NY Fed:

![image](/assets/images/sofr_calc.jpg)


### An Example

On 25 Apr 2023, the published 30-day SOFR average (VD 25 Apr 2023) is actually calculated with daily SOFR rates as of 26 Mar to 24 Apr 2023 (30 calendar days). 

As 26 Mar 2023 is a Sunday, we will apply the rate of 24 Mar 2023 to this day. Below is the step-by-step calculation with actual formulas as column names: 

![image](/assets/images/sofr_30_example.jpg)

The result is ~0.0482369 = 4.82369%, which is in line with the screenshot in the upper part of this page.

------


## Converting from USD LIBOR to SOFR

SOFR is (nearly) risk free because it is the cost of borrowing collaterized by Treasuries while USD LIBOR is not.

So when trades originally opened for USD LIBOR are now converted and fixed in SOFR, they need to be added a Spread Adjustment on top of the SOFR fixing to reflect that. Bloomberg has published the spreads for each LIBOR and each tenor [here](/assets/others/IBOR-Fallbacks-LIBOR-Cessation_Announcement_20210305.pdf).


------

## Forward Rates

