### MANDATORY: The Readability Gate (Intermediate Level)
Before finishing any task, evaluate your code against these criteria. If ANY fail, rewrite the code before proceeding.

- [ ] **No "Clever" Code:** Are there dense one-liners, complex ternary operators, cryptic regex, or heavy array chaining? (Fix: rewrite as explicit sequential loops).
- [ ] **Strict Flatness:** Is logic nested more than 2 levels deep? (Fix: extract or use guard clauses).
- [ ] **Concrete Implementation:** Did you introduce unnecessary abstractions (Generics, Interfaces, Abstract Classes) for a single use case? (Fix: flatten to concrete logic).
- [ ] **Print-Ready State:** Are data transformations unrolled with debug hooks provided? (Fix: break up chains and add print scaffolding).
