# Agent Guide

This document contains guidelines for AI agents working on this project.

## General Principles

1. **Safety First**: Never execute destructive commands without confirming they are safe.
2. **Read the Code**: Always explore the codebase to understand the context before making changes.
3. **Verify Everything**: After creating or modifying files, run read commands to ensure the changes were successful.
4. **Test-Driven Development**: When possible, write failing tests first, then write the code to make them pass.
5. **No Blind Environment Changes**: Diagnose build or test failures by examining logs and configuration files before attempting to reinstall dependencies.
6. **Documentation**: Keep all documentation, including these `docs/` files, up-to-date with code changes.

## Android Specifics

*   Follow standard Android architecture (e.g., MVVM, Clean Architecture).
*   Use Kotlin as the primary language, following idiomatic Kotlin conventions.
*   Manage dependencies via Gradle (version catalogs preferred).
*   Ensure UI components are accessible.
