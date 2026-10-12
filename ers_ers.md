# Engineering Requirement Specification for ERS Documents

Version 1.1

## Scope

This document specifies requirements for writing an Engineering Requirement Specification (ERS). An ERS captures required product outcomes and constraints, including aesthetic needs and interface constraints such as supported platforms, protocols, and data formats.

This document covers the structure, content, and quality of an ERS. It does not prescribe a particular product design or documentation tool. Aesthetic requirements are included within its scope and are subject to the same verifiability rules as other requirements.

## Glossary

- **ERS:** Engineering Requirement Specification.
- **ID:** Identifier.
- **QA:** Quality assurance.
- **shall:** Indicates a mandated requirement.
- **should:** Indicates a recommendation.
- **may:** Indicates permission.

## System Description
The purpose of an ERS is to give product designers, marketing, engineers, QA, and sales a shared definition of the product's requirements. It connects customer needs and use cases to product design, verification, and sales claims.

The initial ERS establishes the required outcomes before product design begins. Exploring those outcomes without prematurely selecting an implementation helps keep the design open. Known constraints still inform the requirements, and the ERS evolves as feasibility findings and stakeholder needs become clearer. The requirements below define this workflow.

## Use Cases

| Case ID | Description |
|:--------|:------------|
| U01 | Product designers document product requirements in the ERS. |
| U02 | Marketing checks the ERS to verify that it captures customer and market needs. |
| U03 | Engineers use the ERS to guide product design. |
| U04 | QA and reliability engineers use the ERS to develop validation and test plans. |
| U05 | Sales checks the ERS to ensure that sales messages are consistent with the product's specified capabilities. |

## Requirements

| ID | Description | Related use case ID |
|:---|:------------|:--------------------|
| R001 | The ERS shall contain five sections: *Scope*, *Glossary*, *System Description*, *Use Cases*, and *Requirements*. | U01 |
| R002 | The ERS should display a version number at the top of the document. | U01, U03, U04, U05 |
| R003 | A *Revision History* section may follow the version number. | U01 |
| R004 | The *Scope* section shall specify what is and is not covered in the ERS. | U01, U02, U03, U04, U05 |
| R005 | The *Glossary* section shall define every acronym used in the document. | U01, U02, U03, U04, U05 |
| R006 | Each use case shall have a unique ID. | U01, U02 |
| R007 | Each requirement shall have a unique ID. | U01, U03, U04 |
| R008 | Each requirement shall state an observable outcome or constraint and a pass/fail criterion, including applicable operating conditions, units, and tolerances. **Guidance:** "The system must run fast" does not provide a pass/fail criterion. Define the required performance and the conditions under which it is measured. For aesthetic needs, a specified finish or an agreed reference sample can provide a basis for acceptance instead of an undefined judgment such as "looking nice." | U01, U03, U04, U05 |
| R009 | Each requirement shall describe a required outcome rather than select an implementation, unless the implementation is itself a documented external constraint. **Guidance:** Consider "The door is made of stainless steel." If stainless steel is merely the designer's proposed way to make the door strong, state the required load capacity and acceptance criterion instead. If a stakeholder requires that material for its appearance, it may be a legitimate aesthetic constraint. Required platforms, protocols, and data formats may similarly be legitimate interface constraints. R012 and R013 require the source and rationale for these implementation constraints. | U01, U02, U03 |
| R010 | Each requirement shall contain one independently verifiable obligation. **Guidance:** Split compound requirements into separate statements so QA can test them individually. For example, a startup-time requirement and a shutdown-time requirement need separate IDs. Explanations and examples can accompany an obligation within the same description. | U01, U03, U04 |
| R011 | Each requirement shall identify the use case or use cases it supports. | U01, U02, U03, U04, U05 |
| R012 | Each externally imposed implementation constraint shall identify its source. | U01, U02, U03 |
| R013 | Each externally imposed implementation constraint shall include its rationale. | U01, U02, U03 |
| R014 | If a *Revision History* section is included, each entry shall identify the revision's author. | U01, U03, U04 |
| R015 | If a *Revision History* section is included, each entry shall record the revision's date. | U01, U03, U04 |
| R016 | If a *Revision History* section is included, each entry shall identify the document version associated with the revision. | U01, U03, U04, U05 |
| R017 | If a *Revision History* section is included, each entry shall include a brief, clear description of the change. | U01, U03, U04, U05 |
| R018 | Once assigned, an ID shall remain unchanged through document revisions. | U01, U03, U04, U05 |
| R019 | A retired ID shall not be reused. | U01, U03, U04, U05 |
| R020 | Drafting the initial ERS shall follow a preliminary understanding of the target customers and their use cases. | U01, U02 |
| R021 | The initial ERS shall be drafted before product design begins. | U01, U03 |
| R022 | The ERS shall record known constraints affecting the required product outcomes. | U01, U02, U03, U04 |
| R023 | The ERS shall be revised when feasibility findings or stakeholder needs change its requirements. | U01, U02, U03, U04, U05 |

## Authoring Notes

Authors may choose the format of version numbers and IDs. Source control should capture revision history; an in-document *Revision History* section remains optional.

This document uses Markdown because it is simple to write, provides sufficient layout control, and works well with source control. Markdown is not required.
