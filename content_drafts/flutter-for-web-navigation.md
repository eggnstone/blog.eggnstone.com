---
title: "New Flutter App From Scratch"
subtitle: "Creating a new Flutter app from scratch with logging, Analytics, Crashlytics, proper icons and splash screen."
lead: "Creating a new Flutter app from scratch with logging, Analytics, Crashlytics, proper icons and splash screen."
description: "description: Creating a new Flutter app from scratch with logging, Analytics, Crashlytics, proper icons and splash screen."
createdAt: 2021-03-01T00:00:00.000Z
updatedAt: 2021-03-20T00:00:00.000Z
cover: 
  image: "/images/Flutter Animation.gif"
  alt: "Flutter"
  thumb: "/images/Flutter Plain 103x128.jpg"
tags: 
  - Flutter
  - Android
  - iOS
  - Web
---
### Motivation
This is how I create my new [Flutter](https://flutter.dev) apps. 
The choices are my personal preferences and yours probably differ.

### Creation and initial cleanup of the main module
To create an app named `AbcXyz` I want `AbcXyzApp` as the project name and `com.example.abc_xyz` as the package name.
- Do **not** use the "New Flutter project" wizard in Android Studio / IntelliJ IDEA.
- Use the command line: `flutter create  --org com.example --project-name abc_xyz AbcXyzApp`

#### git
- Create a git repository and commit all files.
- Remove `*.iml` from `.gitignore` and add the uncovered `.iml` files.
- You can find my example repository at [Github](https://github.com/eggnstone/AbcXyzApp)
  
#### `pubspec.yaml` cleanup
- `pubspec.yaml` cleanup
  - Remove all comments.
  - Add proper copyright.
  - Set version to start at `0.0.1+1`.
  - Set min Dart SDK version to `2.12.0` for sound null safety. 

#### `main.dart` cleanup
  - Remove all comments.
  - Extract app and main screen out to separate files. One file should only host one class if possible. I make exceptions for very closely related classes like a widget and its state class.
  
### Android
- [ ] Android cleanup
- [ ] Android launcher icons
- [ ] Android notification icons
- [ ] Android splash screen

### iOS
- [ ] iOS cleanup
- [ ] iOS launcher icons
- [ ] iOS notification icons
- [ ] iOS splash screen

### Web
- [ ] iOS cleanup
- [ ] Cachebuster

### Adding Analytics

### Adding Crashlytics