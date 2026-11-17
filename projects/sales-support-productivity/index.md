---
title: Sales and Support Productivity
permalink: /projects/sales-support-productivity/
---

*Making operational contributions visible in reporting built around account ownership.*

**Tools:** Power BI · DAX · Power Query · Bookmarks · Figma

## The problem and initiative

Company reporting attributed sales activity and results to Account Executives (AEs) and their management hierarchy. Client Operations Specialists (COS), who supported those AEs by managing transactions and helping move business through the sales process, had no equivalent visibility into their own contributions.

I wanted to answer a straightforward question: **How am I doing?** But the existing reporting couldn't tell me.

I built a Power BI report for my own use. When I began using it in discussions with my manager, she recognised its value for the wider team. She subsequently used it with her manager, and the report's audience expanded from there.

As the report grew beyond my individual needs, a more structured way to identify COS-to-AE support relationships became necessary. No such mechanism existed in company reporting, so I created an Excel-based mapping table maintained by the department manager and team leads. This allowed the report to reflect changing support assignments and analyse activity across the wider Client Operations organisation.

## Growth and business value

Over four years, the report evolved into a 13-page Power BI solution containing 244 measures. Its expansion was driven by stakeholder questions and practical reporting needs rather than a predetermined development plan.

Team leads gained visibility into revenue, gross profit, quote and order volumes, and other performance metrics associated with the Account Executives their teams supported. AE managers could examine the same business activity from their own organisational perspective.

The Finance VP requested executive summaries for both the AE and COS organisations, while a team manager requested a product-mix view to examine business activity by line of business.

Throughout that growth, I maintained a consistent analytical foundation so the same business activity could be examined from different organisational perspectives. The report's continued use, expanding audience and stakeholder-driven additions were the clearest evidence of its value.

## Technical decisions

Several requirements called for solutions beyond standard Power BI visuals and calculations:

- **Context-sensitive DAX:** Percentage measures adjusted their denominators based on the expanded level of an AE matrix, moving between team, individual AE and COS support views.
- **Qualification indicators:** A six-state classification combined qualification status with COS support assignment, using custom icons created in Figma and incorporated through theme JSON.
- **Interactive comparisons:** A month-over-month/year-over-year toggle used bookmarks and styled buttons, predating Power BI's field parameters.
- **Contextual reporting:** Measure-driven text displayed assigned COS names, supported AE counts and qualification summaries directly within the report.

I also included an About page explaining business terminology and report navigation, hidden development notes documenting implementation decisions, and an embedded data dictionary using Power BI's INFO functions.

These decisions helped keep a growing report understandable and maintainable for people who hadn't built it.

## Rebuilding the report for this portfolio

To share the work without exposing company information, I rebuilt the report using synthetic data generated with a custom Python script.

The portfolio version uses Power BI's PBIP format, allowing its underlying Tabular Model Definition Language (TMDL) files to be edited directly. I migrated all 244 measures through targeted find-and-replace operations in those files rather than recreating them individually in the Power BI interface.

This preserved the report's analytical structure while replacing the original business data with synthetic records.

## Report screenshots

The screenshots below are grouped by the business questions they help answer. Select an image to open it at full size.

## Leadership overview
Executive summaries present revenue, gross profit and transaction activity from the AE and COS perspectives.

### Executive AE
*Leadership summary page showing revenue, GP, and quote/order volume with COS support breakdown across all metrics.*
<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20Exec%20AE.png" target="_blank" rel="noopener noreferrer" aria-label="Open Executive AE screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/sales-support-productivity/Productivity%20-%20Exec%20AE.png" alt="Executive AE" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### Executive ClientOps
*Mirror page from the COS team lens, pre-filtered to a single team.*
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
