# ResearchPilot

## Evidence-Grounded AI Framework for Academic Literature Analysis

ResearchPilot is an evidence-grounded AI framework designed to improve **traceability, source control, provenance tracking, and verification** when large language models are used for academic literature analysis.

The framework was developed iteratively through prompt engineering and controlled testing on academic review papers. It evolved from a baseline literature-analysis framework (V1) into a provenance-aware architecture (V2), followed by V2.1 with explicit source-boundary controls and contamination auditing.

> **Important:** ResearchPilot is a research-assistance framework, not an authority. Human verification remains necessary for scholarly use.

---

## The Problem

Large language models can produce useful academic literature summaries, but research workflows create several evidence-traceability problems.

An AI system may blur the distinction between:

- findings directly reported by the active paper
- findings reported by studies cited within a review
- mathematical calculations derived from reported numbers
- AI-generated interpretations
- research gaps explicitly identified by authors
- research gaps inferred by the AI
- information originating from another document in the same working context
- claims that have not actually been verified

ResearchPilot was developed to make these distinctions explicit.

---

# Framework Evolution

ResearchPilot evolved through three major versions:

```text
V1
 │
 │  Baseline literature-analysis framework
 ▼
V2
 │
 │  Provenance + verification architecture
 ▼
V2.1
 │
 │  Source-boundary enforcement
 │  + contamination/exclusion auditing
 ▼
Controlled validation
