---
title: ServiceNow ITSM Reporting
permalink: /projects/servicenow-itsm/
---

*Redesigning a client-facing Power BI report to focus on the information stakeholders actually needed.*

<div class="portfolio-tags" aria-label="Tools used"><span>Power BI</span><span>DAX</span><span>Power Query</span><span>SharePoint</span><span>ServiceNow</span></div>

## Taking over an existing report

With a scheduled client review approaching, I was asked to take over an existing Power BI report built using external ServiceNow data. The original developer had left, and I had only a few days to prepare the report for presentation.

The initial request was straightforward: update the data source. The existing report pointed to a file saved locally on the previous developer's laptop, so I recommended moving the source files to SharePoint to make them accessible and easier to maintain.

Conversations with the managed services stakeholder also revealed that much of the report's information wasn't being referenced in client meetings. The report was visually dense and slow to load.

Rather than simply reconnect the existing report, I proposed a redesign focused on the information the team actually needed.

## Making the report useful

With no formal requirements document to work from, I used discussions with the managed services team to identify which information mattered most in their client meetings.

The existing report relied on implicit calculations, with no measures or period-over-period comparisons. I developed DAX measures to provide more meaningful operational metrics, including incident volumes, average resolution time and reassignment counts, along with quarterly comparisons to give those figures context.

One important consideration was the absence of a formalised SLA agreement. Rather than present compliance figures against targets that hadn't been established, I focused on measures that could help the team assess service performance without implying contractual commitments.

I also replaced a resource-intensive custom visual with native Power BI components, improving report performance while making better use of the available space.

Stakeholders had different preferences for how incident data should be presented. Rather than favour one approach, I created separate matrix and chart views, allowing the same information to be explored in whichever format best suited the discussion.

## Delivering under pressure

The completed report covered incidents, problems and change requests across four pages, including separate matrix and chart views for incident reporting.

I incorporated a bookmark-based toggle between monthly and quarterly views, along with dynamic DAX titles that automatically reflected the reporting period.

Because the data was supplied via email, I also streamlined the update process using SharePoint. The team only needed to upload the latest spreadsheets to the designated location, and Power BI could refresh the report without manual intervention. A twice-weekly refresh schedule kept the reporting current.

The initial client review resulted in only minor layout adjustments, with no structural changes requested.

## Report screenshots

Select an image to open it at full size.

### Incident Performance Overview

*A monthly and quarterly matrix of incident volumes, resolution times and reassignments, with comparisons to the previous quarter.*

<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/servicenow-itsm/SN-ITSM-IncidentOverview.png" target="_blank" rel="noopener noreferrer" aria-label="Open Incident Performance Overview screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/servicenow-itsm/SN-ITSM-IncidentOverview.png" alt="Incident Performance Overview" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### Incident Trends

*Visual trends in incident activity and operational performance, offering an alternative to the detailed matrix view.*

<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/servicenow-itsm/SN-ITSM-IncidentCharts.png" target="_blank" rel="noopener noreferrer" aria-label="Open Incident Trends screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/servicenow-itsm/SN-ITSM-IncidentCharts.png" alt="Incident Trends" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### Problem Management

*A view of problem records designed to support discussions about recurring issues and their operational impact.*

<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/servicenow-itsm/SN-ITSM-Problems.png" target="_blank" rel="noopener noreferrer" aria-label="Open Problem Management screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/servicenow-itsm/SN-ITSM-Problems.png" alt="Problem Management" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### Change Management

*Reporting on change activity to help stakeholders review patterns and monitor change requests over time.*

<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/servicenow-itsm/SN-ITSM-Change.png" target="_blank" rel="noopener noreferrer" aria-label="Open Change Management screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/servicenow-itsm/SN-ITSM-Change.png" alt="Change Management" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

[← Back to Projects]({{ "/projects/" | relative_url }})
