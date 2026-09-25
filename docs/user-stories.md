# User Stories

## 1. Purpose

This document defines the main user stories for the AI IT Support Assistant.

The user stories describe the expected behavior of the application from the perspective of its users.

---

## US01 — Create an Incident

**As an** IT support agent,

**I want to** create a new incident by entering the relevant information,

**so that** the incident can be analyzed and processed.

### Related Requirement

FR01 — Create an Incident

---

## US02 — Validate Incident Information

**As an** IT support agent,

**I want to** receive a validation message when required information is missing,

**so that** I can provide complete information before requesting an AI analysis.

### Related Requirement

FR02 — Validate Incident Information

---

## US03 — Analyze an Incident with AI

**As an** IT support agent,

**I want to** request an AI-assisted analysis of an incident,

**so that** I can quickly obtain structured information about the issue.

### Related Requirement

FR03 — Request AI Analysis

---

## US04 — Classify an Incident

**As an** IT support agent,

**I want the system to** suggest an incident category,

**so that** I can better understand the type of issue and route it to the appropriate team.

### Related Requirement

FR04 — Classify the Incident

---

## US05 — Assess Incident Priority

**As an** IT support agent,

**I want the system to** suggest an incident priority,

**so that** I can evaluate the potential urgency and impact of the incident.

### Related Requirement

FR05 — Assess Incident Priority

---

## US06 — Generate an Incident Summary

**As an** IT support agent,

**I want the system to** generate a concise summary of the incident,

**so that** I can quickly understand the main issue without reading the entire description.

### Related Requirement

FR06 — Generate Incident Summary

---

## US07 — Identify Possible Root Causes

**As an** IT support agent,

**I want the system to** suggest possible root causes,

**so that** I can use them as investigation hypotheses.

### Related Requirement

FR07 — Identify Possible Root Causes

---

## US08 — Get Recommended Actions

**As an** IT support agent,

**I want the system to** suggest investigation or resolution actions,

**so that** I can identify relevant next steps.

### Related Requirement

FR08 — Recommend Investigation Actions

---

## US09 — Identify Missing Information

**As an** IT support agent,

**I want the system to** identify missing information,

**so that** I can collect the information required to investigate the incident.

### Related Requirement

FR09 — Identify Missing Information

---

## US10 — Review AI Analysis

**As an** IT support agent,

**I want to** review the AI-generated analysis before using it,

**so that** I can validate the information and remain responsible for the final decision.

### Related Requirement

FR10 — Review and Validate AI Analysis

---

## US11 — Handle AI Service Errors

**As an** IT support agent,

**I want the system to** inform me when the AI analysis cannot be completed,

**so that** I understand that the analysis is unavailable and can continue the incident handling manually.

### Related Requirement

NFR04 — Reliability

---

## User Story Mapping

| User Story | Requirement | Main Feature        |
| ---------- | ----------- | ------------------- |
| US01       | FR01        | Create incident     |
| US02       | FR02        | Input validation    |
| US03       | FR03        | AI analysis         |
| US04       | FR04        | Classification      |
| US05       | FR05        | Priority            |
| US06       | FR06        | Summary             |
| US07       | FR07        | Possible root cause |
| US08       | FR08        | Recommended actions |
| US09       | FR09        | Missing information |
| US10       | FR10        | Human validation    |
| US11       | NFR04       | Error handling      |

