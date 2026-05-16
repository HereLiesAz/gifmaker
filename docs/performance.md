# Performance Guidelines

This document outlines strategies for maintaining a high-performance application.

## UI Performance
*   Avoid deep view hierarchies (less of an issue with Compose, but still relevant).
*   Optimize Compose recompositions by using `remember` and avoiding unstable parameters.
*   Use `LazyColumn`/`LazyRow` for lists to recycle views efficiently.
*   Profile UI rendering to ensure 60fps (or higher) is maintained.

## Memory Management
*   Avoid memory leaks by managing lifecycles carefully (especially regarding Context and Observers).
*   Use tools like LeakCanary during development to identify leaks early.
*   Be mindful of image loading; use libraries like Coil or Glide which handle memory caching automatically.

## Network & Battery
*   Batch network requests where possible.
*   Use WorkManager for deferrable background tasks to optimize battery usage.
*   Cache data aggressively to reduce unnecessary network calls.
