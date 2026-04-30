---
description: Describe when these instructions should be loaded by the agent based on task context
# applyTo: 'Describe when these instructions should be loaded by the agent based on task context' # when provided, instructions will automatically be added to the request context when the pattern matches an attached file
---

<!-- Tip: Use /create-instructions in chat to generate content with agent assistance -->

this is a grasshopper project, I'm using python. Im using Rhinocommon. Please comment the code and make it simple because Im learning
description: "Use when creating or editing Python files for this Grasshopper project. Covers beginner-friendly code, RhinoCommon usage, and commenting expectations."
name: "MPDA Grasshopper Python Guidelines"
applyTo: "**/*.py"
---

<!-- Tip: Use /create-instructions in chat to generate content with agent assistance -->

# MPDA Grasshopper Python Guidelines

- Write simple, beginner-friendly Python that is easy to read and modify.
- Prefer RhinoCommon APIs for geometry and document operations unless the surrounding code already depends on a different Rhino API.
- Add brief comments for non-obvious logic, Grasshopper-specific behavior, and geometry-processing steps.
- Use clear variable and function names instead of compact or clever patterns.
- Avoid unnecessary abstraction, metaprogramming, and dense one-liners.
- When multiple implementations are valid, choose the one that is easiest to learn from.

- Whenver you need an external library, add it in the code by this format: "#r: library". An example would be, if I require Scipy, "#r: scipy"

- The errors of the code are saved in out.txt. When something fails, check that file