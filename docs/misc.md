# Miscellaneous Guidelines

This document contains guidelines that do not fit neatly into other categories.

## Dependency Management
*   Keep dependencies up to date, but test thoroughly after updates.
*   Avoid adding large libraries for simple functions that can be easily implemented internally.
*   Document the reason for adding any major new dependency.

## Logging
*   Use Android's built-in `Log` class or a library like Timber.
*   Do not leave excessive debug logging in production builds.
*   Never log sensitive user information (PII).

## ProGuard / R8
*   Ensure ProGuard/R8 rules are updated when adding new libraries that use reflection.
*   Test release builds thoroughly to catch minification issues.
