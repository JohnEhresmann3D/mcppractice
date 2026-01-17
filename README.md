# AI Personality & Role Management System

## Overview

This repository defines a **structured, multi-role personality framework** for guiding AI agents in complex creative and technical projects—especially game development, simulation design, and production workflows.

Rather than treating the AI as a single, amorphous assistant, this system enforces **clear roles, authority boundaries, and execution gates**, allowing the AI to behave more like a disciplined cross-functional team.

This approach is designed to:
- Reduce role bleed
- Prevent premature execution
- Improve output consistency over long sessions
- Enable intentional role switching
- Support documentation-first workflows

---

## Core Concepts

### 1. Role-Based Cognition

Each role is defined in its own `.md` file and represents a **distinct mindset**, not just a job title.

Roles include:
- A unique identity
- Responsibilities
- Decision heuristics
- Failure modes
- Authority boundaries
- Preferred output formats
- Explicit success criteria

An AI agent should **only act within the bounds of the currently active role(s)**.

---

### 2. Gated Execution

All behavior is governed by a central context initializer that enforces:

- Role selection before action
- Phase awareness (Discovery → Planning → Design → Implementation → Review)
- Authority enforcement
- Output discipline
- Reality checks before finalization

If required information is missing, the AI must **stop and ask**, not guess.

---

### 3. Documentation as Control Surface

These markdown files are not passive descriptions—they are **behavioral constraints**.

They are intended to be:
- Read at initialization
- Referred to during execution
- Used to self-correct drift
- Treated as authoritative over ad-hoc instruction

---

## Repository Structure

```text
/ai_personalities
│
├─ PRODUCER.md                  # Planning, sequencing, delivery discipline
├─ GAME_DESIGNER_ECONOMICS.md   # Tycoon-style systems, economies, simulations
├─ SOFTWARE_ENGINEER_GAMEPLAY.md# Gameplay systems + UX-first engineering
├─ UI_ENGINEER.md               # Information design & interface clarity
├─ ART_DIRECTOR_CARTOONS.md     # Cartoon foundations & visual direction
│
└─ CONTEXT.md                   # Initialization logic and behavioral gates
