# Acceptance Criteria

## 1. Purpose

This document defines the acceptance criteria for the main features of the AI IT Support Assistant.

The acceptance criteria describe the expected behavior of the application and provide a basis for functional testing.

---

## AC01 — Create an Incident

### Scenario 1 — Valid incident

**Given** the user is on the incident creation page,

**When** the user enters a title and description and submits the form,

**Then** the system shall create the incident successfully.

### Scenario 2 — Missing title

**Given** the user is on the incident creation page,

**When** the user submits the form without a title,

**Then** the system shall display a validation message indicating that the title is required.

### Scenario 3 — Missing description

**Given** the user is on the incident creation page,

**When** the user submits the form without a description,

**Then** the system shall display a validation message indicating that the description is required.

---

## AC02 — Validate Incident Information

**Given** an incident form is displayed,

**When** one or more required fields are empty,

**Then** the system shall prevent the AI analysis from being requested.

**And** the system shall clearly indicate which information is missing.

---

## AC03 — Request AI Analysis

**Given** a valid incident has been created,

**When** the user clicks "Analyze with AI",

**Then** the system shall send the incident information to the AI service.

**And** the system shall display an analysis result when the AI service responds successfully.

---

## AC04 — Classify the Incident

**Given** an incident is analyzed,

**When** the AI analysis is completed,

**Then** the system shall display a suggested incident category.

The category shall belong to one of the supported categories:

* Access
* Application
* Network
* Performance
* Security
* Hardware
* Other

---

## AC05 — Assess Incident Priority

**Given** an incident is analyzed,

**When** the AI analysis is completed,

**Then** the system shall display a suggested priority.

The priority shall be one of:

* Low
* Medium
* High
* Critical

**And** the system shall indicate that the priority is AI-generated and subject to human validation.

---

## AC06 — Generate Incident Summary

**Given** an incident contains a description,

**When** the AI analysis is completed,

**Then** the system shall display a concise summary of the incident.

---

## AC07 — Identify Possible Root Causes

**Given** an incident has sufficient information for analysis,

**When** the AI analysis is completed,

**Then** the system shall display one or more possible root causes when relevant.

**And** the causes shall be presented as hypotheses rather than confirmed technical facts.

---

## AC08 — Recommend Investigation Actions

**Given** an incident has been analyzed,

**When** the AI analysis is completed,

**Then** the system shall display recommended investigation or resolution actions.

The recommendations should be relevant to the incident information provided.

---

## AC09 — Identify Missing Information

**Given** an incident does not contain sufficient information,

**When** the AI analysis is completed,

**Then** the system shall identify relevant missing information.

Examples may include:

* Error message
* Number of affected users
* Environment
* Time of occurrence
* Application version
* Recent deployment

---

## AC10 — Review AI Analysis

**Given** an AI analysis has been generated,

**When** the user reviews the result,

**Then** the system shall display the AI-generated information clearly.

**And** the user shall remain responsible for validating the analysis before using it for further incident processing.

---

## AC11 — AI Service Error

**Given** the user requests an AI analysis,

**When** the AI service is unavailable or returns an error,

**Then** the application shall display an understandable error message.

**And** the application shall not display the failed AI response as a valid analysis.

**And** the user shall be able to continue handling the incident manually.

---

## AC12 — API Key Security

**Given** the application requires an AI API key,

**When** the project is committed to the Git repository,

**Then** the API key shall not be included in the source code.

**And** sensitive configuration shall be stored using environment variables.

