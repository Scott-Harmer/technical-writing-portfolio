# API Documentation Case Study

## Project overview

A technical writing portfolio project demonstrating a docs-as-code workflow for a task-management API. The project uses OpenAPI 3.1, JSON, GitHub and Redocly CLI to connect structured API specifications with validation and rendered developer reference documentation.

## Technical and documentation challenges

API documentation must be accurate enough for developers to work with while remaining readable and navigable. This project demonstrates the relationship between the machine-readable API definition, documentation generation and the checks needed to maintain consistency.

It also illustrates how documentation can be managed as version-controlled source content rather than maintained solely as a separate document.

## Approach and skills demonstrated

- **OpenAPI 3.1 and JSON:** Working with structured specifications to describe an API.
- **Docs-as-code:** Managing documentation alongside source files using GitHub.
- **Documentation validation:** Using Redocly CLI to check specification quality.
- **Developer documentation:** Presenting structured API information as a readable reference.
- **Technical quality assurance:** Connecting source accuracy, validation and published output.

## Project documents

- [Read the API documentation case study (PDF)](api-documentation-case-study.pdf)
- [Inspect the OpenAPI 3.1 source (YAML)](openapi/openapi.yaml)
- [Inspect the bundled OpenAPI specification (JSON)](openapi.json)
- [View the generated API reference (HTML source)](api-reference.html)
- [Inspect the Redocly configuration](redocly.yaml)

The API documentation source, generated reference and validation configuration are included in this portfolio repository. The example describes a fictional Task Management API with five documented operations. The original project records Redocly CLI validation with zero errors and zero warnings.
