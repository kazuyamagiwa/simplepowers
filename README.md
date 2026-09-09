# Mortalpowers

Mortalpowers is a readability-first sandbox for AI coding assistants.

It is a constraint-based wrapper that forces AI tools to write intermediate-level, flat, readable, and highly observable code—code that human intermediate developers can easily read, debug, and learn from.

## How it works

Cursor (and similar AI assistants) load `.cursorrules`, which points at the constraints in `/rules`:

| Rule file | When it applies |
| --- | --- |
| `rules/planning.md` | Planning features and file structure |
| `rules/coding.md` | Writing and refactoring general code |
| `rules/data-processing.md` | Dataframe / array transformations |
| `rules/review-gate.md` | Self-audit before finishing a task |

## Design goals

- Prefer flat file layouts and concrete functions over enterprise patterns
- Keep logic shallow, named, and under short function lengths
- Make data pipelines step-by-step inspectable with debug print scaffolding
- Gate every change through a mandatory readability checklist
