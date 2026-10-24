# Document Analysis Report — OCP Annual Financial Report 2023

## 1. Validation

| Field | Finding |
|---|---|
| Source file inspected | `Rapport Financier Annuel  OCP 2023 (1).pdf` (the supplied copy of `Rapport Financier Annuel OCP 2023.pdf`) |
| Document title | Rapport financier annuel 2023 |
| Organization | Groupe OCP / OCP |
| Reporting year | 2023, with 2022 comparative figures in the financial statements |
| Physical PDF pages | 210 |
| PDF metadata | Creator: Nitro Pro 13; creation date: 29 April 2024 |
| Original preserved | Yes. The source PDF was read only and was not changed. |

The file opens successfully with a PDF reader/parser. The first page identifies the document as
`RAPPORT FINANCIER ANNUEL 2023`, and page 2 provides a table of contents. The PDF has an
extractable text layer on 208 of 210 physical pages. Physical pages 63 and 96 produced no
text with the inspection parser; this does not by itself prove that they are scanned pages,
because they may be separator or graphic-only pages.

## 2. Main sections identified

The table of contents on physical page 2 identifies the core annual-financial-report section:

- **Chiffres clés et faits marquants de l'exercice** — printed pages 3–4; physical pages 3–4.
- **États financiers consolidés** — printed pages 5–10; physical pages 5–10.
- **Notes annexes aux états financiers consolidés** — printed pages 11–54; physical pages 11–54.
- **Rapport des commissaires aux comptes sur les comptes consolidés au 31 décembre 2023** —
  printed pages 55–60; physical pages 55–60.

The supplied PDF continues beyond that contents page. The additional material identified from
page headings is:

- **États financiers — Comptes consolidés & sociaux / OCP SA** — physical pages 62–125,
  including accounting methods, balance-sheet and tax schedules, and auditor material.
- **Management-control presentation** — physical pages 126–152, including market/activity
  analysis, OCP S.A. results, balance-sheet analysis and working-capital information.
- **Annex: Extra Financial Disclosures according to the GRI Standards** — physical pages
  153–209, covering OCP at a glance, sustainability strategy, environmental, social,
  governance and shared-value material, including a double-materiality analysis.
- **Press-release links** — physical page 210.

## 3. Representative content inventory

Page numbers below are **physical PDF page numbers**, not necessarily the printed page number
shown in the footer.

| Representative pages | Content type | Verified content and extraction observations |
|---:|---|---|
| 1–2 | Text / headings / navigation | Cover, title, organization website and table of contents. Text is extractable; the contents gives section names and printed-page references. |
| 3–4 | Text, tables, explanatory paragraphs | Page 3 contains the 2023/2022 key-figures table in millions of dirhams plus narrative commentary and bullet-point highlights. Page 4 contains explanatory text and post-closing events. Table values extract as text, but column alignment should be reconstructed rather than assumed from the text stream. |
| 5–10 | Financial tables and notes | Consolidated income statement, statement of financial position, cash-flow/equity information, footnotes and comparative 2022 figures. These are text-based tables with headings, units and note references; multi-column headers and footnote markers require layout-aware extraction. |
| 11–54 | Text and financial note tables | Notes 1–13, including accounting principles, consolidation scope, segment information, operational data, personnel, investments, provisions, financial instruments, tax, equity/dividends and shareholder relations. Dense tables and notes span multiple pages. |
| 55–60 | Text / audit report | Independent auditors' report and related explanatory text. Text is extractable and suitable for text indexing, subject to paragraph and heading segmentation. |
| 62–125 | Text and tables | OCP SA / consolidated-and-social accounts and schedules. Many pages have structured statement layouts; pages 116–118 have sparse extraction, so table reconstruction and visual verification are recommended. |
| 126–128 | Graphic pages / headings | Management-control section opening and agenda/context slides. Raster image objects are present, and some pages have little or no extractable text; visual extraction is needed for complete content. |
| 129–145 | Charts, figures, tables and explanatory text | Market demand, fertilizer/phosphate activity, raw-material prices, OCP S.A. results, revenue, expenses, financial result, income statement, balance-sheet and working-capital analysis. The page headings and explanatory text extract, while chart labels, plotted values and visual relationships may be stored as graphics or images rather than reliable reading-order text. |
| 149–150 | Charts / visual elements with text | Management-control pages contain multiple raster image objects alongside headings and short text. Treat these as visual evidence, not as ordinary text tables, until rendered and checked. |
| 153–159 | Sustainability headings, text, figures | Extra-financial disclosure annex begins; pages include an agenda/section overview and OCP/sustainability material. Pages 153 and 159 contain image objects. |
| 167–180 | Sustainability tables and charts | Environmental and social indicators, including year comparisons and workforce-related data. These are primarily extractable text, but charts and compact tables need coordinate-aware parsing. |
| 181 | Text plus image | Sustainability/social discussion with a raster image object. Caption-to-image association should be retained during indexing. |
| 207–209 | Text plus figures / closing pages | Double-materiality analysis and annex closing material. Image objects occur on pages 207–209; pages 208–209 contain very little extractable text, so OCR or image understanding may be required. |
| 210 | Text / links | List of OCP press releases and a download link. This is text metadata rather than a substantive financial table or chart. |

