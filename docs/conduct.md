# Code of Conduct & Coding Standards

This document outlines the expected behavior and coding conventions for all contributors (human and AI).

## Coding Standards

### Kotlin Formatting
*   Follow standard ktlint rules.
*   Use 4 spaces for indentation.
*   Keep functions small and focused on a single responsibility.
*   Use meaningful and descriptive variable/function names (camelCase for variables/functions, PascalCase for classes).

### Architecture
*   Adhere strictly to the chosen architecture pattern (e.g., MVVM).
*   Do not bypass architectural layers (e.g., UI should not communicate directly with the database).

### Comments
*   Write clear, concise docstrings for all public classes and functions.
*   Explain *why* something is done if it's not immediately obvious from the code. Avoid commenting on *what* the code does if it's self-explanatory.

## Review Process
*   All code MUST undergo a review process.
*   AI agents must request a review (`request_plan_review`, `request_code_review`) before submitting changes.
*   No direct commits to `main` without review.
