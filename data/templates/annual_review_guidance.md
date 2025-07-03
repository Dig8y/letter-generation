# Guidance for Generating Lockhart Annual Review Letters (HTML Output)

This document provides specific guidance for drafting Annual Review letters for Lockhart Capital Management clients. It should be used in conjunction with the main `guidance.md` file, which contains shared HTML structures, standard text blocks, and general formatting instructions.

Ensure all placeholders `[placeholder]` are replaced with accurate client-specific information.

---

<!-- Instruct the generator to use the Standard HTML Document Structure from guidance.md -->
<!-- Override the default <title> for this specific letter type -->
<!-- <head> -->
<!--   <title>Lockhart Capital Management - Annual Review</title> -->
<!-- </head> -->

<!-- ===== Body Content for Annual Review Letter Starts Here ===== -->

<!-- Refer to guidance.md for Standard Letter Head Elements (Address, Date) -->
<!-- Refer to guidance.md for Standard Salutation -->

## 1. Annual Review Cover Letter Section

- **Opening Paragraph (Annual Review Specific):**
  - State the purpose of the letter clearly.
  - Example: `<p>We are pleased to enclose your annual review which includes the following: </p>`
  - List the key components of the review:
    - `<ul>`
    - `  <li>Confirmation of your current objectives </li>`
    - `  <li>A review of your existing Lockhart Capital Management portfolios </li>`
    - `  <li>Confirmation of your fees and charges </li>`
    - `  <li>An overview of tax year allowances and legislative changes </li>`
    - `</ul>`
- **Standard Introductory Remarks (Annual Review Specific):**
  - Include paragraphs regarding action points, basis of the report, importance of accurate information, and availability for clarification specifically for the annual review context.
  - Example:
    - `<p>Any current action points will have been confirmed to you after our meeting and a recommendation letter will be issued in due course should formal advice be required. </p>`
    - `<p>This report is based on our understanding of legislation and the information provided by you. </p>`
    - `<p>Any material facts that have not been provided, or have been incorrectly stated or omitted by you, could affect the suitability of our recommendations. </p>`
    - `<p>Please note that all relevant reports and materials will be uploaded where possible to the Wealth Platform for your records. </p>`
    - `<p>As always, should you require any clarification or assistance please do not hesitate to contact me. </p>`
- **Sign-off (Cover Letter Part):**
  - <!-- Refer to guidance.md for Standard Sign-off structure -->
  - Example: Use standard sign-off with adviser's details.

## 2. Annual Review Report Structure

- Insert a page break: `<div class="page-break-after"></div>`
- **Main Title:** `<h1>Annual Review Report</h1>`
- **Prepared For:** `<p>Prepared for Mr & Mrs [Client Last Name(s)]</p>`
- **Table of Contents (Annual Review Specific):**
  - <!-- Refer to guidance.md for Standard Table of Contents Structure (<h2> and <ul> tags). -->
  - <!-- The following <li> items are specific to the Annual Review and should be placed inside the <ul> from the standard structure. -->
  - `<li>Introduction</li>`
  - `<li>Considerations & Preferences (if applicable)</li>`
  - `<li>Current Circumstances</li>`
  - `<li>Financial Objectives</li>`
  - `<li>Your Wealth & Inheritance Tax Strategy</li>`
  - `<li>Our Ongoing Service</li>`
  - `<li>Your Lockhart Portfolios</li>`
  - `<li>Your Risk Profile</li>`
  - `<li>Costs and Charges</li>`
  - `<li>Conclusion</li>`
  - `<li>Important Points to Consider (Refer to guidance.md for base, can be extended here if AR specific points are needed)</li>`
  - `<li>Appendix A - Tax Allowances in [Current/Next Tax Year]</li>`
  - `<li>Appendix B - Legislative Update</li>`
  - Include a page break after the ToC: `<div class="page-break-after"></div>`

## 3. Core Annual Review Report Sections

<!-- ===== Introduction (Annual Review Specific) Start ===== -->

### Introduction

- `<h1>Introduction</h1>`
- Include standard firm introductory text, mentioning authorisation status and provision of Service Charter, tailored for the annual review context.
- Example: `<p>We remain authorised as Independent Financial Advisers, providing independent, unbiased and unrestricted advice and have already provided you with a copy of our Service Charter, which includes details of our services, charges and Wealth Management Service proposition.</p>`
<!-- ===== Introduction (Annual Review Specific) End ===== -->

<!-- ===== Current Circumstances Start ===== -->

### Current Circumstances

