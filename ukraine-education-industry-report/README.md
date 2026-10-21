# Structured documentation: DITA and DocBook 5

## Project overview

This project converts my original 45-page 2021 report, *Ukraine: The Education Industry: Strategic Analysis and Market Outlook*, into two structured documentation formats: DITA/XML and DocBook 5.0. The original report remains available in the [parent project folder](../).

The source files preserve the report's historical context. This is a documentation engineering demonstration, not an updated assessment of the Ukrainian education market.

## Contents

- [`ukraine_education_report.ditamap`](ukraine_education_report.ditamap): DITA bookmap defining the publication structure.
- [`ukraine_education_report_topics.dita`](ukraine_education_report_topics.dita): DITA topic content.
- [`ukraine_education_report_docbook.xml`](ukraine_education_report_docbook.xml): DocBook 5.0 version of the report.
- [`images/`](images/): Cover image and 15 figures referenced by the XML source.

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

Download the official schema from `https://cdn.docbook.org/schema/5.0/rng/docbook.rng`, then run:

```bash
xmllint --noout --relaxng docbook.rng ukraine_education_report_docbook.xml
```

## Authorship and context

Original report and structured-documentation conversion by Scott Harmer. The report was written in 2021, before Russia's full-scale invasion of Ukraine in February 2022. Its research and projections should not be treated as current.
