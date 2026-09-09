### Architectural Simplicity Constraint (Intermediate Level)
When drafting an implementation plan and file structure, you MUST optimize for architectural simplicity. The resulting codebase must be easily navigable by an intermediate programmer. 

- **Flat File Structure:** Do not create deeply nested directories. Group related concrete logic together in a single file where appropriate.
- **Ban Enterprise Patterns:** Do NOT plan tasks that implement Repositories, Service Locators, Abstract Factories, complex Dependency Injection, or multi-layered inheritance. Stick to simple functions, standard data structures, or basic classes.
- **No "Future-Proofing":** Plan ONLY the files strictly required for the immediate feature (Strict YAGNI). Do not build generic wrappers in anticipation of future scale.
- **Concrete Tasks:** Every task must result in a working piece of the feature, not abstract boilerplate or scaffolding.
