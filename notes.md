# Notes

## Summary of changes

Fixed a backend SQL filtering issue in `TaskRepository.java`. The title/description search conditions were not grouped correctly, which caused the selected status filter to be applied incorrectly. I grouped the search conditions so the status filter is now applied consistently to the search results.

## What I chose not to change

I did not make broader UI, API, or structural changes because the assignment asked for a focused patch. I also avoided changing unrelated behavior that was working correctly.

## Biggest remaining risk

The main remaining risk is that there may be other edge cases in the filtering, pagination, or frontend/backend interaction that were not covered within the timebox. More comprehensive automated tests would reduce this risk.

## Tools/AI used

I used VS Code for development and testing, Git/GitHub for version control, and ChatGPT to help understand the code and reason about the SQL operator-precedence issue. I verified the behavior and made the final code changes myself.