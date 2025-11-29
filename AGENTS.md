# Work Like It Has To Last

> “Measure twice, cut once.”  
> The people who built the world before the digital age didn’t ship “good enough.”  
> They built things expecting them to be used hard, repaired often, and still standing decades later.

This file is a guide for any AI agent or developer working in this codebase.  
Treat this project like a workshop, not a factory. You’re here to do real craft.

---

## 1. How To Show Up

Before you change anything:

- **Read the grain of the wood**  
  Study the existing code, patterns, and conventions. Don’t fight the structure that’s already working.

- **Assume someone depends on this**  
  Code as if it will run in critical paths, even if it’s “just a small utility.”

- **Respect the tools**  
  Use the project’s existing stack, scripts, and patterns. Don’t introduce shiny new things without a clear reason and a full integration.

---

## 2. Core Philosophy

These are the habits that old-world builders would recognize:

- **Do it right, not fast**  
  If you have to choose, pick the solution that is clear, durable, and testable, even if it takes a bit longer.

- **Work with the material, not against it**  
  Code should work with the language and framework idioms, not fight them. Avoid forcing patterns that don’t fit.

- **Leave clean edges**  
  No half-implemented features, no placeholder data “for now,” no TODOs for essentials. If it matters, either build it or remove it.

- **Make it understandable at a glance**  
  Future readers should be able to see what’s load-bearing and what’s decorative. Clear structure, clear names, clear flow.

- **Honor the invisible work**  
  Tests, docs, edge cases, performance, and accessibility are not optional. They’re the unseen foundations that keep the whole thing standing.

---

## 3. How To Change Things

When you write or modify code:

- **Extend the existing structure**  
  Add new pieces in the same style, folder layout, and naming patterns. Avoid “one special file” that behaves differently.

- **Keep responsibilities sharp**  
  Functions and modules should do one thing well. If something is trying to be a whole toolbox, split it.

- **Refactor like a careful renovation**  
  When improving old code, don’t smash walls just to rearrange furniture. Change only what you must, prove it with tests, and keep behavior stable unless you intentionally evolve it.

- **Prefer clarity over cleverness**  
  A junior developer or another agent should be able to follow your code without guessing at your intentions.

---

## 4. Tests: The Structural Load Check

Builders check that a beam can hold weight before people walk under it. You do the same with tests:

- Every meaningful change should have tests that would fail if your change broke.
- Keep tests close to the code they protect.
- Write tests that describe real usage, not just happy-path demos.
- If a bug appears, add a test that would have caught it, then fix the code.

If it isn’t testable, it’s probably not well-shaped.

---

## 5. Documentation: The Shop Notes

The old way: a notebook on the workbench. The modern way: docs in the repo.

- Document **how** and **why**, not just “it exists.”
- Update existing docs when you change behavior; don’t leave them lying.
- Keep instructions simple enough that a new teammate could follow them without asking questions.

If someone can’t understand how to use or extend what you wrote, the job isn’t finished.

---

## 6. Respect for Constraints

Old builders worked with whatever they had: limited tools, limited materials, harsh environments. Treat project constraints the same way:

- Honor the chosen stack and architecture.
- Work within performance, security, and privacy boundaries.
- Prefer small, stable improvements over flashy, fragile inventions.

Constraints are not annoyances. They are the shape of the problem.

---

## 7. Behavior Expectations for Agents

When acting in this repository:

**Do not:**

- Introduce breaking changes casually.
- Weaken tests, lint rules, or quality checks to “make it pass.”
- Add placeholder logic where real logic is required.
- Invent new patterns if existing ones are good enough.

**Do:**

- Match the project’s voice, structure, and patterns.
- Improve readability while you’re there.
- Tighten tests and error handling where it’s obviously needed.
- Leave the codebase a little better than you found it.

---

## 8. The Standard of Work

Use this as your personal checklist before calling anything “done”:

- [ ] The change fits naturally into the existing structure and style.  
- [ ] The behavior is clear and predictable from reading the code.  
- [ ] Tests exist, pass, and would catch obvious regressions.  
- [ ] No essential part of the system relies on placeholder or fake data.  
- [ ] Documentation and comments are updated and accurate.  
- [ ] The change makes the system simpler to understand, not more tangled.  
- [ ] You’d be comfortable signing your name to this work in ten years.

---

## 9. Why This Matters

The people who poured concrete, shaped steel, and set brick weren’t chasing “engagement metrics.”  
They tried to leave behind something solid, something that wouldn’t embarrass them when time had its say.

Treat this codebase the same way.

Work as if someone you respect will read every line.  
Build as if it has to stand for a long time.  
Let the quality of the work speak for itself.
