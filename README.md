# 🧪 TDD Workflow

[![ClawHub Skill](https://img.shields.io/badge/ClawHub-Skill-blue)](https://clawhub.ai/djc00p/tdd-workflow) [![Agent Skill](https://img.shields.io/badge/Agent-Skill-blue)](#) [![TDD](https://img.shields.io/badge/TDD-00758F.svg)](https://en.wikipedia.org/wiki/Test-driven_development) [![Coverage](https://img.shields.io/badge/Coverage-80%25-success.svg)](https://en.wikipedia.org/wiki/Code_coverage) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**TDD Workflow** ensures all code development follows test-driven principles with **80%+ coverage**.

The discipline isn't "write tests eventually." It's the **RED-GREEN-REFACTOR** cycle — and the most important part is RED. A test that has never failed proves nothing: it might be asserting the wrong thing, or asserting nothing at all. Seeing it fail first is what gives it meaning.

---

## 🎯 When to Activate

* Writing new features or functionality
* Fixing bugs or issues
* Refactoring existing code
* *"Write tests"*, *"add specs"*, *"how should I test this"*

---

## 🚀 Quick Start

1. **Write the user journey** in acceptance-test format — *"As a [role], I want..."*
2. **Generate test cases** — happy path + edge cases + errors
3. **Run tests → verify RED** — it must fail before implementation
4. **Implement minimal code** to make them pass → **GREEN**
5. **Refactor** while keeping tests green
6. **Verify 80%+ coverage** achieved

---

## 🔴🟢🔵 RED-GREEN-REFACTOR

```text
🔴 RED       Write a failing test. Watch it fail for the RIGHT reason.
🟢 GREEN     Write the minimum code that passes. Nothing more.
🔵 REFACTOR  Clean up the implementation. Tests stay green throughout.
```

**No exceptions.** Writing implementation first and adding tests afterward is not TDD — it's test-after, and the tests are weaker for it.

---

## 🧠 Key Concepts

* **Tests before code** — write the test first, then the implementation
* **RED-GREEN-REFACTOR** — fail → pass → improve
* **80% coverage minimum** — unit, integration, and E2E combined
* **Unit-level isolation** — mock dependencies; test behavior, not implementation
* **Independent tests** — no ordering dependencies; each can run solo

---

## 📂 Test Types

| Type | Scope | Speed |
|------|-------|-------|
| **Unit** | Functions and components in isolation | < 50ms each |
| **Integration** | API endpoints, database operations | Seconds |
| **E2E** | Critical user flows | Minutes |

Fast unit tests run constantly. Slow E2E tests run before release. Don't put E2E assertions where a unit test would do.

---

## ✅ What Good Tests Look Like

* **Test behavior, not implementation** — asserting on internal calls makes refactoring painful and tests brittle
* **Mock dependencies, not the unit under test** — mocking what you're testing means testing nothing
* **Independent** — any test can run alone, in any order
* **Explicit edge cases** — empty arrays, nulls, boundary values, error paths

---

## 📚 References

* `references/test-patterns.md` — unit, integration, and E2E patterns with examples
* `references/tdd-workflow.md` — the detailed RED-GREEN-REFACTOR cycle and coverage tooling

---

**Published by [@djc00p](https://github.com/djc00p)**
