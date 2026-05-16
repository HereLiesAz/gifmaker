# Testing Standards

This document outlines the testing strategy for the application.

## Test Types

1.  **Unit Tests (Local)**
    *   Location: `src/test/java`
    *   Scope: ViewModels, Repositories, Use Cases, Utility classes.
    *   Tools: JUnit 4/5, MockK, Coroutines Test library.
    *   Goal: Test business logic in isolation.

2.  **Instrumented Tests (Device/Emulator)**
    *   Location: `src/androidTest/java`
    *   Scope: Database (Room DAOs), specific platform-dependent logic.
    *   Tools: AndroidX Test, JUnit.

3.  **UI Tests**
    *   Location: `src/androidTest/java`
    *   Scope: Screen rendering, user interactions, navigation flows.
    *   Tools: Compose Testing API, Espresso.

## Guidelines
*   Aim for high code coverage, but prioritize testing complex business logic over simple getters/setters.
*   Tests should be deterministic (not flaky).
*   Mock external dependencies (network, database) in unit tests.
*   Follow the Arrange-Act-Assert pattern in test functions.
