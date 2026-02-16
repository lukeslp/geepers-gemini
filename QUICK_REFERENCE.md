# Geepers Task Mapping

| Task | Primary Skill | Secondary |
|------|---|---|
| "What should I work on?" | **geepers-planner** | geepers-scout |
| "Build this feature" | **geepers-builder** | geepers-planner |
| "Surgical code edit" | **geepers-scalpel** | — |
| "Code review" | **geepers-critic** | — |
| "Deep research" | **geepers-scout** | — |
| "Debug an error" | **geepers-diag** | geepers-scalpel |
| "Security audit" | **geepers-security** | — |
| "Write tests" | **geepers-test** | geepers-critic |

## Orchestration Flow
1. **Plan**: `geepers-planner` → `geepers-scout`
2. **Execute**: `geepers-builder` OR `geepers-scalpel`
3. **Verify**: `geepers-critic` → `geepers-test`
4. **Finalize**: `geepers-team`
