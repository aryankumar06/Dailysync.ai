## 2024-05-15 - Explicit Context in Data Grid Checkboxes
**Learning:** Checkboxes within a data grid without explicit context in their aria-label can be confusing for screen reader users as they lack spatial context.
**Action:** When using checkboxes within a data grid, always provide explicit row and column context in the aria-label (e.g., `aria-label="Toggle [Row] on [Column]"`) so screen readers can announce the context.

## 2026-06-08 - Explicit Context for Icon-Only Action Buttons in Lists
**Learning:** Icon-only action buttons (like Delete) in nested lists or trees without the item's context in the aria-label are ambiguous to screen reader users.
**Action:** When adding icon-only action buttons to items in lists, always include the specific item's title in the `aria-label` (e.g., `aria-label="Delete task: [Task Title]"`) to provide explicit context.
## 2026-09-15 - Accessible Disclosure and Group Forms
**Learning:** Relying on simple toggles and grouped buttons without semantic markup (like `aria-expanded`, `aria-controls`, and `role="group"`) creates a disconnected experience for screen reader users when interacting with expanding forms.
**Action:** When building collapsible sections or grouped toggle buttons, always use `aria-expanded` with `aria-controls` for triggers, and `role="group"` with `aria-labelledby` and `aria-pressed` for custom mutually exclusive selectors.
