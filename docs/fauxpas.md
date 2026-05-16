# Faux Pas & Anti-Patterns

This document lists common mistakes and anti-patterns that must be avoided in this project.

## General
1.  **Skipping Tests**: Never commit code without associated tests (unit or UI) where applicable.
2.  **Ignoring Errors**: Do not use empty catch blocks (`catch (e: Exception) {}`). Always log or handle exceptions appropriately.
3.  **Hardcoding Strings**: Do not hardcode user-facing strings in code. Use `strings.xml`.
4.  **Hardcoding Dimensions/Colors**: Do not hardcode dimensions or colors. Use `dimens.xml` and the defined theme/color palettes.

## Architecture
1.  **God Activities/Fragments**: Do not put business logic or data fetching in UI classes.
2.  **Context Leaks**: Be extremely careful when passing `Context`. Avoid passing Activity contexts to singletons or long-lived background tasks. Use Application context if necessary.
3.  **Direct Database Access from UI**: Never query the database directly from an Activity, Fragment, or Compose function.

## Asynchronous Operations
1.  **Main Thread Blocking**: Never perform heavy computations or blocking I/O operations on the main thread.
2.  **Unstructured Concurrency**: Avoid launching coroutines in the `GlobalScope`. Always use lifecycle-aware scopes (e.g., `viewModelScope`, `lifecycleScope`).
