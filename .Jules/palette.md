## 2024-05-15 - Explicit Context in Data Grid Checkboxes
**Learning:** Checkboxes within a data grid without explicit context in their aria-label can be confusing for screen reader users as they lack spatial context.
**Action:** When using checkboxes within a data grid, always provide explicit row and column context in the aria-label (e.g., `aria-label="Toggle [Row] on [Column]"`) so screen readers can announce the context.

## 2026-06-08 - Explicit Context for Icon-Only Action Buttons in Lists
**Learning:** Icon-only action buttons (like Delete) in nested lists or trees without the item's context in the aria-label are ambiguous to screen reader users.
**Action:** When adding icon-only action buttons to items in lists, always include the specific item's title in the `aria-label` (e.g., `aria-label="Delete task: [Task Title]"`) to provide explicit context.

## 2024-08-01 - Explicit Semantic Focus States for Form and Comment Toggles
**Learning:** Disclosure toggles (like "Add Task" or comment toggles) and toggle switches often lack clear focus states and semantic linkage to the sections they control.
**Action:** Always add `aria-expanded` / `aria-controls` for disclosure elements linked to IDs of the target containers, use `role="switch"` with `aria-checked` for binary task statuses, and explicitly apply `focus-visible:ring-2 focus-visible:outline-none` for all custom interactive controls so keyboard users have clear visual focus feedback.
