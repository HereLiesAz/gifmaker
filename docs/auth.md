# Authentication Specifications

This document describes the authentication flow and security requirements.

## Authentication Methods

*   **Primary**: Email and Password.
*   **Secondary (OAuth)**: Google Sign-In, Apple Sign-In.

## Token Management

*   Use short-lived JWT access tokens and long-lived refresh tokens.
*   Store tokens securely using Android's `EncryptedSharedPreferences` or the Android Keystore system.
*   Never log sensitive authentication data (passwords, raw tokens).

## Flows

1.  **Login**: Request credentials -> Receive tokens -> Store securely -> Navigate to Home.
2.  **Registration**: Request details -> Validate -> Create account -> Receive tokens -> Store securely -> Navigate to Home.
3.  **Token Refresh**: Detect expired access token -> Use refresh token to request new access token -> Retry original request.
4.  **Logout**: Clear locally stored tokens -> Navigate to Login screen -> Notify server to invalidate tokens (if applicable).

## Security Best Practices

*   All network traffic must be over HTTPS.
*   Implement certificate pinning if highly sensitive data is handled.
*   Validate all inputs on both the client and server sides.
