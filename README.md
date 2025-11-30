# Calories Calculator

An Android application for calculating daily calorie requirements.

This exercise was the third weekly assignment for the course Mobile programming with Native Technologies in Oulu University of Applied Sciences.

## Features

- Calculate daily calorie needs based on weight, gender, and activity level
- Simple and clear user interface
- Built with Jetpack Compose

## Usage

1. Enter your weight in kilograms
2. Select your gender (Male/Female)
3. Select your activity level:
   - Light (1.3) - Little or no exercise
   - Usual (1.5) - Light exercise 1-3 days per week
   - Moderate (1.7) - Moderate exercise 3-5 days per week
   - Heavy (1.9) - Heavy exercise 6-7 days per week
   - Extreme (2.2) - Very heavy exercise and physical job
4. Press the "Calculate" button to see your daily calorie requirement

## Calculation Formula

- For males: (879 + 10.2 × weight) × activity multiplier
- For females: (795 + 7.18 × weight) × activity multiplier

## Project Structure

```
Calories/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/com/example/calories/
│   │       │   ├── MainActivity.kt                    # Main activity
│   │       │   └── ui/
│   │       │       ├── components/
│   │       │       │   ├── Calculation.kt            # Calorie calculation logic
│   │       │       │   ├── GenderChoices.kt          # Gender selection component
│   │       │       │   ├── Heading.kt                # App title component
│   │       │       │   └── IntesityList.kt           # Activity level dropdown
│   │       │       └── theme/
│   │       │           └── Theme.kt                  # Material 3 theme configuration
│   │       ├── res/
│   │       │   ├── drawable/                         # App icons and images
│   │       │   ├── values/                           # Strings, colors, themes
│   │       │   └── xml/                              # Backup and data extraction rules
│   │       └── AndroidManifest.xml
│   └── build.gradle.kts                              # App-level Gradle configuration
├── gradle/
│   └── libs.versions.toml                            # Dependency version catalog
├── build.gradle.kts                                  # Project-level Gradle configuration
└── settings.gradle.kts                               # Gradle settings
```

## Technology

- Kotlin
- Jetpack Compose
- Material Design 3
- Android SDK 35

