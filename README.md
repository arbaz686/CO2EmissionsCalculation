# Machine Learning-Based Reporting for Sustainable Supply Chains (GHG Protocol) 🌲
*4 Steps to Develop ESG Reporting Focusing on Distribution Network CO2 Emissions*

<p align="center">
  <img align="center" src="images/intro.png" width=75%>
</p>
<p align="center">Supply Chain Sustainability Reporting</p>

The demand for transparent sustainable development from investors and customers has surged in recent years.

Investors now prioritize a company's sustainability when evaluating its value and resilience.

As a result, organizations are increasingly investing resources in developing sustainability reporting capabilities and devising optimal strategies for sustainable supply chains.

### YouTube Video
Click on the GIF below to watch a brief explanatory video outlining the concept behind this solution.
<div align="center">
  <a href="https://www.youtube.com/watch?v=yodNWnf7PQ0"><img src="https://github.com/samirsaci/supply-chain-sustainability/blob/main/thumbnail.webp" alt="Explainer Video Link"></a>
</div>

## **Article**
In this [article](https://towardsdatascience.com/supply-chain-sustainability-reporting-with-python-161c1f63f267), we introduce a simple methodology for **reporting CO2 emissions from your Distribution Network** using **Python and PowerBI**.

## **Definition**
Following the GHG Protocol corporate standard (Link), greenhouse gas emissions are classified into three scopes:

- Scope 1: Direct emissions released into the atmosphere due to the company’s activities (e.g., company facilities like manufacturing plants/warehouses, company vehicles).
- Scope 2: Indirect emissions from the generation of purchased energy (e.g., purchased electricity, gas).
- Scope 3: All other indirect emissions occurring in the company's value chain (e.g., transportation, waste operations, business travel).

This article focuses on Scope 3 calculations related to downstream transportation.
What is the environmental impact of your distribution network?

## **Formula**
Following the protocol of the French Environmental Agency Ademe, the formula for estimating transportation CO2 emissions is:

<p align="center">
  <img align="center" src="images/equation.png" width=75%>
</p>
<p align="center">Formula using Emission Factor</p>

This formula provides a gross estimation of CO2 emissions without requiring granular transportation data.
A more accurate approach would be to estimate CO2 emissions for each delivery, considering the vehicle model (e.g., truck, container carrier, plane, or train) and filling rate.

## **Objective**

1. Collect and process data to calculate emissions based on this formula.

<p align="center">
  <img align="center" src="images/data collection.png" width=75%>
</p>
<p align="center">Data Collection</p>

2. Calculate unit of measure conversions considering shipped handling units.

<p align="center">
  <img align="center" src="images/weight reference.png" width=75%>
</p>
<p align="center">Handling Units</p>

3. Add distances by mode and compute CO2 emissions per order.

<p align="center">
  <img align="center" src="images/emissions factors.png" width=75%>
</p>
<p align="center">Emission by Transportation Mode</p>

## **Examples of Visuals using PowerBI**

### Bubble map with size = f(CO2 Total)
<p align="center">
  <img align="center" src="images/bubble map.png" width=75%>
</p>
<p align="center">Bubble Map</p>

_Visual Insights_

Identify locations with the majority of CO2 emissions (large bubbles), color-coded by transportation mode.

### Split by Country Destination and Item Code
<p align="center">
  <img align="center" src="images/bar chart.png" width=75%>
</p>
<p align="center">Bar Chart</p>

_Product Portfolio Insights_

Discover the items with the highest environmental impact in each market.

### CO2 = f(Turnover) by City Destination
<p align="center">
  <img align="center" src="images/scatter plot.png" width=75%>
</p>
<p align="center">Scatter Plot</p>

_Financial Insights_

Evaluate the impact of future CO2 emission reduction efforts on profitability, particularly for customers in PEINE-WOLTORF.

# Code
This repository contains all the code and data used to explain the concepts presented in the article.
