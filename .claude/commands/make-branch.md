# make-branch

Generate consistent branch names from GitHub issue information.

## Usage

```
/make-branch <issue-index> "<issue-title>"
```

## Template

```
i{issue-index}-{type}/{action-description_with_underscores}
```

## Supported Types

- `feat` - New features
- `fix` - Bug fixes  
- `docs` - Documentation changes
- `config` - Configuration updates
- `refactor` - Code refactoring

## Examples

- Input: `/make-branch 15 "feat: implement Button component"`
- Output: `i15-feat/implement_button_component`

- Input: `/make-branch 23 "fix: resolve styling issues in Dialog"`
- Output: `i23-fix/resolve_styling_issues_in_dialog`

- Input: `/make-branch 8 "config: setup ESLint configuration"`
- Output: `i8-config/setup_eslint_configuration`

- Input: `/make-branch 42 "docs: add component usage examples"`
- Output: `i42-docs/add_component_usage_examples`

## Implementation

Parse the issue title to:
1. Extract the type prefix (feat:, docs:, etc.)
2. Extract the action description after the colon
3. Convert spaces to underscores
4. Preserve existing hyphens
5. Remove other special characters
6. Format as the template above

## Workflow

1. Generate branch name using the command
2. Review the generated name
3. Create and checkout the branch if approved:
   ```bash
   git checkout -b <generated-branch-name>
   ```