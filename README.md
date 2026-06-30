# ServiceNow Cybersecurity ITSM & Incident Response Workflow Lab

## Project Overview

This project uses a ServiceNow Personal Developer Instance to simulate cybersecurity-focused ITSM workflows. Instead of building a basic help desk ticketing lab, this project demonstrates how security incidents can be documented, prioritized, assigned, escalated, remediated, and reported using ServiceNow.

The lab focuses on practical security operations workflows such as phishing intake, suspicious login escalation, vulnerability remediation, CMDB asset mapping, change management, knowledge articles, and reporting.

## Project Goal

The goal of this project is to demonstrate how cybersecurity operations rely on structured ITSM processes after an alert or user report is identified.

This lab shows how a security analyst can:

* Create and triage security incidents
* Link incidents to affected CMDB assets
* Assign tickets to the correct security teams
* Prioritize incidents using impact and urgency
* Escalate suspicious login activity from SOC to IAM
* Track vulnerability remediation through change management
* Document investigation steps using work notes
* Create knowledge articles for repeatable security procedures
* Build reporting visibility for security incidents

## Lab Environment

* ServiceNow Personal Developer Instance
* Incident Management
* Change Management
* Configuration Management Database
* Knowledge Management
* Reporting

## Simulated Organization

**Company:** MapleTech Financial Services

This fictional organization was created to simulate an enterprise environment with endpoints, servers, cloud assets, identity systems, and security operations teams.

## Cybersecurity Assignment Groups

The following assignment groups were created to simulate real security and IT operations ownership:

| Group                               | Purpose                                                                                        |
| ----------------------------------- | ---------------------------------------------------------------------------------------------- |
| Cyber Lab - SOC Tier 1              | Initial triage of security alerts, phishing reports, suspicious login activity, and escalation |
| Cyber Lab - IAM Security Team       | Reviews account compromise, unauthorized access, lockouts, and identity-related incidents      |
| Cyber Lab - Infrastructure Security | Handles endpoint/server remediation, security patching, and vulnerability tickets              |
| Cyber Lab - Cloud Security Team     | Handles AWS/cloud misconfiguration, logging, access control, and cloud remediation tickets     |
| Cyber Lab - Change Advisory Board   | Reviews remediation changes that may affect production systems                                 |
| Cyber Lab - Service Desk L1         | Receives user-submitted IT/security reports and escalates confirmed security issues            |

## Lab Users

Sample users were created to represent employees and security team members:

| User           | Role                                    |
| -------------- | --------------------------------------- |
| Alex Morgan    | Employee reporting phishing             |
| Priya Shah     | SOC analyst                             |
| Daniel Lee     | IAM analyst                             |
| Marcus Chen    | Cloud security analyst                  |
| Sarah Thompson | Infrastructure security analyst         |
| Krish Patel    | Security operations analyst / lab owner |

## CMDB Assets

The following configuration items were created to simulate enterprise assets:

| Configuration Item | Asset Type          | Purpose                                                                     |
| ------------------ | ------------------- | --------------------------------------------------------------------------- |
| DC01               | Server              | Domain controller used for suspicious login and brute-force alert workflows |
| WIN10-CLIENT01     | Workstation         | Endpoint used for phishing and vulnerability remediation scenarios          |
| WAZUH-SIEM01       | Server              | SIEM/log monitoring server used to simulate alert intake                    |
| AWS-WEB01          | Cloud Server        | Public-facing cloud server used for cloud misconfiguration workflow         |
| AWS-APP01          | Cloud Server        | Private application server used for cloud segmentation workflow             |
| VPN-GATEWAY01      | Network Device      | Remote access gateway used for access review workflows                      |
| M365-TENANT01      | Application Service | Email/collaboration service used for phishing report workflow               |

## Security Incident Scenarios

### 1. Phishing Email Report

A user reported a suspicious Microsoft 365 login verification email. The ticket was assigned to SOC Tier 1, linked to the M365 tenant configuration item, prioritized as a high-priority security incident, and documented with SOC triage work notes.

**Key actions demonstrated:**

* User-reported phishing intake
* SOC assignment group routing
* Affected CI mapping
* Work note documentation
* User guidance and investigation steps

### 2. Suspicious Login / Brute-Force Alert

A simulated SIEM alert indicated multiple failed login attempts against DC01. The incident was initially assigned to SOC Tier 1 and then escalated to the IAM Security Team for identity review.

**Key actions demonstrated:**

* Critical incident prioritization
* DC01 asset mapping
* SOC triage documentation
* SOC-to-IAM escalation
* Identity review workflow

### 3. Vulnerability Remediation

A simulated vulnerability scan identified a critical missing security patch on WIN10-CLIENT01. The incident was assigned to Infrastructure Security and linked to a formal change request for remediation.

**Key actions demonstrated:**

* Vulnerability remediation tracking
* Endpoint CI mapping
* Risk assessment documentation
* Change request creation
* Patch planning and remediation evidence

## Change Management Workflow

A normal change request was created to remediate the simulated vulnerability on WIN10-CLIENT01.

The change request included:

* Configuration item: WIN10-CLIENT01
* Priority: High
* Risk: Moderate
* Impact: High
* Assignment group: Cyber Lab - Infrastructure Security
* Implementation plan
* Backout plan
* Test plan
* Affected CI linkage

This demonstrates how vulnerability remediation can be managed through formal change control to reduce operational risk and maintain evidence of approval, testing, and rollback planning.

## Knowledge Articles

Knowledge articles were created to document repeatable security procedures.

Planned or created SOPs include:

* Phishing Email Triage SOP
* Vulnerability Remediation and Change Request SOP
* Suspicious Login Alert Response SOP

These articles help standardize security response steps and improve documentation quality.

## Reporting

A report was created to show cybersecurity incidents by assignment group using the filter:

`Short description contains SECURITY`

This report provides visibility into how security incidents are distributed across SOC, IAM, and Infrastructure Security teams.

## Screenshots

Screenshots are stored in the `screenshots/` folder.

Recommended screenshots:

1. ServiceNow PDI homepage
2. Cybersecurity assignment groups
3. Lab users
4. SOC Tier 1 group members
5. CMDB asset list
6. DC01 CI record
7. AWS-WEB01 CI record
8. Phishing security incident
9. Suspicious login IAM escalation
10. Vulnerability remediation incident
11. Patch change request
12. Vulnerability incident linked to change request
13. Knowledge article
14. Security incident report

## Skills Demonstrated

* ServiceNow ITSM
* Incident Management
* Change Management
* CMDB
* Knowledge Management
* Security incident triage
* SOC workflow documentation
* IAM escalation
* Vulnerability remediation tracking
* Cloud security workflow
* Risk-based prioritization
* Work notes and closure evidence
* Security operations reporting

## Lessons Learned

This lab helped demonstrate that cybersecurity operations are not only about identifying alerts. A strong security workflow also requires documentation, prioritization, assignment, escalation, remediation tracking, change control, and evidence-based closure.

By using ServiceNow ITSM, this project shows how security teams can manage incidents in a structured and auditable way across SOC, IAM, Infrastructure, and Cloud Security functions.

## Project Status

Core workflow completed:

* Assignment groups created
* Lab users created
* CMDB assets created
* Security incident tickets created
* SOC-to-IAM escalation documented
* Vulnerability remediation incident created
* Change request created
* Knowledge article workflow started
* Security incident reporting configured

Future improvements:

* Build a full dashboard with multiple security reports
* Add SLA rules for critical and high-priority security incidents
* Add more cloud security and IAM scenarios
* Link knowledge articles directly to incidents
* Add more detailed incident closure documentation
