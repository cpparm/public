# Engineering Requirement Specifications for ERS

version 1.0

## Scope

This document describes the requirements for Engineering Requirement Specifications, or, the ERS for ERS's. It does not cover non engineering requirements. For instance, "looking nice" is a valid requirement for many products, but it's not an *engineering* requirement.

## Glossary

- **ERS:** Engineering Requirement Specification

## System Description
The goal of the Engineering Requirment Specification is to capture all the product's requimrents. It shall be devleoped after a preliminary understanding of the target customers and their use cases are achieved, and before the product design starts. In writing the ERS, it's imperative not to think about what the design solution looks like. Assume anything can be done. Just focus on what you want the product to do.

This document is written in Markdown. The advantages are:
1. It is simple to write, yet have sufficient layout control for my purpose.
1. It works nicely with source control tools. 
But it's not a requirement.

## Use Cases

| Case ID  | Description |
|:----------|:----------|
| U01   | Product designers document the prodcut requirments in the ERS. |
| U02   | Marketiers check the ERS to verify it captures what the market needs. |
| U03   | Engineers use the ERS to guide what to design in the product. |
| U04   | QA/reliability engineers use the ERS to design validation and test plans. |
| U05 | Sales check the ERS to make sure the sales messages are consistent with what the ERS promises to deliver. |

## Requirements

| Requirement ID  | Description |
|:----------|:----------|
| R001   | There are four required secstions: *Scope*, *Glossary*, *Use Cases*, *Requiremnts*.|
| R002   | There should be a version number at the top of the ERS. The author is free to choose the format of the version number. |
| R003   | An optional section of *Revision History* could follow the version number. It's encouraged to use a source control tool to capture the revision history instead of keeping it in the doucmnet itself. But if you do decide to keep the revision history in the document, each entry should include the author of that revision, the date of that revision, the version number that revision is related to, and a brief and clear description fo the revision. |
| R004 | The *scope* section shall specify what is and is not covered in the ERS. |
| R005 | All acronyms used in the document must be defined in the *glossary* section. |
| R006   | Each use case must have a unique ID. The author is free to choose the format of the ID   |
| R007   | Each requirment must have a unique ID. The author is free to choose the format of the ID   |
| R008   | A requirment has to be verifiable. You can't have a requiremnt "the system must run fast". How fast is fast?   |
| R008  | A requirement can not answer its own question. In otherwords, a requirement can not be the solution. "The door is made of stainless steel" maybe written down as a requirment. If it's a solution to the requirment the door must be strong, then the actual requirement should be written down instead. However, if it's an aesthetic consideration the door must have that specific look, it could be a legitimate requirement.  |
