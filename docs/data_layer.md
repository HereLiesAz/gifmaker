# Data Layer Specifications

This document defines how data is managed, stored, and retrieved in the application.

## Architecture

The data layer is responsible for providing data to the rest of the application, abstracting the source of the data (network vs. local database).

### Repositories
*   Repositories act as the single source of truth for data.
*   They mediate between different data sources (e.g., fetching from an API, caching in a local database).
*   ViewModels should interact *only* with repositories or use cases, never directly with data sources.

### Network Source
*   Use Retrofit for API communication.
*   Use Kotlin Coroutines and Flow for asynchronous operations.
*   Define clear DTOs (Data Transfer Objects) for network responses and map them to domain models in the repository.

### Local Source
*   Use Room for local database persistence.
*   Define Entities for database tables.
*   Use DAOs (Data Access Objects) for database operations.

## Caching Strategy
*   Implement a "Single Source of Truth" strategy where applicable: Fetch from network -> Save to database -> Read from database to update UI.
