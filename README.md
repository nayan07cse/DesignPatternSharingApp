# DesignPatternSharingApp

An Android application demonstrating the implementation of software design patterns in a practical item-sharing context.

## 🚀 Overview
This project is an evolution of a "Sharing App" used to manage items and contacts. The primary goal is to showcase **clean architecture** and the practical application of **GoF (Gang of Four) Design Patterns** to create a maintainable and scalable codebase.

## 🛠 Design Patterns Implemented

### 1. Observer Pattern
Decouples the data models (`ItemList`, `ContactList`) from the UI components.
- **Subject**: `Observable.java`
- **Observer**: `Observer.java`
- **Impact**: Activities automatically refresh when the underlying data changes, eliminating manual UI sync logic.

### 2. Command Pattern
Used for contact management to encapsulate operations as objects.
- **Commands**: `AddContactCommand.java`, `DeleteContactCommand.java`, `EditContactCommand.java`.
- **Impact**: Encapsulates requests as objects, allowing for easier maintenance and potential undo/redo functionality.

### 3. Model-View-Controller (MVC)
Strict separation of concerns using controllers to manage data persistence and business logic.
- **Model**: `Item`, `Contact`
- **Controller**: `ItemListController`, `ContactListController`

## 📦 Features
- **Lend & Borrow**: Track items shared between contacts.
- **Local Persistence**: Data saved securely using internal storage.
- **Dynamic UI**: Responsive layouts for adding/editing items with photo support.

## ⚙️ Installation
1. Clone the repository.
2. Open in **Android Studio**.
3. Sync Gradle and run on a device with **API 23+**.

---
*Developed as part of the Software Design and Architecture Specialization.*
