---
title: Partner Commission Modelling Tool
permalink: /projects/partner-commission-tool/
---

*An Excel-based prototype developed to support the design and evaluation of a proposed software partner program.*

<div class="portfolio-tags" aria-label="Tools used"><span>Excel</span></div>

## Background

An early-stage independent software vendor (ISV) was exploring the introduction of a partner program. With no established partner network or sales history, the company needed to define a commission structure that would encourage external partners to sell its products.

During an informal discussion with the person responsible for developing the proposal, we explored potential commission structures, partner tiers and how these might relate to volume-based pricing.

Drawing on my experience with SaaS licensing and pricing structures, I offered to develop a working model that would allow management to explore the proposed structure rather than relying solely on a written proposal.

## Development and Design

I developed the Excel prototype that same evening, incorporating two distinct scenarios:

**New and Prospective Partners**

The model allows users to enter purchase quantities and commitment terms to determine the applicable partner tier, commission rate and estimated earnings. Where quantities fall below the minimum qualifying threshold, the model displays a notification.

**Existing Partners**

Although not part of the initial discussion, I added a second scenario to demonstrate how an increase in commitment could affect an existing partner's status and commission earnings. Comparing current and projected tiers side by side provided a way to evaluate the financial incentive for increasing that commitment.

Both scenarios reference a shared structured table containing the tier thresholds and commission rates. The model uses XLOOKUP with approximate matching to determine the applicable tier, with error handling for quantities below the minimum threshold.

Separating the tier and rate definitions from the calculation logic allows the proposed parameters to be adjusted without modifying the underlying formulas.

## Outcome

The prototype was used during an internal presentation to management. Feedback indicated that the working model helped management better understand the proposed commission structure.

The company ultimately chose not to proceed with the partner program, and the tool remained a working prototype.

## Tool Screenshots

Select an image to open it at full size.

### New and Prospective Partners

<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/PartnerCommTool/PCTool-New.png" target="_blank" rel="noopener noreferrer" aria-label="Open New and Prospective Partners screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/PartnerCommTool/PCTool-New.png" alt="New and Prospective Partners" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

### Existing Partners

<a href="https://janicewhitson.github.io/voiceofdata/data/case-studies/PartnerCommTool/PCTool-Existing.png" target="_blank" rel="noopener noreferrer" aria-label="Open Existing Partners screenshot at full size"><img src="https://janicewhitson.github.io/voiceofdata/data/case-studies/PartnerCommTool/PCTool-Existing.png" alt="Existing Partners" loading="lazy" style="display:block; max-width:100%; height:auto;" /></a>

*Product names have been replaced with generic placeholders. No proprietary company or partner data is included.*

[← Back to Projects]({{ "/projects/" | relative_url }})
