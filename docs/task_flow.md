# Task Flow and Implementation Guidelines

This document outlines the step-by-step process for implementing a new feature.

## 1. Planning and Understanding
*   Read the feature requirements carefully.
*   Identify the necessary UI changes, data models, and API endpoints.
*   Consult the `/docs/` to ensure the planned approach aligns with architectural guidelines.

## 2. Data Layer Implementation
*   Create or update network DTOs and API interfaces (Retrofit).
*   Create or update local Entities and DAOs (Room).
*   Update the Repository to handle data fetching and caching logic.
*   Write unit tests for the Repository logic.

## 3. Domain/Presentation Layer
*   Create or update ViewModels.
*   Expose state to the UI using StateFlow or LiveData.
*   Implement business logic within the ViewModel (or Use Cases if utilizing Clean Architecture).
*   Write unit tests for ViewModels.

## 4. UI Implementation
*   Build the UI using Jetpack Compose.
*   Observe the state from the ViewModel.
*   Ensure UI aligns with `UI_UX.md` guidelines.
*   Write UI tests (Compose tests or Espresso).

## 5. Review and Verification
*   Run all tests.
*   Verify no regressions were introduced.
*   Request a code review.
