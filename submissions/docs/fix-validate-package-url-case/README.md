# Fix: Case-Sensitivity in validate-package.mjs

Normalizes the repository URL check in `validate-package.mjs` to lowercase before comparison.

## What does this do?
- **Prevents Casing Rejections:** Standardizes package check validation rules so that casing variations in the package.json repository URL do not cause CI rejections.