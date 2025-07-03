```
# Guidance for Generating Lockhart Letter Sections (HTML Output)

This document provides guidance and boilerplate text for shared, common elements across different Lockhart Capital Management letters. Specific letter-type guidance files (e.g., `annual_review_guidance.md`) will refer to this document for these common parts and will provide instructions for the content unique to that letter type.

Fill in bracketed placeholders `[placeholder]` or `XXX` with relevant client and plan information. Retain HTML comments `<!-- ... -->` as instructions.

---

## 1. Standard HTML Document Structure

<!-- This basic structure should be assumed for all letters. -->
<!-- Specific guidance can override the <title> or add other <head> elements. -->

```html
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Lockhart Capital Management</title>
    <!-- Default Title - Override in specific guidance -->
    <!-- Add any firm-wide CSS links or common meta tags here if applicable -->
  </head>
  <body>
    <!-- ===== Letter Content Start ===== -->
    <!-- Specific letter content, guided by type-specific files, goes here. -->

    <!-- ===== Standard Important Points to Consider Start ===== -->
    <!-- This section can be appended to or modified by specific letter guidance if needed. -->
    <h2>Important Points to Consider</h2>
    <p>
      We offer "Independent Advice", meaning we will advise and make recommendations based on a comprehensive and fair analysis of the relevant market after assessing your needs.
    </p>
    <p>
      We categorize all clients to identify the appropriate level of regulatory protection. For this advice, you are treated as a Retail Client, enjoying the highest level of investor protection under UK law.
    </p>
    <p>
      Tax information is based on our understanding of current law and HMRC practice, which are subject to change. Tax treatment depends on individual circumstances and may change in the future.
    </p>
    <p>
      You have received our business card and Service Charter, including Terms of Business, confirming our authorization to advise on the areas covered in this report.
    </p>

    <h3>Financial Services Compensation Scheme ('FSCS')</h3>
    <p>
      The FSCS, established under the Financial Services and Markets Act 2000, protects clients of FCA-authorized firms, covering deposits, insurance, and investments.
    </p>
    <p>
      The Scheme compensates clients who have lost money due to dealings with FCA-authorized firms unable to pay claims, typically due to insolvency or ceasing trade.
    </p>
    <p>Compensation limits vary by product type. Refer to the FSCS guide provided for details. Contact us for a copy if needed.</p>
    <!-- ===== Standard Important Points to Consider End ===== -->

    <!-- ===== Letter Content End ===== -->
  </body>
</html>
```

## 2. Standard Letter Head Elements

<!-- To be included at the beginning of the letter body, before specific content. -->

```html
<!-- ===== Standard Client Address and Date Start ===== -->
<p><br /></p>
<div class="address">
  <p>
    Mr & Mrs [Client Last Name(s)]<br />
    [Client Address Line 1]<br />
    [Client Address Line 2 (if any)]<br />
    [City]<br />
    [Postcode]
  </p>
</div>

<div class="letter_date">
  <p>[Date of Letter, e.g., 30 April 2025]</p>
</div>
<!-- ===== Standard Client Address and Date End ===== -->
```

## 3. Standard Salutation

<!-- To follow the Letter Head elements. Can be adjusted in specific guidance if needed. -->

```html
<!-- ===== Standard Salutation Start ===== -->
<p>Dear Mr & Mrs [Client Last Name(s)],</p>
<!-- Or other appropriate salutation -->
<!-- ===== Standard Salutation End ===== -->
```

## 4. Standard Table of Contents Structure

<!-- Optional: Include this section if the letter requires a Table of Contents. -->
<!-- The specific list items (<li>) should be provided by the type-specific guidance. -->

```html
<!-- ===== Standard Table of Contents Start ===== -->
<h2>Table of Contents</h2>
<ul>
  <!-- Specific <li> items to be inserted here from type-specific guidance -->
