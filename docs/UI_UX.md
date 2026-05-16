# UI/UX Guidelines

This document outlines the user interface and user experience standards for the application.

## Design System

*   **Color Palette**: Use semantic colors defined in the theme (Primary, Secondary, Background, Surface, Error).
*   **Typography**: Stick to the defined type scale for consistency across headings, body text, and labels.
*   **Spacing**: Use an 8dp grid system for all padding and margins. (e.g., 8dp, 16dp, 24dp, 32dp).

## Accessibility

*   All interactive elements must have a minimum touch target size of 48x48dp.
*   Provide `contentDescription` for all meaningful images and icons.
*   Ensure sufficient color contrast between text and background.

## Interactions

*   Provide immediate visual feedback for user actions (e.g., ripple effects, loading indicators).
*   Use standard Android navigation paradigms.
*   Handle empty states and error states gracefully with clear messaging.

## Tooling

*   Use Jetpack Compose for all new UI development.
*   Follow Material Design 3 guidelines unless custom branding dictates otherwise.
