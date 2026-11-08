# Specifications of Software Systems

Course materials and project briefs for **CEN 3016: Specifications of Software Systems** at Keiser University, Fall 2026. This repository collects presentations and diagrams used to explore requirements, software architecture, and system specification.

## Course overview

The [syllabus](<Syllabus Spring-2026-Term-CEN-3016-893473-Specifications-Of-Software-Systems Fall 20206 Last.pdf>) covers specification models with well-defined semantics, including algebraic, Petri-net, and model-theoretic approaches. Its learning objectives include specifying systems with UML, modeling simple concurrent systems with Petri nets, understanding temporal logic, and augmenting UML designs with OCL.

The detailed course calendar also covers requirements engineering and Robert C. Martin's *Clean Architecture*: design principles, component cohesion and coupling, boundaries, business rules, and architecture. The Week 9 materials below connect those topics to a practical cancellation scenario.

## Repository contents

### [Week 9: Clean Architecture, chapters 16–20](week-9-chapter-16-20/)

The [lecture presentation](week-9-chapter-16-20/Clean_Architecture_Chapters_16_20.pptx.pdf) covers independence, drawing boundaries, boundary anatomy, policy and level, and business rules. It includes a group activity to model an order cancellation, identify entities and use cases, define boundary contracts, and test the design against changes and competing requests. The syllabus places chapters 18–20 in Week 9; this presentation also reviews chapters 16–17.

### [Week 9 practice: order cancellation and refund timeout](week-9-practice-chapter-16-20/)

The [workshop presentation](<week-9-practice-chapter-16-20/Food Delivery Architecture_ Order Cancellation & Refund Timeout.pptx>) applies Clean Architecture to a prepaid food order canceled when a refund request times out. It explores separating cancellation from payment settlement, use-case and gateway boundaries, stopping kitchen preparation, and retrying refunds through a transactional outbox with idempotency.

### [Final project](final-project/)

The [software architecture and system specification brief](final-project/final-software-spec-proj.pdf) describes Pozool Stays, a rental operations platform, and asks teams to develop an Architecture Design Document for **one** of two features:

- **OTA channel integration:** evaluate direct APIs versus an aggregator and design synchronization, reservation concurrency controls, and scaling.
- **AI-powered direct booking site builder:** design property-data ingestion, generated content, tenant hosting, and a direct-booking checkout.

The brief describes the existing system and its scale targets as the project's design context. It evaluates system modeling and C4 diagrams (35%), technical feasibility and trade-offs (35%), and the final presentation (30%). The folder also includes the [entity relationship diagram](final-project/ERD.svg) and [infrastructure diagram](final-project/Infra.svg) referenced by the brief.

## Viewing the materials

Open the PDFs in a PDF reader, the workshop `.pptx` in a presentation application, and the SVG diagrams in a browser or vector editor. The repository contains course documents and diagrams rather than a runnable application. `mise.toml` specifies Node.js 22.22.2 for the local environment.

## Course references

- Grady Booch, James Rumbaugh, and Ivar Jacobson, *The Unified Modeling Language User Guide*, 2nd edition (required textbook).
- Robert C. Martin, *Clean Architecture: A Craftsman's Guide to Software Structure and Design* (recommended).
- James Robertson, Suzanne Robertson, and Adrian Reed, *Mastering the Requirements Process*, 4th edition (recommended).

Consult the syllabus for the full calendar, evaluation details, and course policies.
