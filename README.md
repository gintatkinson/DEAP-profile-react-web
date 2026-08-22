# Digital Engineering Agent Platform (DEAP) — React Web Profile

> **Repository Identifier:** `DEAP-profile-react-web`  
> **Repository Role:** `TECHNOLOGY_PROFILE_TEMPLATE` (React TypeScript Web Implementation Profile)  
> **Classification:** `Web Interface & Operator Console Technology Profile`  
> **Primary Technology Profile:** `React 18 / TypeScript / Vite`  

---

## 1. Overview

This repository provides the **React Web Technology Profile** (`DEAP-profile-react-web`) for the Digital Engineering Agent Platform (DEAP). It supplies baseline templates, LUI bindings, type validations, and build configurations for downstream web consoles, telemetry dashboards, and operator interfaces.

### 1.1 Primary Commercial Toolchain Integration Context

This platform explicitly declares **MATLAB / Simulink / Stateflow / Embedded Coder** as the Primary Tier-1 Commercial Toolchain Integration Context (Model-Based Design, Control Law Synthesis, DO-178C C/SPARK Ada code generation).

---

## 2. Directory Structure

- `web_react/`: Baseline React + TypeScript application template with Vite.
- `rules/`: Profile-specific governance rules (e.g. `react-lui-binding.md`, `latex-katex-integrity.md`).
- `schema/`: Contract definitions and SysML v2 schemas.
- `scripts/`: Modular installer and downstream verification scripts.
- `tests/`: Automated baseline verification test suite.

---

## 3. Verification & Quality Gates

Execute baseline and profile verification:

```bash
# Run baseline environment and integrity tests
pytest tests/

# Run downstream conformance gate
python3 scripts/verify_downstream_baseline.py --no-domain
```
