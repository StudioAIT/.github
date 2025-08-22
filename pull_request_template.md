<!-- 
🚀 PR Template for Linear + GitHub Integration

BRANCH NAMING + PR INTEGRATION:
Your branch should be named: feature/inv-123-description
This allows Linear to auto-link the PR to issue INV-123

INSTRUCTIONS:
1. Ensure your branch name contains the Linear issue ID (e.g., feature/inv-123-description)
2. Replace INV-XXX below with the SAME Linear issue ID from your branch name
3. Use "Closes INV-XXX" to auto-close the issue when this PR merges
4. Use "Related to INV-XXX" if this PR only partially addresses the issue
5. Fill out all sections below - delete any that don't apply
6. Add screenshots/videos for UI changes
7. Double-check: branch name and PR template reference the same Linear issue!

BRANCH NAMING EXAMPLES:
✅ feature/inv-123-allow-negative-penalties
✅ bugfix/inv-456-protest-flag-scaling  
✅ tech/inv-789-refactor-scoring-engine
❌ fix-penalties (no Linear ID - won't auto-link)
❌ update-docs (no Linear ID - won't auto-link)

WHY BOTH BRANCH NAME + PR TEMPLATE?
- Branch naming: Auto-detection by Linear (primary method)
- PR template: Manual specification (safety net)
- Together: Bulletproof linking that ensures every PR connects to its Linear issue
-->

## Linear Issue
Closes INV-XXX

<!-- 
LINKING OPTIONS:
- "Closes INV-XXX" → Auto-closes issue when PR merges
- "Fixes INV-XXX" → Same as Closes
- "Resolves INV-XXX" → Same as Closes  
- "Related to INV-XXX" → Links but doesn't auto-close
- Manual link: https://linear.app/yourteam/issue/INV-XXX

IMPORTANT: The INV-XXX here should match the Linear ID in your branch name!
-->

## Summary
<!-- Brief description of what this PR accomplishes -->

## Changes Made
<!-- Detailed list of changes - be specific -->
- [ ] 
- [ ] 
- [ ] 

## Testing
<!-- How did you test these changes? -->
- [ ] Manual testing steps completed
- [ ] Automated tests added/updated
- [ ] Edge cases considered
- [ ] Cross-browser testing (if applicable)

## Screenshots/Videos
<!-- For UI changes, add before/after images or demo videos -->

## Breaking Changes
<!-- List any breaking changes and migration steps -->
- [ ] No breaking changes
- [ ] Breaking changes (list below):

## Checklist
- [ ] Code follows project conventions
- [ ] Tests added/updated and passing
- [ ] Documentation updated (if needed)
- [ ] Linear issue linked correctly
- [ ] Ready for review

## Additional Notes
<!-- Any extra context, concerns, or future considerations -->

---

<!-- 
EXAMPLES:

Example 1 - Feature Implementation:
```
## Linear Issue  
Closes INV-123

## Summary
Implements negative penalty feature flag system allowing race officials to assign negative penalties as "wildcards" for race manipulation.

## Changes Made
- Added `VITE_ALLOW_NEGATIVE_PENALTIES` environment variable support
- Updated penalty validation logic in `src/components/admin/live-race-table/table-rows.jsx`
- Modified UI constraints in race editor components
- Added feature flag configuration to `src/constants/index.js`
- Updated validation messages to be dynamic based on feature state

## Testing
- Tested with flag enabled/disabled in development
- Verified negative penalties work correctly in race calculations
- Confirmed backward compatibility when flag is disabled
- Added validation for edge cases (NaN, extreme negative values)

## Screenshots/Videos
[Screenshot of penalty input accepting -5 points]
[Screenshot of dynamic validation message]
```

Example 2 - Bug Fix:
```
## Linear Issue
Fixes INV-456

## Summary
Resolves critical issue where protest flags weren't scaling properly in OBS detailed views at different resolutions.
a
## Changes Made
- Fixed CSS class application in `leaderboard-overview-row.jsx` 
- Corrected template literal syntax error (unclosed quote)
- Added proper OBS scaling classes for protest flag display
- Updated obs-scaling.css to include protest flag scaling rules

## Testing
- Verified scaling works correctly at 1080p, 1440p, and 4K resolutions
- Tested in OBS Studio with browser source
- Confirmed flags display consistently across all OBS detailed routes
- No regression in non-OBS views

## Screenshots/Videos
[Before: Small protest flags in 4K OBS overlay]
[After: Properly scaled protest flags in 4K OBS overlay]

## Breaking Changes
- [x] No breaking changes
```
-->