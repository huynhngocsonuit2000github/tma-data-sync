# Key feature
 
- Role-base access
- Approval workflow
- Audit for document version, tracking
- Generate the document
- Integrate with multiple system/db or there is a centralize db
- E-signature the document
- Notification: study milestones
 
# --------------
 
# 1. Introduction
 
## 1.1. Document Scope
 
- Document is the high-level requirement and product scope for a new Study Setup Portal
- Provide the background and context for the requirement on the new solution
- Basic phase, and the new specific details of each requirement will be updated in the future versions
 
## 1.2. Business Challenges
 
- Currently, to setup a study, they need multiple system to define, build, track, and QC a new study from proposal to live configuration in database
- There is no single source of data for a study. Different between source data proposal and final protocol often differ significantly
- High human manual effort and numerous face-to-face and email interactions for creating study
- Check pieces separately, but not validating the whole thing end-to-end against the original requirement
- Hard to track the status and progress, there is not transparency(stakeholder can not tell who is doing what, what is done, what is delayed)
- Processes aren’t consistent
- Many related operational tasks, external labs, kit preparation, requisitioning of kit and supplies are all manual with no centralized co-ordination and tracking
- Some other challenges that are sometimes required in study setup, that rely on other departments and time consuming
  - Test validation/ new test code creation
  - Custom reference ranges panic value
  - Buy new kit supplies
  - Custom programming
 
## 1.3. Business Drivers (Investigate the solution)
 
- Using one integrated, automated platform to manage workflows, documents, and progress tracking will speedup study startup and improve sponsor involvement and approvals
- Automatically pull data from trusted sources and validate it for example ILs, validate the data, will improve the accuracy, compliance and auditing capabilities for studies going forward
- Currently, there is a high human effort employed across many task in the current process: SUS, other stakeholders such as BD, SA, QC...
- Reduce manual effort, improve quality increase efficiency and accuracy across the study setup, ensure quicker timelines for study startup.
- Reducing study setup periods from weeks to days (To be confirmed on exact savings/benefit), will provide significant competitive advantage for Ic
 
## 1.4. Vision and Benefits
 
- The new Study Setup Portal will expedite Study Setup and provide the following benefit
- Doing less manual quality checking and instead of using automated, ongoing, end-to-end QC wherever possible, so the issue would be caught earlier and more consistently
- Perform as a single source of core study data to avoid duplicate data entry
- [Define-the-context-depend-on-each-stakeholder]
- Status tracking of study setup [across-all-functions]
- Optimized business process execution and reduce costs
  <!-- - Design the system in flexible, independent parts, that is easy to update, reuse, and integrate as needs and technologies evolve -->
 
## 1.5. Key Performance Indicator (KPIs)
 
- Number of metrics we track
- see if we are doing well or need improvement
- make service faster, more reliable and more predictable
  - Setup Cycle Time: time it takes to complete a study setup
  - Amendment Cycle Time: time needed to make and approve changes to an already set-up study
  - Setup Errors: Mistakes or issues found during or after study setup that require correction
  - CAPAs for Study Setup: [Corrective-and-Preventive-Actions] taken to fix setup problems and prevent them from happening again
 
## 1.6. Study Setup Cycle Times:
 
- The following are current metrics being captured for access study setup performance
  - Specification (SL) start data to QC Completion (DB go-live) - [12w-Avg:10.1w]
  - Configuration & QC (Final SL sign off to QC completion) [8w-Avg:6.8w]
  - Gap between study publish and first deliverable (usually kits on site)
 
- These can be broken down further after initial analysis
  - Pre SL 7d -> 2-3d
  - SL creation 2-4w -> 5-7d
  - Study Configuration (IL) 2-4w -> 7d
  - QC 2-3w -> 5d
  - Post QC 10d+ -> 10d
 
# 2. Overview of Study Setup
 
- One portal, one interface, faster and more coordinated study setup.
- Secure role based document generation
- Notify for all stakeholder aware the study milestones, tak assignments and tracked progress
 
# 2.1. Architecture
 
- The new Study Setup Portal will replace SL app, include the study DB configuration that is currently done in ILs
-