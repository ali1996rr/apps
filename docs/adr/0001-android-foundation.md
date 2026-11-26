# ADR 0001: Android foundation

- Status: Accepted
- Date: 2026-11-26

## Decision

Use Kotlin, Jetpack Compose, Gradle Kotlin DSL, minSdk 26, target/compile SDK 35, and JDK 17 for the initial Android foundation.

## Rationale

This provides a maintainable Android-first baseline with modern UI, explicit RTL support, and a path to modular native media engines. Capabilities remain runtime-detected; no Samsung-specific behavior is hardcoded.

## Consequences

Native media, GPU, and DSP engines will be isolated in later modules. Each must expose a versioned capability report and CPU-safe fallback where required by the master specification.
