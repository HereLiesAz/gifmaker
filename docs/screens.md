# Screen Definitions

This document outlines the primary screens of the application and their relationships.

## Authentication Flow
*   **Splash Screen**: Initial loading screen, checks authentication state. Routes to Login or Home.
*   **Login Screen**: Allows user to authenticate. Routes to Registration or Home.
*   **Registration Screen**: Allows new user creation. Routes to Home upon success.

## Main Application
*   **Home Screen (Dashboard)**: The primary landing view. Displays key metrics or a feed.
*   **Profile Screen**: Displays user details and settings. Allows editing of user info.
*   **Settings Screen**: Application preferences (theme, notifications, etc.).
*   **Details Screen**: A generic screen structure for displaying detailed information about a specific item selected from the Home Screen.

## Navigation
*   Use Jetpack Navigation Component.
*   Define a clear navigation graph (e.g., `NavHost`).
*   Pass minimal data (like IDs) between screens; let the destination screen fetch the full data.
