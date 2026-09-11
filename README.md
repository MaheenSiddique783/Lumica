#  Lumeca Health — Software Systems Capstone Project (ENSE 400)

> **Industry Partner:** Lumeca Health  
> **Academic Institution:** University of Regina — Faculty of Engineering and Applied Science  
> **Course:** ENSE 400 (Design Workshop I)  
> **Supervisor:** Dr. Tim  

---

##  Team Members

* **Maheen Siddique**
* **Gursharan Singh**
* **Ansar**

---

##  Overview

This capstone project focuses on integrating production-ready software modules into **Lumeca Health’s** virtual-care platform. Lumeca Health operates a white-labeled telehealth platform across Saskatchewan and other Canadian regions, connecting patients with doctors and nurse practitioners for remote consultations and appointments.

Rather than building an isolated application from scratch, our engineering team is contributing directly to Lumeca's existing codebase across three potential backlog areas:

1. **Dynamic Post-Consultation Survey System:** An admin-facing survey management module allowing administrators to dynamically configure survey questions and answer choices per client environment, prompting patients post-visit with full English/French localization support.
2. **Inbound & Outbound Fax Management System:** An end-to-end medical faxing infrastructure leveraging a third-party API adapter layer, AWS S3 PDF document handling, database logging tables, and a filterable administrative UI for prescriptions and medical notes.
3. **Legal Document Version Control & Consent Tracking:** An automated audit compliance system that maintains version control across legal agreements (Terms of Service, Privacy Policies, EULAs) and prompts users upon login to review and accept policy updates.

---

##  Technology Stack

* **Backend:** PHP 8 / Laravel Framework, Eloquent ORM
* **Frontend:** Vue.js, HTML5 / SCSS
* **Database:** MySQL
* **File Storage:** AWS S3 (for medical PDF documents and faxes)
* **API & Integrations:** RESTful API architecture with adapter patterns for 3rd-party providers
* **DevOps & Workflow:** Git / GitHub Pull Request reviews, Staging Environment with synthetic test data

---

##  Project Structure

```text
├── docs/                      # Documentation for the project
│   ├── meeting_minutes/       # Notes and minutes from team and stakeholder meetings
│   ├── user_stories/          # User Story Maps and Agile planning documents
│   └── architecture/          # Architecture diagrams and technical design documents
├── src/                       # Source code for the application
│   ├── app/                   # Laravel backend controllers, models, and Eloquent queries
│   ├── database/              # Database migrations and seeders
│   └── resources/js/          # Vue.js frontend components and views
└── tests/                     # Unit, feature, and integration test suites
