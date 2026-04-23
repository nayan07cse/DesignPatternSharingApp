# DesignPatternSharingApp

![Android CI](https://github.com/nayan07cse/DesignPatternSharingApp/actions/workflows/android.yml/badge.svg)

An Android application demonstrating the implementation of software design patterns in a practical item-sharing context.

## Modern Android Stack
This project has been updated to follow modern Android development standards:
- **Target SDK**: 33 (Android 13)
- **Language**: Java 17
- **Build System**: Gradle 7.5 + AGP 7.4.2
- **CI/CD**: Fully automated builds via GitHub Actions

## Design Patterns Implemented

### 1. Observer Pattern
Decouples the data models (`ItemList`, `ContactList`) from the UI components.
- **Subject**: `Observable.java`
- **Observer**: `Observer.java`
- **Impact**: Activities automatically refresh when the underlying data changes, eliminating manual UI sync logic.

### 2. Command Pattern
Used for contact management to encapsulate operations as objects.
- **Commands**: `AddContactCommand`, `DeleteContactCommand`, `EditContactCommand`.
- **Impact**: Encapsulates requests as objects, allowing for cleaner code and potential undo/redo functionality.

### 3. Model-View-Controller (MVC)
Strict separation of concerns using controllers to manage data persistence and business logic.
- **Model**: `Item`, `Contact`
- **Controller**: `ItemListController`, `ContactListController`, `ItemController`

## Features
- **Lend & Borrow**: Track items shared between contacts.
- **Local Persistence**: Data saved using GSON serialization for portable storage.
- **Media Support**: Capability to attach photos to items using the camera.
- **Contact Management**: Integrated contact list for assignment of items.

## Installation & Setup
1. Clone the repository: `git clone https://github.com/nayan07cse/DesignPatternSharingApp.git`
2. Open the project in **Android Studio (Flamingo or newer recommended)**.
3. Sync Gradle and run on a device or emulator with **Android 6.0 (API 23) or higher**.

---
*Developed as part of the Software Design and Architecture Specialization.*
