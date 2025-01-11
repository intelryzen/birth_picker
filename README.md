# BirthPicker Flutter Package

A customizable date picker widget for Flutter applications, designed specifically for selecting birth dates. It offers a seamless user experience by supporting platform-specific date pickers (Cupertino for iOS and Material for Android) and customizable UI components.

| **Keyboard Input Example**              | **iOS Date Picker Example**               | **Android Date Picker Example**            |
|-----------------------------------------|------------------------------------------|-------------------------------------------|
| ![screenshot1](https://github.com/user-attachments/assets/b84936e6-8a22-41c1-89a7-db49767244e6) | ![screenshot2](https://github.com/user-attachments/assets/c57173cd-f897-4b0b-a178-798cf345a7ed) | ![Screenshot3](https://github.com/user-attachments/assets/8fe735b7-2309-4207-921e-f29bd7ff1f00) |

## Features
- Supports both **iOS-style** (Cupertino) and **Android-style** (Material) date pickers.
- Auto-formats date fields (**year**, **month**, **day**) and validates input.
- Supports **localization** with customizable date field order.
- **Flexible input options**:  
  - Allows users to enter the date directly using the keyboard.  
  - Provides an **icon button** to easily select the date using a platform-specific date picker.

## Installation
1. Add the following line to your `pubspec.yaml` under `dependencies`:
    ```yaml
    birth_picker: ^0.0.2
    ```
2. Run the following command to install the package:

    ```bash
    flutter pub get
    ```

## Usage
Before using the `BirthPicker` widget, **initialize date formatting** by calling `initializeDateFormatting()` in your `main` function:

```dart
void main() async {
  WidgetsFlutterBinding.ensureInitialized();
  await initializeDateFormatting(); // Important: Initialize date formatting
  runApp(const MyApp());
}
