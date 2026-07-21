# AssessmentTracker Third-Party Services

**Effective Date:** July 20, 2026

> Published from AssessmentTracker, Effective Date July 20, 2026.

---

## Purpose

AssessmentTracker is an internal consulting platform used to perform Operational Excellence Assessments (OEAF) for authorized client organizations.

The Software integrates with selected third-party services to support operational discovery, reporting, and reconciliation activities. This document identifies those services and clarifies their relationship to AssessmentTracker.

---

## Third-Party Services

AssessmentTracker currently integrates with the following third-party platforms:

### Microsoft Graph

**Provider:** Microsoft Corporation

Microsoft Graph provides secure access to authorized Microsoft 365 resources through Microsoft's OAuth authorization framework.

Current AssessmentTracker usage includes:

- Outlook Calendar metadata
- Outlook Email metadata
- Microsoft 365 operational discovery
- Read-oriented operational assessment

Authentication is performed directly through Microsoft's OAuth authorization system.

AssessmentTracker does not collect, transmit, or store Microsoft account usernames or passwords.

---

### QuickBooks Online

**Provider:** Intuit Inc.

QuickBooks Online provides secure access to authorized accounting information through Intuit's OAuth authorization framework.

Current AssessmentTracker usage includes:

- Company information
- Customer information
- Estimates
- Invoices
- Payments
- Operational reporting
- Reconciliation support

Authentication is performed directly through Intuit's OAuth authorization system.

AssessmentTracker does not collect, transmit, or store Intuit account usernames or passwords.

---

## Authorization

AssessmentTracker accesses third-party services only after authorization has been granted by the owner of the connected account.

Authorization is obtained through the provider's own OAuth consent process.

The account owner may revoke AssessmentTracker's access at any time using the provider's own account management tools.

---

## Data Usage

Information retrieved from connected services is used solely to support the consulting engagement for which authorization was granted.

AssessmentTracker does not:

- Sell retrieved information
- Broker retrieved information
- Display advertising
- Use advertising or marketing trackers
- Perform behavioral profiling
- Access information beyond the permissions granted through OAuth authorization

---

## Data Storage

AssessmentTracker follows a local-first architecture.

OAuth access tokens, refresh tokens, retrieved metadata, workpapers, findings, and operational reports are stored locally on the consultant's secured workstation unless the client explicitly authorizes another storage location.

AssessmentTracker does not operate a centralized cloud service for storing client operational data.

---

## Service Availability

AssessmentTracker depends upon the availability of third-party services.

Microsoft Graph and QuickBooks Online are operated independently by Microsoft Corporation and Intuit Inc., respectively.

AssessmentTracker cannot guarantee the availability, accuracy, completeness, or continued operation of any third-party service.

Changes made by a third-party provider—including API changes, authentication changes, service interruptions, or discontinued functionality—may affect AssessmentTracker's operation.

---

## Third-Party Terms and Policies

Use of connected services remains subject to the terms, conditions, and privacy policies established by their respective providers.

AssessmentTracker does not replace or supersede those agreements.

Users should consult the providers' official documentation for current terms and privacy practices.

Current providers include:

- Microsoft Corporation
  - Microsoft Services Agreement
  - Microsoft Privacy Statement

- Intuit Inc.
  - Intuit Terms of Service
  - Intuit Privacy Statement

---

## Future Integrations

AssessmentTracker may integrate with additional business systems in future releases to support authorized consulting engagements.

Examples may include:

- Customer Relationship Management (CRM) platforms
- Enterprise Resource Planning (ERP) systems
- Payroll systems
- Document management platforms
- Other client-authorized operational systems

Future integrations will follow the same architectural principles:

- Explicit account-owner authorization
- Least-privilege access
- OAuth or equivalent secure authentication where available
- Read-oriented operational discovery unless additional authorization is granted

---

## Questions

Questions regarding AssessmentTracker's use of third-party services may be directed to:

**Peter Holdorf**

Email: **PeterHoldorf18@gmail.com**