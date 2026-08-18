# Verification Model

## Purpose

Verification identifies whether an analytical claim has actually been checked.

## Categories

### NOT_CHECKED

The claim has not been independently checked.

### SOURCE_CHECKED

The claim has been checked against the active paper.

### HUMAN_VERIFIED

A human researcher has explicitly checked and verified the claim.

This status must never be assigned automatically by the AI.

### EXTERNAL_SOURCE_VERIFIED

The claim has been checked against an external source that was explicitly requested.

## Key Rule

Verification answers:

> Has this claim been checked?

Verification is independent from provenance.

For example:

`CITED_SOURCE_REPORTED + SOURCE_CHECKED`

means the active paper reports a finding from another study, and the statement has been checked against the active paper, but the original study has not necessarily been verified.
