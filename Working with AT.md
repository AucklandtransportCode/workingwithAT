>   **Working with Auckland Transport**

### Minimum Engagement Criteria (MEC) for Technology

### Date: 29/8/2019

### Next Review Date: 29/8/2020

>   Version: 1.0

Background
==========

Auckland Transport (AT) is a Council Controlled Organisation which employs a
variety of technology solutions. In the course of selecting and implementing
this technology it is important for AT to maintain consistence and control of
those technologies to provide a secure cost-effective service to Auckland.

Purpose
=======

The purpose of the MEC is to set standards for vendors, partners and affiliates
to provide technology services and equipment to Auckland Transport

Auckland Transport’s Business Technology Office (BTO) is the authorative group
for the creation, amendment and approval of all technology related policies and
standards. The MEC is a summary collection of those standards and policies and
serves as a quick reference to some of the main points of engagement. In nearly
all cases more detailed review of the relevant policy or standards is required.

Scope
=====

These criteria apply to all technology services and solutions in place, proposed
and planned by both Auckland Transport and any third party providing those
services and solutions

1.  All Cloud and hybrid services

2.  Software as a Service (SaaS)

3.  On premise

Auckland Transport recognises that solutions presented as; wholly managed, or
software as a service may not comply completely with the standards set out in
this document. Auckland Transport will not compromise standards that may
diminish the return to the public of Auckland, nor will it place at material
risk the confidentiality, availability or integrity of the services it provides.

If a provider or vendor believes that their proposal supports the objectives of
these standards but differs significantly in their delivery, an application for
exception may submitted to the BTO. The submission will be reviewed against the
following criteria:

1.  Strategic value - the proposal will reshape AT’s technology strategy

2.  Operational mass – The scale of the solution is such that it can sustain
    its’ own support services and infrastructure without materially reducing the
    value of the business case

3.  Demonstrable alignment – equivalent or better standards can be mapped
    without materially reducing the value of the business case

4.  Targeted value – The proposal targets a niche requirement and has negligible
    impact on support, costs or architecture

Strategic Requirements

When evaluating services and solutions Auckland Transports Business Technology
team will assess the suitability based on the following four key decision
points. These are in no priority and each is weighted according to the use case

1.  Business Agility

2.  Cost

3.  Business continuity

4.  Security

Each proposed solution will be assed against these requirements for its relative
strengths and weaknesses. Each requirement encompasses a broad range of decision
points e.g. technical debt, support costs, speed to deploy, response velocity
etc.

Section One
===========

1.  Service Management

    1.  AT uses ServiceNow as its technology service management tool. All
        incidents, changes and requests must be tracked through AT’s ServiceNow.
        Third parties may integrate with AT’s ServiceNow (at their cost) or
        manually synchronise tickets if they wish to maintain their own service
        management queues.

        1.  **Incident Management** - Incidents must be logged and tracked in
            AT’s ServiceNow

        2.  **Change Management** - Only AT’s Change Board may approve changes
            to Pre-production and Production environment.

        3.  **Change Control** – Proposed changes must be lodged with the AT
            Change Team at least two days before the AT Technical Advisory Board
            (TAB) meets

        4.  **Peer Review** – All changes must be Peer Reviewed by a member of
            the AT Operations Team not already involved with the work.

        5.  Invoices for support will only be approved with a breakdown of work
            with an associated AT incident, request or change number.

2.  Transition to Production

    1.  A service or solution is in “Production” when it is in use either
        directly or indirectly by AT customers or supporting an AT business
        process or function.

    2.  Documentation required is detailed in section 4 Documentation

    3.  Transition to production must be approved by the Technical Advisory
        Board

    4.  A “soft launch” has the same requirements as a full transition

    5.  A “Feature Flag” release has the same requirements as a full transition

    6.  SaaS and Hybrid solutions are required to meet the same production
        standards are on premise solutions. Where a support feature is managed
        by the solution provider the transition documentation must reference the
        support contract clause that meets the requirement.

    7.  Evergreen products in addition to complete documentation must manage a
        formal change and adoption process including internal market
        segmentation, persona development and ring deployment.

    8.  Production Requirements

        ![](media/f1eef9c4cbdad84e4b7e39a462c22446.png)

