# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a learning repository for Android development with Kotlin. It contains two main sections:

1. **basic/** - Kotlin language fundamentals and exercises
2. **app/** - Jetpack Compose Android application for practical development

## Project Structure

### basic/
Contains standalone Kotlin files for learning language fundamentals. These are simple `.kt` files that can be compiled and run independently.

**Running Kotlin files:**
```bash
# Compile and run a Kotlin file
kotlinc basic/*.kt -include-runtime -d output.jar && java -jar output.jar
```

### app/
A Jetpack Compose Android application using Material 3 design.

**Package structure:**
- `com.example.jetpackcomposelearning` - Main package
- `com.example.jetpackcomposelearning.ui.theme` - Theme, colors, and typography

**Key configuration:**
- compileSdk: 34
- minSdk: 24
- targetSdk: 34
- Compose BOM: 2024.02.00
- Kotlin JVM target: 1.8

## Android Development

This project requires Android Studio to build and run the `app/` module. There is currently no root-level `settings.gradle.kts` or `build.gradle.kts`, so the Android app module is not yet connected to a Gradle project structure.

**To work with the Android app:**
1. Open the project in Android Studio
2. Ensure a proper Gradle wrapper and settings file are configured at the root level
3. Sync the project with Gradle files
4. Run on an emulator or physical device

**Note:** The app module is standalone and would need integration into a proper multi-module Gradle project structure for full functionality.

## Theme and UI

The app uses Material 3 with a custom theme (`JetpackComposeLearningTheme`) that supports both light and dark modes. UI components follow Jetpack Compose declarative patterns with `@Composable` functions and `@Preview` annotations for development.