- `<h1>Current Circumstances</h1>`
- Briefly state that personal circumstances were discussed and noted.
- Example: `<p>We discussed your personal circumstances during our meeting, which have been noted on our confidential Fact find. </p>`
<!-- ===== Current Circumstances End ===== -->

<!-- ===== Financial Objectives Start ===== -->

### Financial Objectives

- `<h1>Financial Objectives</h1>`
- State that objectives were revisited and summarise them.
- Example: `<p>We revisited your objectives, which are summarised as follows: </p>`
- Use a list for clarity:
_ `<ul class="ul_financial_objectives">`
_ `  <li>[Objective 1, e.g., The funds are to remain invested for the foreseeable future...]</li>`
_ `  <li>[Objective 2, if applicable]</li>`
_ `</ul>`
<!-- ===== Financial Objectives End ===== -->

<!-- ===== Wealth & Inheritance Tax Strategy Start ===== -->

### Your Wealth & Inheritance Tax Strategy

- `<h1>Your Wealth & Inheritance Tax Strategy</h1>`
- Recommend having a valid Will and Lasting Power of Attorney.
- Comment on potential IHT liability based on information provided.
- Mention future considerations (e.g., gifting) and commitment to ongoing review.
- Example snippets:
_ `<p>We strongly recommend that you have a valid Will and Lasting Power of Attorney in place at all times. </p>`
_ `<p>If appropriate we can recommend a firm of lawyers to assist if required. </p>`
_ `<p>Based on the information provided, there may be an inheritance tax liability on your estate upon death. </p>`
_ `<p>You may consider gifting in the future, but feel it is too early in retirement to do so. </p>` \* `<p>We will continue to review this area of planning at our annual reviews. </p>`
<!-- ===== Wealth & Inheritance Tax Strategy End ===== -->

<!-- ===== Ongoing Service Start ===== -->

### Our Ongoing Service

- `<h1>Our Ongoing Service</h1>`
- Explain the importance of regular reviews and the firm's commitment to them.
- Mention client access to support (e.g., Client Account Executive).
- Refer to the Service Charter for detailed service breakdown.
<!-- ===== Ongoing Service End ===== -->

<!-- ===== Lockhart Portfolios Start ===== -->

### Your Lockhart Portfolios

- `<h1>Your Lockhart Portfolios</h1>`
- Specify the review date: `<p>As discussed, our Annual Review concentrated on the following plans that you currently hold, as at [Date of Valuation, e.g., 30th April 2025]: </p>`
- **Portfolio Table:** Present plan details clearly.
  - `<table class="table_portfolio">`
  - `  <colgroup> <col/> <col/> <col/> <col/> <col/> </colgroup>`
  - `  <tr> <th>Product</th> <th>Owner</th> <th>Provider</th> <th>Policy Number</th> <th>Value</th> </tr>`
  - `  <tr> <td>[Product Type, e.g., GIA]</td> <td>[Owner, e.g., Mrs Client]</td> <td>[Provider, e.g., Fusion Wealth]</td> <td>[Policy No.]</td> <td>Â£[Value]</td> </tr>`
  - `  <!-- Repeat for each product -->`
  - `  <tr> <td colspan="4"><strong>Total</strong></td> <td><strong>Â£[Total Value]</strong></td> </tr>`
  - `</table>`
- **Suitability Statement:** Confirm arrangements remain suitable.
  - `<p>We confirm the existing arrangements remain suitable for you, based on your current circumstances, requirements and attitude to risk. </p>`
  - Include fair value assessment statement.
- **Disclaimers:** Note any limitations (e.g., not authorised for individual shareholdings).
<!-- ===== Lockhart Portfolios End ===== -->

<!-- ===== Risk Profile Start ===== -->

### Your Risk Profile

- `<h1>Your Risk Profile</h1>`
- Explain that risk attitude is reviewed regularly.
- Mention the process (e.g., risk profiling questionnaire every two years).
- If a questionnaire is due, state this: `<p>[Client Name], as your risk results are now older than two years, we have enclosed a risk questionnaire for you to complete. </p>` (or state it was completed).
- Confirm discussions about risk tolerance.
- **Risk Profile Table:**
  - `<table class="table_riskinfo">`
  - `  <colgroup> <col/> <col/> <col/> <col/> </colgroup>`
  - `  <tr> <th>Client</th> <th>Risk level from questionnaire</th> <th>Agreed risk level</th> <th>Time Horizon</th> </tr>`
  - `  <tr> <td>[Client Name, e.g., Mr Client]</td> <td>[Score/Description, e.g., 5/10 (Medium)]</td> <td>[Score/Description]</td> <td>[Time Horizon, e.g., Throughout retirement]</td> </tr>`
  - `  <!-- Repeat for other client if applicable -->`
  - `</table>`