3.  Service Level Agreements

    1.  Each service or solution must have an SLA that matches AT’s business
        operations.

    2.  This will include:

        1.  Availability expressed as a percentage calculated monthly

        2.  Response time to a notified incident

        3.  Communication frequency

        4.  Restore Time Objective (RTO)

        5.  Restore Point Objective (RPO)

4.  Documentation

    1.  Documentation will comply with AT’s record management policies and use
        Auckland Transport templates.

    2.  Solution documentation will at a minimum include:

        1.  Service Desk Guide

        2.  Operations guide

        3.  Implementation guide

        4.  As built

    3.  If Azure DevOp’s (ADO) is being used for deployment and ongoing backlog
        management system documentation may be maintained in an ADO wiki or AT’s
        Git in Markdown

    4.  Evergreen solutions also require the following:

        1.  Product road map

        2.  User persona’s

        3.  User market segmentation

5.  Disaster Recovery

    1.  Auckland Transport makes a clear distinction between Disaster Recovery,
        High Availability and Business Continuity:

        1.  **DR**- The ability to restore a service within SLA’s

        2.  **HA- Hot/Warm/Cold** inherit resilience of a service. HA may be
            applied to the entire service or targeted vulnerabilities

        3.  **Business Continuity**- business contingency planning in the event
            of an outage

    2.  The requirement for DR or HA is determined by the contracted service
        level agreements. Where possible the service should be immutable in
        production to facilitate automated deployment. The intent is that issues
        are resolved by redeploying last known good.

    3.  DR from media must be tested to operation every six months.

    4.  HA fail over and fail back must be tested every six months

    5.  Business Continuity planning will be reviewed every 12 months in
        cooperation with the Auckland Transport service manager

6.  Operating Systems

    1.  AT will support the following server operating systems:

        1.  Windows server 2016

        2.  Windows Server 2019

        3.  RedHat 7.6, 7.7

7.  Virtual Machine Sizing

    1.  Cloud virtual machines will be size to the minimum specification
        required to run the service.

    2.  Machines may be set to auto-scale if load is variable

8.  Network

    1.  IP addresses ranges are managed allocated by AT network team

    2.  Physical network infrastructure must be approved by the AT Network team
        before design approval

    3.  IaaS IP addressing must by assigned by DHCP

9.  Security

    1.  Technologies and architectural patterns not already in use in Auckland
        Transport must be reviewed and approved by AT’s Security team before
        acceptance.

    2.  Advice should be sought from the AT Security team on currently
        acceptable standards and protocols for data in motion and data at rest.

    3.  Authentication that is not Microsoft Active Directory or MS Azure AD
        integrated must be approved by the Security team.

    4.  Third party use of AT cloud services is only permissible with Microsoft
        365 Guest Accounts. The accounts are not provided by AT.

    5.  External facing services must not connect directly to internal services

    6.  Unencrypted protocols are not permitted outside of AT’s corporate
        network and must not cross security boundaries

10. Deployment Environments

    1.  Code repositories must be in either AT’s Azure DevOp’s (ADO) or Git

        1.  <https://aucklandtransport.visualstudio.com>

        2.  <https://github.com/AucklandtransportCode>

    2.  Auckland Transport’s Digital delivery is built on Microsoft Azure
        DevOp’s:

        1.  Backlogs, sprint/iteration planning, tasks, Kanban,

        2.  CICD

        3.  Release

        4.  Test Management

    3.  Detailed standards and processes on AT’s Application Lifecycle
        Management and the use of ADO are in the ALM Wiki

    ![](media/fef2bb254b2a5797e6b2dad2b3f85a62.png)

11. Product Management

    1.  Backlogs are prioritised by a stakeholder representative working group

    2.  Prioritised work is scoped by at Business Technology technical team

    3.  AT’s Product Management is a part of the wider ATDx program

![](media/794905b49a5b05421b7eccdedd6e5588.png)

1.  Integration

    1.  Azure Logic App’s are AT’s standard for integration in Azure

    2.  On-premise integration will use Kafka unless directed by the AT
        Architecture team

    3.  Personal workflow services (such as 365 Flow) will not be used for
        corporate applications.

2.  Workflow

    1.  Business logic workflow may use the following:

        1.  Logic App’s

        2.  Nintex

        3.  Dynamics CRM

        4.  Personal workflow services (such as 365 Flow) will not be used for
            corporate applications

