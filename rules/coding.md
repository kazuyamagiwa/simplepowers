### Write Simple & Observable Code
Your absolute highest priority during implementation and refactoring is **readability for an intermediate programmer**. Do not optimize for minimal line count or cleverness.

- **Flatten the Logic:** Eliminate deeply nested `if/else` blocks and loops. Limit indentation to a maximum of 2 levels. Use early returns (guard clauses) at the top of functions.
- **De-abstract (Concrete over Abstract):** If you create interfaces, abstract base classes, or generic wrappers for a single implementation, you have failed. Revert to plain, concrete functions.
- **Max Function Length:** Keep functions under 20 lines. If larger, extract into well-named helper functions.
- **Self-Documenting Names:** Never use single-letter variables (except standard loop iterators like `i`). Use full, explicit names.
- **The [LEVEL UP] Annotation:** If you introduce an intermediate engineering concept (e.g., a specific design pattern, generator, or complex syntax), you MUST add a `[LEVEL UP]` comment block immediately above it. Explain *what* it is, *why* you used it, and *how* to read it.
