# Functional Requirements

## 1. Purpose

This document defines the functional requirements for the AI IT Support Assistant.

The requirements describe the main capabilities that the application must provide in order to support IT support teams in analyzing and processing incidents with the assistance of Generative AI.

---

## 2. Functional Requirements

### FR01 — Create an Incident

The system shall allow an IT support agent to create a new incident.

The incident shall contain the following information:

* Title
* Description
* Application
* Environment

---

### FR02 — Validate Incident Information

The system shall validate the required incident information before submitting the incident for AI analysis.

The following fields shall be mandatory:

* Title
* Description

The system shall display an appropriate validation message when required information is missing.

---

### FR03 — Request AI Analysis

The system shall allow the IT support agent to request an AI-assisted analysis of an incident.

The analysis shall be triggered by an explicit user action.

---

### FR04 — Classify the Incident

The system shall use Generative AI to suggest an incident category.

The available categories shall initially include:

* Access
* Application
* Network
* Performance
* Security
* Hardware
* Other

---

### FR05 — Assess Incident Priority

The system shall use the incident information to suggest a priority level.

The available priority levels shall be:

* Low
* Medium
* High
* Critical

The suggested priority should take into account indicators such as:

* Business impact
* Urgency
* Number of affected users
* Service availability
* Application criticality

The final priority shall remain subject to human validation.

---

### FR06 — Generate Incident Summary

The system shall generate a concise summary of the incident based on the information provided by the user.

The summary should clearly describe the main issue and its impact when this information is available.

---

### FR07 — Identify Possible Root Causes

The system shall use Generative AI to identify potential root causes based on the available incident information.

The generated causes shall be presented as hypotheses to investigate and shall not be considered confirmed technical root causes.

---

### FR08 — Recommend Investigation Actions

The system shall provide recommended investigation or resolution actions based on the incident information and the AI analysis.

The recommendations shall support the IT support agent in determining the next investigation steps.

---

### FR09 — Identify Missing Information

The system shall identify important information that may be missing from the incident description.

Examples may include:

* Error message
* Number of affected users
* Environment
* Time when the incident started
* Application version
* Recent deployment information

---

### FR10 — Review and Validate AI Analysis

The system shall allow the IT support agent to review the generated AI analysis before using it for further incident processing.

AI-generated information shall remain subject to human validation.

---

## 3. Non-Functional Requirements

### NFR01 — Security

The application shall protect sensitive configuration information such as API credentials.

API keys shall not be stored directly in the source code or committed to the Git repository.

---

### NFR02 — Usability

The interface should allow an IT support agent to submit an incident and understand the AI analysis without requiring technical knowledge of Generative AI.

---

### NFR03 — Performance

The application should return the AI analysis within a reasonable response time.

---

### NFR04 — Reliability

The application shall handle AI service errors gracefully and provide an understandable message to the user.

---

### NFR05 — Maintainability

The application shall use a modular architecture to facilitate future changes and the addition of new AI capabilities.

---

## 4. MVP Scope

The following requirements are included in the first version:

* FR01 — Create an Incident
* FR02 — Validate Incident Information
* FR03 — Request AI Analysis
* FR04 — Classify the Incident
* FR05 — Assess Incident Priority
* FR06 — Generate Incident Summary
* FR07 — Identify Possible Root Causes
* FR08 — Recommend Investigation Actions
* FR09 — Identify Missing Information
* FR10 — Review and Validate AI Analysis

The non-functional requirements apply to the overall MVP.