- **Risk Level Descriptions:** Include standard descriptions for the agreed risk levels.
  - Example for one risk level (repeat for each relevant level):
    - `<table class="table_risk"> <colgroup> <col /> <col /> </colgroup> <tr>`
    - `  <td> <p class="risk_number">[Risk Score, e.g., 3]</p> <p class="risk_value">[Risk Description, e.g., Low Medium]</p> </td>`
    - `  <td class="risk_para"> <p>[Standardised text for this risk level description]</p> </td>`
    - `</tr> </table>`
- **Capacity for Loss:** Assess and confirm the client's capacity for loss. \* Example: `<p>Based on your circumstances, I feel you have the capacity for loss to accept this level of risk at this stage. </p>`
<!-- ===== Risk Profile End ===== -->

<!-- ===== Costs and Charges Start ===== -->

### Costs and Charges

- `<h1>Costs and Charges</h1>`
- Refer to the ex-post statement for aggregated fees (e.g., from Fusion Wealth Platform).
- Explain how fees are reconciled (e.g., from investments).
- Detail Lockhart's Ongoing Advice & Wealth Management Fee (percentage and current monetary value based on portfolio).
  - Example: `<p>Lockhart's Ongoing Advice & Wealth Management Fee is [Fee Percentage, e.g., 1.00%] each year, which based on the current value of your portfolio is Â£[Calculated Fee] p.a. (this fee is included in your Fusion fee statement). </p>`
- List any additional administration charges (e.g., SIPP charges from Embark), specifying amounts and how they relate to plan values if variable.
<!-- ===== Costs and Charges End ===== -->

<!-- ===== Conclusion (Annual Review Report Body) Start ===== -->

### Conclusion (Report Body)

- `<h1>Conclusion</h1>`
- Summarise client's satisfaction (if known) and reaffirm commitment to working together.
- Thank the client.
- <!-- Refer to guidance.md for Standard Sign-off structure -->
      *   Example: Use standard sign-off with adviser's details.
  <!-- ===== Conclusion (Annual Review Report Body) End ===== -->

## 4. Annual Review Specific Appendices

<!-- The main "Important Points to Consider" section, including FSCS, is now in guidance.md -->
<!-- If there are additional points specific ONLY to Annual Reviews, they can be guided here to be appended or integrated. -->

<!-- ===== Appendix A - Tax Allowances Start ===== -->

### Appendix A - Tax Allowances

- `<h1>Appendix A - Tax Allowances in [Tax Year, e.g., 2024/25]</h1>`
- **Instruction:** Ensure this section is updated with the correct allowances for the relevant tax year.
- List key allowances using `<ul>` and nested `<ul>` for sub-points:
  - ISA allowance
  - Pension annual allowance (including notes on high earners)
  - Income Tax bands (specify if different for Scotland) with personal allowance notes
  - Capital Gains Tax annual exemption
  - Dividend Allowance
  - Personal Savings Allowance
  - Starting Rate Savings Allowance
- **Crucial:** Always verify these figures against the latest government information.
<!-- ===== Appendix A - Tax Allowances End ===== -->

<!-- ===== Appendix B - Legislative Update Start ===== -->

### Appendix B - Legislative Update

- `<h1>Appendix B - Legislative Update</h1>`
- **Instruction:** This section must be kept current with recent and relevant legislative changes affecting financial planning.
- List key updates using `<ul>` and nested `<ul>` for sub-points. Examples from template:
  - Lifetime Allowance changes (LSA, LSDBA)
  - Pension Death Benefits (tax treatment before/after age 75, IHT implications from 2027)
  - Pension Contribution Annual Allowance (tapered allowance)
  - ISA rule changes (multiple ISAs, flexible ISAs)
  - State Pension & NI Record (voluntary contribution deadlines, cost/benefit, employer NIC changes)
  - Capital Gains Tax rate changes
  - Inheritance Tax relief changes (business/agricultural reliefs, AIM shares)
- **Crucial:** Research and include any new significant legislation.
- Concluding remark: `<p>To the best of our knowledge, we believe there have been no other developments since our last review that require any major changes to your financial plan.</p>` (Adjust if there are significant developments).
<!-- ===== Appendix B - Legislative Update End ===== -->

<!-- ===== Body Content for Annual Review Letter Ends Here ===== -->

<!-- Ensure the document generation process concludes with the final </body> and </html> tags from guidance.md -->