</ul>
<!-- ===== Standard Table of Contents End ===== -->
```

## 5. Standard Sign-off

<!-- Used for concluding the letter. The adviser's name, qualifications, and title are placeholders. -->
<!-- This can be used multiple times if the letter has distinct parts signed off (e.g., cover letter part vs. report part) -->

```html
<!-- ===== Standard Sign-off Start ===== -->
<p>Yours sincerely,</p>
<p>
  <strong>[Financial Adviser Name] [Qualifications]<br />[Title]<br />Lockhart Capital Management</strong>
</p>
<!-- ===== Standard Sign-off End ===== -->
```

## 6. General Formatting Notes

- Use classes like `page-break-after` for print formatting where appropriate, as detailed in specific letter guidance.
- Ensure all placeholders `[placeholder]` are replaced with accurate client-specific information.
- HTML comments `<!-- ... -->` are for instructional purposes for the generator and should usually be removed from the final output unless specified.
- Comments like `<!-- ===== Section Name Start/End ===== -->` are used to clearly delineate blocks for easier template management and AI processing.

--- SPECIFIC TEMPLATE GUIDANCE ---

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
  - Example: `<p>Enclosed is your annual review, including:</p>`
  - List the key components of the review:
    - `<ul>`
    - `  <li>Confirmation of your current objectives</li>`
    - `  <li>Review of your Lockhart Capital Management portfolios</li>`
    - `  <li>Confirmation of fees and charges</li>`
    - `  <li>Overview of tax year allowances and legislative changes</li>`
    - `</ul>`
- **Standard Introductory Remarks (Annual Review Specific):**
  - Include paragraphs regarding action points, basis of the report, importance of accurate information, and availability for clarification specifically for the annual review context.
  - Example:
    - `<p>Action points agreed upon during our meeting will be confirmed separately. Formal advice requiring a recommendation letter will be issued if needed.</p>`
    - `<p>This report is based on our understanding of current legislation and the information you provided.</p>`
    - `<p>The suitability of our recommendations depends on the accuracy and completeness of the information provided. Please inform us of any changes to your circumstances.</p>`
    - `<p>Relevant reports and materials will be uploaded to the Wealth Platform for your records where possible.</p>`
    - `<p>Please contact us if you require clarification or assistance.</p>`
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
  - `<li>Current Circumstances</li>`
  - `<li>Financial Objectives</li>`
  - `<li>Wealth & Inheritance Tax Strategy (if applicable)</li>`
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
- Example: `<p>As Independent Financial Advisers, we provide independent, unbiased, and unrestricted advice. You have already received a copy of our Service Charter, detailing our services, charges, and Wealth Management Service proposition.</p>`
<!-- ===== Introduction (Annual Review Specific) End ===== -->

<!-- ===== Current Circumstances Start ===== -->

### Current Circumstances

- `<h1>Current Circumstances</h1>`
- Briefly state that personal circumstances were discussed and noted.
- Example: `<p>We discussed your personal circumstances during our meeting, and these have been recorded on our confidential Fact Find.</p>`
<!-- ===== Current Circumstances End ===== -->

<!-- ===== Financial Objectives Start ===== -->

### Financial Objectives

- `<h1>Financial Objectives</h1>`
- State that objectives were revisited and summarise them.
- Example: `<p>We revisited your financial objectives, which are summarized below:</p>`
- Use a list for clarity:
  - `<ul class="ul_financial_objectives">`
  - `  <li>[Objective 1, e.g., The funds are to remain invested for long-term growth.]</li>`
  - `  <li>[Objective 2, if applicable, e.g., To generate a sustainable income stream in retirement.]</li>`
  - `</ul>`
<!-- ===== Financial Objectives End ===== -->

<!-- ===== Wealth & Inheritance Tax Strategy Start ===== -->

### Wealth & Inheritance Tax Strategy

- `<h1>Wealth & Inheritance Tax Strategy</h1>`
- Recommend having a valid Will and Lasting Power of Attorney.
- Comment on potential IHT liability based on information provided.
- Mention future considerations (e.g., gifting) and commitment to ongoing review.
- Example snippets:
  - `<p>We strongly recommend you maintain a valid Will and Lasting Power of Attorney.</p>`
  - `<p>We can recommend a firm of lawyers if required.</p>`
  - `<p>Based on the information provided, your estate may be subject to inheritance tax.</p>`
  - `<p>You may consider gifting assets in the future.</p>`
  - `<p>We will continue to review your wealth and inheritance tax strategy during our annual reviews.</p>`
<!-- ===== Wealth & Inheritance Tax Strategy End ===== -->

<!-- ===== Ongoing Service Start ===== -->

### Our Ongoing Service

- `<h1>Our Ongoing Service</h1>`
- Explain the importance of regular reviews and the firm's commitment to them.
- Mention client access to support (e.g., Client Account Executive).
- Refer to the Service Charter for detailed service breakdown.
- Example: `<p>Regular reviews are essential to ensure your financial plan remains aligned with your goals and circumstances. We are committed to providing ongoing support and guidance. Your Client Account Executive is available to assist with any queries. Please refer to our Service Charter for a detailed breakdown of our services.</p>`
<!-- ===== Ongoing Service End ===== -->

<!-- ===== Lockhart Portfolios Start ===== -->

### Your Lockhart Portfolios

- `<h1>Your Lockhart Portfolios</h1>`
- Specify the review date: `<p>This Annual Review covers the following plans as of [Date of Valuation, e.g., 30th April 2025]:</p>`
- **Portfolio Table:** Present plan details clearly.
  - `<table class="table_portfolio">`
  - `  <colgroup> <col/> <col/> <col/> <col/> <col/> </colgroup>`
  - `  <tr> <th>Product</th> <th>Owner</th> <th>Provider</th> <th>Policy Number</th> <th>Value</th> </tr>`
  - `  <tr> <td>[Product Type, e.g., GIA]</td> <td>[Owner, e.g., Mrs Client]</td> <td>[Provider, e.g., Fusion Wealth]</td> <td>[Policy No.]</td> <td>Â£[Value]</td> </tr>`
  - `  <!-- Repeat for each product -->`
  - `  <tr> <td colspan="4"><strong>Total</strong></td> <td><strong>Â£[Total Value]</strong></td> </tr>`
  - `</table>`
- **Suitability Statement:** Confirm arrangements remain suitable.
  - `<p>Based on your current circumstances, requirements, and attitude to risk, we confirm that your existing arrangements remain suitable.</p>`
  - Include fair value assessment statement.
- **Disclaimers:** Note any limitations (e.g., not authorized for individual shareholdings).
  - `<p>Please note that we are not authorized to provide advice on individual shareholdings.</p>`
<!-- ===== Lockhart Portfolios End ===== -->

<!-- ===== Risk Profile Start ===== -->

### Your Risk Profile

- `<h1>Your Risk Profile</h1>`
- Explain that risk attitude is reviewed regularly.
- Mention the process (e.g., risk profiling questionnaire every two years).
- If a questionnaire is due, state this: `<p>As your risk profile is now older than two years, we have enclosed a risk questionnaire for you to complete.</p>` (or state it was completed).
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
    - `  <td class="risk_para"> <p>[Standardized text for this risk level description]</p> </td>`
    - `</tr> </table>`
- **Capacity for Loss:** Assess and confirm the client's capacity for loss.
  - Example: `<p>Based on your current financial situation, we believe you have the capacity for loss associated with your agreed risk level.</p>`
<!-- ===== Risk Profile End ===== -->

<!-- ===== Costs and Charges Start ===== -->

### Costs and Charges

- `<h1>Costs and Charges</h1>`
- Refer to the ex-post statement for aggregated fees (e.g., from Fusion Wealth Platform).
- Explain how fees are reconciled (e.g., from investments).
- Detail Lockhart's Ongoing Advice & Wealth Management Fee (percentage and current monetary value based on portfolio).
  - Example: `<p>Our Ongoing Advice & Wealth Management Fee is [Fee Percentage, e.g., 1.00%] per year, which amounts to Â£[Calculated Fee] p.a. based on the current value of your portfolio (this fee is included in your Fusion fee statement).</p>`
- List any additional administration charges (e.g., SIPP charges from Embark), specifying amounts and how they relate to plan values if variable.
  - `<p>In addition, you incur SIPP administration charges from Embark of [Amount] per year.</p>`
<!-- ===== Costs and Charges End ===== -->

<!-- ===== Conclusion (Annual Review Report Body) Start ===== -->

### Conclusion (Report Body)

- `<h1>Conclusion</h1>`
- Summarise client's satisfaction (if known) and reaffirm commitment to working together.
- Thank the client.
- <!-- Refer to guidance.md for Standard Sign-off structure -->
  - Example: Use standard sign-off with adviser's details.
<!-- ===== Conclusion (Annual Review Report Body) End ===== -->

## 4. Annual Review Specific Appendices

<!-- The main "Important Points to Consider" section, including FSCS, is now in guidance.md -->
<!-- If there are additional points specific ONLY to Annual Reviews, they can be guided here to be appended or integrated. -->

<!-- ===== Appendix A - Tax Allowances Start ===== -->

### Appendix A - Tax Allowances

- `<h1>Appendix A - Tax Allowances in [Tax Year, e.g., 2024/25]</h1>`
- **Instruction:** Ensure this section is updated with the correct allowances for the relevant tax year.
- List key allowances using `<ul>` and nested `<ul>` for sub-points:
  - `<ul><li>ISA allowance: [Amount]</li></ul>`
  - `<ul><li>Pension annual allowance: [Amount] (including notes on high earners)</li></ul>`
  - `<ul><li>Income Tax bands: [Specify bands and rates] (specify if different for Scotland) with personal allowance notes</li></ul>`
  - `<ul><li>Capital Gains Tax annual exemption: [Amount]</li></ul>`
  - `<ul><li>Dividend Allowance: [Amount]</li></ul>`
  - `<ul><li>Personal Savings Allowance: [Amount]</li></ul>`
  - `<ul><li>Starting Rate Savings Allowance: [Amount]</li></ul>`
- **Crucial:** Always verify these figures against the latest government information.
<!-- ===== Appendix A - Tax Allowances End ===== -->

<!-- ===== Appendix B - Legislative Update Start ===== -->

### Appendix B - Legislative Update

- `<h1>Appendix B - Legislative Update</h1>`
- **Instruction:** This section must be kept current with recent and relevant legislative changes affecting financial planning.
- List key updates using `<ul>` and nested `<ul>` for sub-points. Examples from template:
  - `<ul><li>Lifetime Allowance changes (LSA, LSDBA): [Details]</li></ul>`
  - `<ul><li>Pension Death Benefits (tax treatment before/after age 75, IHT implications from 2027): [Details]</li></ul>`
  - `<ul><li>Pension Contribution Annual Allowance (tapered allowance): [Details]</li></ul>`
  - `<ul><li>ISA rule changes (multiple ISAs, flexible ISAs): [Details]</li></ul>`
  - `<ul><li>State Pension & NI Record (voluntary contribution deadlines, cost/benefit, employer NIC changes): [Details]</li></ul>`
  - `<ul><li>Capital Gains Tax rate changes: [Details]</li></ul>`
  - `<ul><li>Inheritance Tax relief changes (business/agricultural reliefs, AIM shares): [Details]</li></ul>`
- **Crucial:** Research and include any new significant legislation.
- Concluding remark: `<p>To the best of our knowledge, there have been no other significant legislative developments since our last review that require major changes to your financial plan.</p>` (Adjust if there are significant developments).
<!-- ===== Appendix B - Legislative Update End ===== -->

<!-- ===== Body Content for Annual Review Letter Ends Here ===== -->

<!-- Ensure the document generation process concludes with the final </body> and </html> tags from guidance.md -->
```