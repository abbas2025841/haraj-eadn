# حراج عدن - Haraj Aden Classifieds Platform

## Overview

This is a comprehensive Android native classifieds application called "حراج عدن" (Haraj Aden) designed for buying and selling goods and services in Aden, Yemen. The application is built using modern Android development practices with Kotlin, Jetpack Compose, and follows clean architecture patterns with dependency injection using Hilt.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Android Architecture
- **Framework**: Android Native with Kotlin as the primary programming language
- **UI Framework**: Jetpack Compose for modern declarative UI development
- **Architecture Pattern**: Clean Architecture with MVVM pattern using ViewModel and Repository layers
- **Dependency Injection**: Hilt for dependency management and modular design
- **Database**: Room for local data persistence with SQLite backend
- **Navigation**: Jetpack Navigation Compose for type-safe navigation
- **Theming**: Material 3 Design System with custom colors for Yemeni market

### Project Structure Design
```
app/src/main/
├─ java/com/harajaden/
│  ├─ di/                ⟶ Hilt modules (DB, Network, Repository)
│  ├─ data/
│  │   ├─ local/
│  │   │   ├─ entity/    ⟶ Room entities & enums
│  │   │   ├─ dao/       ⟶ Room DAO interfaces
│  │   │   ├─ Converters.kt
│  │   │   └─ AppDatabase.kt
│  │   ├─ remote/        ⟶ Retrofit services (future API integration)
│  │   └─ repository/    ⟶ Single-source-of-truth layer
│  ├─ domain/            ⟶ Use-cases / business logic
│  ├─ ui/                ⟶ Compose screens
│  │   ├─ auth/
│  │   ├─ home/
│  │   ├─ listing/
│  │   ├─ components/
│  │   └─ theme/
│  ├─ util/              ⟶ Helpers / constants
│  └─ HarajAdenApp.kt    ⟶ Application class (Hilt)
└─ res/                  ⟶ Drawables, RTL strings, themes
```

### Configuration Management
- **Gradle Build System**: Multi-module Android application with proper dependency management
- **Room Database**: Local data persistence for offline-first experience
- **RTL Support**: Full Arabic language support with right-to-left layout
- **Material 3 Theming**: Custom color scheme matching Yemeni cultural preferences

## Technology Stack

### Core Technologies
- **Kotlin**: Modern Android development language with full coroutines support
- **Jetpack Compose**: Declarative UI toolkit for native Android interfaces
- **Hilt**: Dependency injection framework built on top of Dagger
- **Room**: Local database abstraction layer over SQLite
- **Navigation Compose**: Type-safe navigation for Compose applications

### UI/UX Libraries
- **Material 3**: Latest Material Design components and theming
- **Compose UI**: Core Compose libraries for UI development
- **Coil**: Modern image loading library for Android

### Database & Storage
- **Room**: Local database with entity relationships and type converters
- **Coroutines**: Asynchronous programming for database operations
- **Flow**: Reactive data streams for real-time UI updates

### Future Integration Ready
- **Retrofit**: HTTP client for future API integration
- **OkHttp**: Network layer with logging capabilities
- **Gson**: JSON serialization/deserialization

## Project Status

### Current Implementation
- ✅ Complete Android project structure with Kotlin and Compose
- ✅ Hilt dependency injection setup with database and repository modules
- ✅ Room database with entities for Categories, Listings, and Users
- ✅ Clean architecture implementation with repository pattern
- ✅ Material 3 theming with custom Yemeni-focused color scheme
- ✅ Home screen with gradient hero section and category grid
- ✅ Full Arabic RTL support with localized strings
- ✅ Navigation setup with Compose Navigation
- ✅ Type converters for complex data types (Date, List<String>)

### Ready for Development
The application is now ready for feature development with:
- Clean architecture foundation for scalable development
- Database layer ready for offline-first functionality
- Modern UI components following Material 3 guidelines
- Proper Arabic language and RTL layout support
- Dependency injection configured for easy testing and maintenance
- Future-ready structure for API integration and advanced features