3.  Database

    1.  MS SQL Server 2012

    2.  MS SQL Server 2014

    3.  MS SQL Server 2016

    4.  Azure Cosmos DB

    5.  Azure SQL Database

    6.  SQL Server on Virtual Machines

    7.  SQL Data Warehouse

    8.  Azure Database Migration Service

    9.  Azure Cache for Redis

4.  Data Policies

    1.  Business system/applications must meet the requirements of the
        Information & Records Management compliance as per PRA2005, and IRM
        standard as issued by the Chief Archivist.

    2.  Documentary information must integrate/interface with AT’s
        auto-classification system to enable the tagging (incl. retention
        tagging) of documents.

    3.  External contractors working for or on behalf of AT must have a
        contractual Recordkeeping clause so that all records created and
        maintained when carrying out any AT business be captured and maintained
        in AT’s prescribed documentary information system. For project
        information that is 365 Project Online and Fulcrum

5.  Analytics

    1.  All reporting and visualisations must be developed using AT’s enterprise
        reporting tool; Power BI. No new development is to be done in AT’s
        legacy reporting tool – Business Objects without the approval of the
        Information Delivery Manager. This approval must be gained upfront.

    2.  Peer Review – All designs and development, both data model and
        visualisation must be peer reviewed by a member of the Information
        Delivery team not already involved with the work. Solution design must
        be reviewed and approved before development starts.

    3.  Any associated ETL work must also be reviewed and signed off by the Data
        Delivery team before UAT starts.

    4.  UAT must not start until all development has been reviewed and approved.

    5.  Any development done outside of the Information Delivery team will not
        be supported or maintained by the central Information Delivery team
        until the ‘Handover to BAU’ process has been completed and signed off
        for approval by either the Information Delivery Tech Lead or the
        Information Delivery Manager. Any development that does not meet the
        Enterprise Reporting and Analytics standards will need to be redeveloped
        using AT best practice and standards and will not be deployed to the
        Production environment until that standard is met.

    6.  Documentation will comply with AT’s record management policies and use
        Auckland Transport templates.

    7.  Solution documentation will at a minimum include:

    8.  SSaS Peer Review template (if using SSaS for data model)

    9.  Reporting Peer Review template

    10. BAU Handover template (if development is to be supported and maintained
        by Enterprise Reporting and Analytics team)

    11. Upon commencement of a Reporting, Analytics or Advanced Analytics
        project, the contractor or PM must make themselves and their project
        known to the Information Delivery Manager with delivery timelines so
        that appropriate resource can be made available to that project for the
        review processes.

    12. Any support time required by the Information Delivery team up until it
        is accepted into BAU will be charged to the corresponding Project or WRB
        code.

