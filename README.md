# VYRO

VYRO is an Android-first, offline-first creative production ecosystem.

## Current phase

Foundation milestone: project structure, Arabic/English localization, Compose shell, architectural boundaries, tests, and GitHub Actions validation.

## Product rules

- The authoritative scope is documented in `docs/VYRO_MASTER_SPEC.md`.
- No feature is represented as implemented until it is tested and verified.
- The first release contains no AI features.
- Arabic and English are authored independently.
- Local projects remain usable offline.

## Modules

- `app`: Android application shell and navigation.
- Future domain and engine modules will be added behind versioned contracts.

## Build

Requirements: JDK 17 and Android SDK.

```bash
./gradlew :app:assembleDebug
./gradlew test lint
```
