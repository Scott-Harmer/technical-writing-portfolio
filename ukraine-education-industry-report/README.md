# Ukraine Education Industry Report: Research and Structured Publishing

**Strategic industry research | Long-form report writing | DITA/XML and DocBook 5.0**

## Project overview

My original 45-page report, *Ukraine: The Education Industry: Strategic Analysis and Market Outlook* (2021), demonstrates long-form research, strategic analysis and the organisation of complex industry information into a structured, readable publication.

I subsequently converted the report into DITA/XML and DocBook 5.0, demonstrating structured authoring, XML validation and HTML5 publishing. Recruiters can review both the [original 45-page report (PDF)](ukraine-education-report-2021.pdf) and the published web version.

The research reflects the Ukrainian education industry in 2021; its findings and projections are historical rather than current.

**[Read the published HTML5 report](https://scott-harmer.github.io/technical-writing-portfolio/ukraine-education-industry-report/ukraine-report-html5/index.html)**

## Contents

- [`ukraine_education_report.ditamap`](ukraine_education_report.ditamap): DITA bookmap defining the publication structure.
- [`ukraine_education_report_topics.dita`](ukraine_education_report_topics.dita): DITA topic content.
- [`ukraine_education_report_docbook.xml`](ukraine_education_report_docbook.xml): DocBook 5.0 version of the report.
- [`images/`](images/): Cover image and supporting figures referenced by the XML source.
- [`ukraine-report-html5/`](ukraine-report-html5/): Generated HTML5 report with navigation, stylesheets and images.

## Validation and publishing

- The DITA bookmap contains 80 verified references.
- HTML5 output was successfully built with DITA Open Toolkit 4.4.1 using validation enabled. The resulting table-of-contents navigation was tested in Chrome.
- The DocBook 5.0 XML passed RELAX NG schema validation with `xmllint` and the official DocBook 5.0 schema.

### Reproduce the DITA HTML5 build

With DITA Open Toolkit 4.4.1 installed, run from this directory:

```bash
dita --input ukraine_education_report.ditamap --format html5 --output html5 --validate true
```

### Reproduce DocBook 5.0 validation

Download the official schema from `https://cdn.docbook.org/schema/5.0/rng/docbook.rng` and save it as `docbook.rng` in this directory, then run:

```bash
xmllint --noout --relaxng docbook.rng ukraine_education_report_docbook.xml
```

## Authorship and context

Original report and structured-documentation conversion by Scott Harmer. The report was written in 2021, before Russia's full-scale invasion of Ukraine in February 2022. Its research and projections should not be treated as current.
