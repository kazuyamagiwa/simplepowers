### Dataframe & Transformation Observability
When working with dataframes (e.g., Pandas) or large data collections, you MUST structure the code to allow for step-by-step visual inspection. 

- **Break the Chain:** Absolutely NO long method chains (e.g., `df.query().groupby().agg()`). Break transformations into discrete steps and assign intermediate results to well-named variables.
- **Scaffold Data Hooks:** After every major transformation (merge, filter, complex aggregation), inject a commented-out inspection line so I can instantly check the state: `# debug: print(f"Shape: {df_filtered.shape}"); print(df_filtered.head(3))`
- **Ban `inplace=True`:** Never mutate dataframes in place. Always use explicit assignment so the original state is preserved for debugging.
- **Named Functions over Complex Lambdas:** Extract complex `lambda` logic into standard, readable Python functions and use `.apply(my_named_func)`.