## 4. Content-type confirmation

- **Text: confirmed.** Headings, paragraphs, bullet points, explanatory notes, audit language,
  dates, units and numerical values are directly extractable from most pages.
- **Tables: confirmed.** Examples include the key-figures comparison on page 3, consolidated
  financial statements on pages 5–10, note tables on pages 11–54, and OCP SA schedules on
  pages 62–125. These are actual tabular financial data, not merely decorative grids.
- **Images and charts: confirmed.** The PDF contains raster image objects on 34 physical pages
  (66 image objects detected in total), notably in pages 126–145, 149–150, 153, 159, 181 and
  207–209. The headings and surrounding text identify market/activity charts, price visuals,
  management-control graphics and sustainability visuals. Vector graphics/form objects also
  occur, so an image-object count is not a complete count of all visual elements.
- **Decorative elements versus data visuals:** cover/section artwork and branding should not be
  indexed as factual charts. Conversely, the market, price, activity, results, environmental
  and social visuals listed above should be treated as data-bearing figures or charts unless
  page rendering proves otherwise. A table represented as text is not classified as an image
  merely because it has borders or a designed layout.

## 5. Suitability and limitations

This is a strong test document for a multimodal document-processing pipeline because it combines
long-form French and English text, financial tables with comparative years, footnotes, audit
prose, slide-like pages, raster figures, charts, and sustainability disclosures in one PDF.
It is **not a purely scanned document**: the extensive text layer makes ordinary text extraction
viable for most pages.

Expected extraction difficulties:

1. Reading order and column boundaries may be lost in dense financial tables. A text extractor
   can return values and labels but not reliably preserve row/column relationships.
2. Footnote markers, superscripts, repeated headers/footers and printed versus physical page
   numbering can create duplicate or misleading chunks.
3. Chart axes, legends, plotted values and captions may not be represented as normal text.
   Pages with sparse text and image objects (especially 126–145 and 207–209) require rendering,
   image extraction and/or OCR/vision analysis.
4. The document contains mixed French and English material. Language detection and
   normalization should be per page or chunk, not assumed globally.
5. Pages 63 and 96 have no text returned by the inspection parser. They should be rendered
   before deciding whether they are blank, image-only, or affected by an extraction issue.
6. The PDF contains multiple logical documents/annexes after the core annual financial report.
   Index metadata must preserve the section/annex boundary rather than treating all 210 pages
   as one undifferentiated financial statement.

## 6. Recommended inventory for the next LlamaIndex stage

Preserve one page-level record per physical page with at least:

```text
document_id
source_filename
title
organization
reporting_year
physical_page
printed_page (when visible)
logical_section
language
content_types: [text, table, chart, image, footnote, link]
extraction_method: [text_layer, table_parser, rendered_image, OCR, vision]
text
table_regions / figure_regions
caption
confidence
```

Recommended next steps are to render representative pages before indexing, detect table and
figure regions using page coordinates, extract tables with their units and comparative-year
headers, preserve captions and footnotes with their parent figures/tables, and run OCR/vision
only on image-only or chart-heavy regions. Keep the original PDF as the immutable source and
retain physical-page references in every LlamaIndex node so extracted answers can be traced
back to the document.