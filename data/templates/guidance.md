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
    <h1>Important Points to Consider</h1>
    <p>
      We offer "Independent Advice", this means that we will advise and make a
      recommendation for you after we have assessed your needs, and that our
      recommendation will be based on a comprehensive and fair analysis of the
      whole of the relevant market.
    </p>
    <p>
      We assess and categorise all our clients to identify the level of
      regulatory protection which should be applied.
    </p>
    <p>
      For the purpose of this piece of advice, we'll treat you as a Retail
      Client.
    </p>
    <p>
      Retail clients enjoy the highest level of investor protection provided by
      UK law.
    </p>
    <p>
      Any information provided about the tax position of any plans and
      recommendations made in the report, is based on my understanding of
      current law and HM Revenue & Customs practice which may be subject to
      alteration in the future.
    </p>
    <p>
      In particular, what assets, gains or income are taxed and the levels of
      taxation on them are all subject to change.
    </p>
    <p>
      Tax reliefs may also change and their value to you will depend on your
      individual circumstances.
    </p>
    <p>
      You have been provided with my business card and Lockhart Capital
      Management's Service Charter, which included our Terms of Business and
      confirms we are authorised to advise on the areas covered within this
      report.
    </p>

    <h3>Financial Service Compensation Scheme ('FSCS')</h3>
    <p>
      The FSCS was set up under the Financial Services and Markets Act 2000 and
      exists to protect clients of FCA authorised firms and covers deposits,
      insurance and investments.
    </p>
    <p>
      The Scheme can pay compensation to clients who have lost money as a result
      of their dealings with FCA authorised firms that are unable to pay claims
      against them, usually because they are insolvent or have stopped trading.
    </p>
    <p>The limit of protection varies between different types of products.</p>
    <p>
      Details of the FSCS compensation limits can be found in the FSCS guide,
      which has been previously provided.
    </p>
    <p>If you require a copy of this document please let us know.</p>
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
    Mr & Mrs [Client Names]<br />[Client Address Line 1]<br />[Client Address
    Line 2 (if any)]<br />[City]<br />[Postcode]
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
  <strong
    >[Financial Adviser Name] [Qualifications]<br />[Title]<br />Lockhart
    Capital Management</strong
  >
</p>
<!-- ===== Standard Sign-off End ===== -->
```

## 6. General Formatting Notes

- Use classes like `page-break-after` for print formatting where appropriate, as detailed in specific letter guidance.
- Ensure all placeholders `[placeholder]` are replaced with accurate client-specific information.
- HTML comments `<!-- ... -->` are for instructional purposes for the generator and should usually be removed from the final output unless specified.
- Comments like `<!-- ===== Section Name Start/End ===== -->` are used to clearly delineate blocks for easier template management and AI processing.
