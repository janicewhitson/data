---
title: Sales and Support Productivity
permalink: /projects/sales-support-productivity/
---

*Making operational contributions visible in reporting built around account ownership.*

**Tools:** Power BI · DAX · Power Query · Bookmarks · Figma

## The problem and initiative

Client Operations Specialists (COS) were the day-to-day point of contact for clients, handling quotes, orders, renewals, licensing enquiries and other account-related requests on behalf of their assigned Account Executives (AEs).

But company reporting told a different story. Everything was attributed to the Account Executives and their management hierarchy. There was no reporting that allowed COS to see the revenue, gross profit or transaction volumes associated with the accounts they supported.

I wanted to answer a fairly simple question: **How am I doing?**

The existing reports couldn't tell me.

So I built something that could.

What started as a Power BI report for my own use would eventually grow into something much bigger than I'd originally imagined.

## From a personal question to a shared resource

I began using the report with my Team Lead. She asked me to expand it to include our whole team, and eventually began using it with our Manager.

As its audience grew, I needed a way to connect each COS to the AEs they supported. That relationship didn't exist in company reporting, so I created an Excel-based mapping table, maintained by our Manager and Team Leads as assignments changed.

With that in place, Client Operations could finally see *their* activity and performance metrics.

Over the following four years, the report continued to grow in response to requests from different stakeholders, including additional performance views and executive summaries. Each addition answered a question someone actually needed answered.

## Making the details work

Some of the trickiest parts of the report involved finding ways to present nuanced, multilayered information clearly.

The sales qualification indicators were one of those challenges. Users needed to see both qualification and COS support statuses without having to interpret several separate fields. I developed six distinct indicators, designed the icons in Figma and incorporated them into Power BI through a custom theme. Getting the business rules, conditional formatting and visual design to work together took some experimentation, but the result communicated both statuses at a glance.

I also built a month-over-month/year-over-year comparison toggle using bookmarks and styled buttons, before Power BI introduced field parameters. It gave users a straightforward way to switch perspectives without navigating to another page.

Other details were less visible but equally deliberate: dynamic text that provided context within the report, an About page explaining terminology, and development notes to make future changes easier. I also used Power BI's INFO functions to build an embedded data dictionary, making table and column metadata available directly within the report.

## Rebuilding the report for this portfolio

To share the work without exposing company information, I rebuilt the report using synthetic data generated with a custom Python script.

The portfolio version uses Power BI's PBIP format, allowing its underlying Tabular Model Definition Language (TMDL) files to be edited directly. I migrated the existing measures through targeted find-and-replace operations in those files rather than recreating them individually in the Power BI interface.

This preserved the report's analytical structure while replacing the original business data with synthetic records.

## Report screenshots

The screenshots below are grouped by the business questions they help answer. Select an image to open it at full size.

## Leadership overview

### Executive ClientOps
*An executive-level overview of Client Operations performance, bringing revenue, gross profit and transaction activity into a single view of the team's contributions. The screenshot is filtered to a single team for illustration.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20Exec%20COS.png" target="_blank" rel="noopener noreferrer" aria-label="Open Executive ClientOps screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20Exec%20COS.png" alt="Executive ClientOps" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

## Team and individual performance
These views make the underlying business metrics accessible to Client Operations teams and managers, with detail by team, specialist and Account Executive.

### Client Ops Summary
*At-a-glance team comparison with COS count and full metric breakdown per team. No team filter — the columns are structural.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20COS%20Summary.png" target="_blank" rel="noopener noreferrer" aria-label="Open Client Ops Summary screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20COS%20Summary.png" alt="Client Ops Summary" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### ClientOps Team Summary
*Team-level detail with field parameter-driven column selection and bookmark-based table toggle.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20COS%20Team%20Summary.png" target="_blank" rel="noopener noreferrer" aria-label="Open ClientOps Team Summary screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20COS%20Team%20Summary.png" alt="ClientOps Team Summary" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### ClientOps Team Detail
*Full metric matrix with conditional formatting arrows and QoQ/YoY comparisons per COS/AE pairing.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20COS%20Team%20Detail.png" target="_blank" rel="noopener noreferrer" aria-label="Open ClientOps Team Detail screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20COS%20Team%20Detail.png" alt="ClientOps Team Detail" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### AE Team Summary
*AE-side equivalent of the Client Ops Summary, with COS support percentage visible on every volume metric.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Team%20Summary.png" target="_blank" rel="noopener noreferrer" aria-label="Open AE Team Summary screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Team%20Summary.png" alt="AE Team Summary" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### Account Executives
*Expandable matrix with context-sensitive percentage denominators shifting by hierarchy level.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE.png" target="_blank" rel="noopener noreferrer" aria-label="Open Account Executives screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE.png" alt="Account Executives" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

## Performance comparisons
Comparison views help users examine changes over time, including a bookmark-driven toggle between month-over-month and year-over-year perspectives.

### AE Team Detail — YoY
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Team%20Detail%20YoY.png" target="_blank" rel="noopener noreferrer" aria-label="Open AE Team Detail YoY screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Team%20Detail%20YoY.png" alt="AE Team Detail YoY" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### AE Team Detail — MoM
*MoM/YoY toggle implemented via bookmarks and styled buttons — no native toggle exists in Power BI.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Team%20Detail%20MoM.png" target="_blank" rel="noopener noreferrer" aria-label="Open AE Team Detail MoM screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Team%20Detail%20MoM.png" alt="AE Team Detail MoM" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

## Qualification tracking
Qualification views bring together business thresholds and COS support assignments.

### AE Sales Qualification Summary
*DAX-driven qualification classification across Hardware and Software thresholds, with dynamic support assignment indicators.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Support%20Qualify%20Summary.png" target="_blank" rel="noopener noreferrer" aria-label="Open AE Sales Qualification Summary screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Support%20Qualify%20Summary.png" alt="AE Sales Qualification Summary" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### AE Sales 12 Month Rolling — Full View
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Support%20Qualify%20Details.png" target="_blank" rel="noopener noreferrer" aria-label="Open AE Sales 12 Month Rolling Full screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Support%20Qualify%20Details.png" alt="AE Sales 12 Month Rolling Full" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### AE Sales 12 Month Rolling — Single AE
*Six-state custom icons built in Figma and imported via theme JSON, encoding qualification level and COS assignment status in a single visual element.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Support%20Qualify%20Details%20(1%20person).png" target="_blank" rel="noopener noreferrer" aria-label="Open AE Sales 12 Month Rolling Single AE screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20AE%20Support%20Qualify%20Details%20(1%20person).png" alt="AE Sales 12 Month Rolling Single AE" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

[← Back to Projects]({{ "/projects/" | relative_url }})
