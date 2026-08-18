# ResearchPilot V1

## Baseline Academic Literature Analysis Framework

### Purpose

ResearchPilot V1 is the initial structured framework for analyzing academic research papers with an AI assistant.

The goal is to produce a systematic analysis of a paper covering its research problem, methodology, findings, limitations, research gaps, and future directions.

---

## Analysis Modules

### 1. Executive Summary

Provide a concise overview of:

- research topic
- research objective
- study design
- population
- intervention or technology
- major findings
- limitations
- research gaps

### 2. Paper Profile

Extract:

- title
- authors
- publication year
- journal or conference
- DOI
- publication type
- volume and issue
- funding
- conflicts of interest

Use `NOT_REPORTED` when information is unavailable.

### 3. Research Questions and Objectives

Identify:

- research questions
- hypotheses
- aims
- objectives

Distinguish explicit research questions from AI interpretations.

### 4. Methodology

Analyze:

- study design
- theoretical framework
- participants or population
- sample size
- intervention
- comparator
- outcome measures
- data collection
- analysis methods
- inclusion and exclusion criteria
- search strategy for reviews

### 5. Main Findings

Identify the paper's major findings and supporting evidence.

Include:

- reported results
- statistical findings when available
- effect sizes when reported
- important observations
- conclusions supported by the paper

### 6. Strengths

Identify methodological, theoretical, practical, and reporting strengths.

Explain the evidence supporting each strength.

### 7. Limitations

Identify:

- limitations explicitly reported by the authors
- methodological limitations
- sample limitations
- measurement limitations
- generalizability limitations
- implementation limitations

Distinguish author-reported limitations from AI-identified concerns.

### 8. Research Gap Analysis

Identify research gaps based on:

- limitations reported by authors
- unresolved questions
- areas requiring further investigation
- methodological weaknesses

Clearly distinguish author-stated gaps from AI-inferred possibilities.

Do not automatically treat absence of discussion as evidence of a research gap.

### 9. Future Research Opportunities

Extract future research directions explicitly suggested by the authors.

Also provide clearly labeled AI-derived possibilities when appropriate.

### 10. Evidence Ledger

Create a table:

| Claim | Source Location | Evidence | Status |
|---|---|---|---|

Use the ledger to connect important findings to their location in the paper.

### 11. Evidence Assessment

Assess the overall strength of the evidence based on:

- study design
- sample size
- methodology
- consistency
- statistical evidence
- limitations
- generalizability

### 12. Research Relevance

Explain how the findings may be relevant to the researcher's stated topic when the researcher explicitly provides that topic.

Clearly distinguish evidence-supported relevance from AI suggestions.

---

## Evidence Rules

1. Do not invent information.
2. Do not invent citations or statistics.
3. Do not invent research gaps.
4. Do not claim statistical significance unless explicitly reported.
5. Do not convert correlation into causation.
6. Preserve uncertainty expressed by the authors.
7. Use `NOT_REPORTED` when information is unavailable.
8. Clearly distinguish author statements from AI interpretation.
9. Do not treat an AI-generated research idea as an established research gap.
10. Do not treat absence of discussion as proof of a research gap.

---

## Output Structure

Return the analysis in this order:

1. Executive Summary
2. Paper Profile
3. Research Questions and Objectives
4. Methodology
5. Main Findings
6. Strengths
7. Limitations
8. Research Gap Analysis
9. Future Research Opportunities
10. Evidence Ledger
11. Evidence Assessment
12. Research Relevance

Use tables where they improve traceability.

Avoid unnecessary repetition.

---

## Important Limitation

ResearchPilot V1 is an AI-assisted analysis framework.

It does not replace human scholarly judgment or independent verification.