6.  Risk and Compliance

    1.  Computer operation controls are in place

    2.  To be demonstrated that a regular software patching process is in place

    3.  Demonstrate the approval process for elevated access to systems

    4.  Data centre physical security controls are in place

    5.  Evidence that only authorised personnel have data centre access

    6.  System development life cycle (SDLC) controls are in place

    7.  Evidence that a process for developing software includes a life cycle
        (Plan/Build/Test/Deploy/Maintain)

    8.  Cloud Risk Assessment has been done (e.g. Completing the DIA [Department
        of Internal Affairs checklist)

        1.  Evidence that the checklist has been completed and sent back to AT

    9.  Internet exposed services must pass a security penetration test in
        pre-production and production.

    10. Once these criteria have been accepted by the supplier/vendor they
        should then become part of the MSA (Master Services Agreement)

    11. The vendor has implemented a security framework (e.g ISO270001, NIST,
        PCIDSS or a similar accepted framework)

    12. Logical access controls over applications, data and supporting
        infrastructure exist

    13. Demonstrated by way of a Policy or similar document that defines how the
        organisation manages access to systems that store AT data

    14. Program change management controls exist

    15. Demonstrated by a Change Control Policy or evidence of a formal change
        control process

7.  Architecture

    1.  Solution designs must comply with standards outlined and referenced
        material in this document.

    2.  Where available Designs must use approved AT blueprints

    3.  All designs must be approved by the Design Review Board (DRB)

    4.  Submissions to the DRB must be made by an Auckland Transport Solution
        Architect

8.  MVP, PoC, PoV

    1.  **Minimum Viable Product** (MVP) is a fully functioning supported
        production system and is subject to the same standards and reviews as a
        full production system.

    2.  An MVP is characterised by a limited feature set that allows an early
        release to market. The solution must have testing and support structures
        no less than a fully featured product

    3.  **Proof of Concept** (PoC) Must never be released into production and
        must not be used as the start point for a production build.

    4.  A PoC serves only to validate a design and must be decommissioned after
        successful design review by the BTO

    5.  **Proof of Value** (PoV) extends a PoC to validate the problem statement
        of a business case. The same rules apply for PoV’s as PoC’s

9.  Supported Browsers

    1.  Microsoft Internet Explorer 11

    2.  Microsoft Edge

10. Mobile Applications

    1.  Must be available in both the Apple App Store and the Google Play Store

    2.  Only the AT Online team will have access to the store.

    3.  All releases will be manged by the AT Online team

11. Immutable Infrastructure

    1.  All server implementations must be automated using the current AT
        standard image unless approved by the BTO

    2.  Each service will have three environments:

        1.  Test – manual deployment from template – Change control not required

        2.  Pre-production – CICD deployment with manual intervention – Change
            notification required

        3.  Production – CICD deployment, immutable infrastructure IaC –
            Standard Change approval required

12. Development and Proof of Concept

    1.  Development work should be carried out in a suppliers’ own environment
        at their cost.

    2.  Where integration or AT specific services are necessary development or a
        PoC can be carried out in AT’s Azure Development subscription. At the
        end of the initial development the environment will be deleted.

    3.  To move a service from development to test a template is taken of the
        solution and deployed manually into an environment in the Test
        subscription. Change control is not required.

    4.  Before moving to test a cost for budget must be approved

13. Geographical Information Systems (GIS)

    1.  Auckland Transport has a GIS team responsible for managing, maintaining,
        developing and presenting all geospatial data.

    2.  All geodata must be approved and managed by AT’s GIS team

    3.  Google Map’s is not to be used

    4.  ESRI is AT’s standard for geospatial information

    5.  FME is AT’s standard for GIS data integration

14. Directory Authentication

    1.  Applications must be able to authenticate to Azure Active Directory
        (AAD)

    2.  The prime source for groups and security is currently Microsoft Active
        Directory (AD) but AT’s strategic direction is to move to Azure AD.

Section 2
=========

Breach of Policy
================

1.  Breach of this policy may result in disciplinary action, including where
    appropriate, summary dismissal (as set out in Auckland Transport’s
    Discipline and Dismissal Policy).

2.  Failure to comply by a supplier, contractor or vendor to Auckland Transport
    may result in the termination of any related agreement or initiate a
    contracted dispute process.

3.  Failure to meet these standards in a Request for Information (RFI) or a
    Request for Purchase or other tender or procurement process may immediately
    disqualify any proposal.

Related Documents
=================

1.  ATDx

2.  AT.ALM Wiki

3.  Information and Records Management Policy

4.  Information and Records Management Standards

5.  IT Access Policy

6.  Mobile Device Guidelines

7.  Mobile Device Policy

8.  Procurement Policy

9.  DIA Cloud Risk Assessment Process

Related Legislation
===================

1.  Public Records Act 2005

2.  Privacy Act 1993

3.  Local Government and Official Meetings Act 1987

Revision History 
=================

| **Date** | **Authored by** | **Approved by** | **Ver.** | **Notes**     |
|----------|-----------------|-----------------|----------|---------------|
|          |                 | EGM Technology  | 1.0      | Initial draft |
|          |                 | EGM Technology  | 1.0      | Final version |
|          |                 |                 |          |               |

Authority
=========

| **Owner**                                   | ELT (Roger Jones)                     |               |   |
| (contact for updates, clarity etc)          |                                       |               |   |
|---------------------------------------------|---------------------------------------|---------------|---|
| **Stakeholders for consultation**           | All Auckland Transport Business Units |               |   |
| **Authorised by**                           | Chief Executive                       |               |   |
| **Name**                                    | Shane Ellison                         | **Signature** |   |
| **Version no**                              | Date as on front cover                |               |   |
| **Issue date**                              |                                       |               |   |
| **Review date**                             | Date as on front cover                |               |   |

Appendices
==========
