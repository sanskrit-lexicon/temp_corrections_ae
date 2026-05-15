# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**temp_corrections_ae** is a working repository for analyzing and applying English word corrections to the AE (Apte English-Sanskrit), BHS, BOR, MWE, and PGN dictionaries.

## Architecture

| File | Purpose |
|---|---|
| `ae.txt` / `ae_error.txt` | AE entries and English spelling errors |
| `bhs.txt` / `bhs_error_todo.txt` | BHS entries and remaining errors to review |
| `bor.txt` / `bor_error.txt` | BOR entries and errors |
| `mwe.txt` / `mwe_error.txt` | MWE entries and errors |
| `pgn.txt` | PGN entries for review |

## Workflow

1. Start from error lists (from CORRECTIONS repo's English spell-check pipeline)
2. Cross-reference entries across dictionaries to distinguish errors from intentional usage
3. Apply confirmed corrections via `updateByLine.py` to `csl-orig` source files

## Dependencies

- **Python 3**
- **CORRECTIONS** sibling repo — source of the error lists
