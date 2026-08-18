# ResearchPilot Architecture

## Overview

ResearchPilot is an evidence-grounded framework for academic literature analysis.

## V2.1 Pipeline

```text
Active Paper
     ↓
Paper Identification
     ↓
Claim Extraction
     ↓
Source Boundary Gate
     ↓
Source Categorization
     ↓
Provenance Classification
     ↓
Verification Classification
     ↓
Evidence Ledger
     ↓
Contamination / Exclusion Log
     ↓
Findings Analysis
     ↓
Limitations & Research Gaps
     ↓
Overclaim Detection
     ↓
Internal Consistency Check
     ↓
Human Verification



Source Categories
ACTIVE_SOURCE
CITED_SOURCE_WITHIN_ACTIVE_PAPER
EXTERNAL_REQUESTED_SOURCE
UNVERIFIED / OMITTED


Provenance
DIRECTLY_REPORTED
CITED_SOURCE_REPORTED
CALCULATED
INFERRED
NOT_REPORTED
EXTERNAL

Verification
NOT_CHECKED
SOURCE_CHECKED
HUMAN_VERIFIED
EXTERNAL_SOURCE_VERIFIED
