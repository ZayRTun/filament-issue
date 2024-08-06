**Title**: UI Bug: `Select` Filter with Multiple Options Hidden by `overflow: hidden` CSS in `FiltersLayout::BelowContent`

**Description**:
When using the `Select` filter component with multiple options enabled in Filament, and setting the filter layout to `FiltersLayout::BelowContent`, the dropdown containing the options is hidden by CSS `overflow: hidden` when placed near the bottom of the viewport. This issue makes it impossible to interact with the dropdown.

**Steps to Reproduce**:

1. Set up a Filament table with filters.
2. Use a `Select` filter with multiple options enabled.
3. Set the filter layout to `FiltersLayout::BelowContent`.
4. Place the filter near the bottom of the viewport.
5. Attempt to open the dropdown.

**Expected Behavior**:
The dropdown should either open above the input field if there's no space below or adjust its position to ensure it’s visible.

**Actual Behavior**:
The dropdown is hidden by the CSS `overflow: hidden`, making it impossible to interact with.

**Screenshots**:
_Include screenshots or a screen recording here to visually demonstrate the issue._

**Environment**:

-   Filament Version: [Your Filament version]
-   Laravel Version: [Your Laravel version]
