# Architectural Statement of Needs

The **Architectural Statement of Needs** is a foundational artefact in the architecture lifecycle. It defines the **context**, **drivers**, **principles**, and **requirements** that shape the High-Level Design (HLD). This document sets the tone for architectural thinking — guiding design without prescribing implementation.

## 💡 Why It Matters

This artefact is:

- **Structured enough to guide design** — with clear sections and prompts  
- **Flexible enough to adapt to context** — usable across domains and solution types  
- **Human-readable and Copilot-ready** — designed for manual drafting or AI-assisted authoring  

By formalising this early step, we make architecture **repeatable**, **scalable**, and **ready for automation**.

## 🧭 Where It Fits

The Statement of Needs follows the identification of a business need or opportunity. It precedes the HLD and marks the transition from variable thinking to repeatable patterns:

![Process Flow](./Templates/Process%20Flow/architecture-artefact-flow.png)

> Diagram from [Architectural Process Flow](https://github.com/buildbod/Architecture/blob/main/Templates/Process%20Flow/README.md)

## 🧩Template Contents

The template includes:

- **Problem Statement** – business drivers and pain points  
- **Architectural Vision** – strategic alignment and goals  
- **Architectural Principles** – standards and directives  
- **Initial Solution Intent** – constraints, NFRs, risks  
- **Architectural Runway** – existing capabilities and gaps  
- **Enablers** – technical stories and investigations  
- **Stakeholders and Roles** – contributors and decision-makers  
- **Roadmap Alignment** – delivery milestones and dependencies  

Each section includes **completion guidance** to support clarity, consistency, and traceability.

## 🧱 Framework Mapping

The Statement of Needs aligns with established architecture frameworks such as **TOGAF** and **SAFe**, even if not explicitly named. Here's how it maps:

| **Statement of Needs Section**         | **TOGAF Equivalent**                          | **SAFe Equivalent**                          |
|----------------------------------------|-----------------------------------------------|----------------------------------------------|
| Problem Statement                      | Business Drivers, Architecture Vision         | Strategic Themes, Lean Business Case         |
| Architectural Vision                   | Architecture Vision                           | Portfolio Vision                              |
| Architectural Principles               | Principles Catalog                            | SAFe Lean-Agile Principles                    |
| Initial Solution Intent                | Solution Concept Diagram, Requirements Catalog| Solution Intent, Enabler Epics               |
| Architectural Runway                   | Baseline Architecture                         | Architectural Runway                          |
| Enablers                               | Technical Requirements, Gap Analysis          | Enabler Epics, Capabilities                   |
| Stakeholders and Roles                 | Stakeholder Map Matrix                        | ART Roles, Portfolio Roles                    |
| Roadmap Alignment                      | Architecture Roadmap                          | Program Increments, PI Planning               |

This mapping helps position the Statement of Needs as a **practical bridge** between business strategy and architectural execution, supporting both traditional and agile delivery models.

## 📁 Files

- `architectural_statement_of_needs.docx` – Editable Word version for reuse and adaptation.
- `architectural_statement_of_needs.pdf` – Polished reference version for distribution.

## 🧾 Attribution
This guide uses content adapted from my work at **Mott MacDonald**. Please ensure appropriate attribution if reused or modified.
