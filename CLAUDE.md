# iPad Journal App - Development Guide

## Project Overview

This is an iPad-native journaling application that combines handwritten input via Apple Pencil with structured prompts for personal development, productivity, and mental health.

## Development Standards

### Code Style
- Follow Swift best practices and conventions
- Use SwiftUI for all UI components
- Implement proper error handling and validation
- Write comprehensive unit tests for all business logic
- Use Core Data for persistence with proper data modeling

### Architecture
- MVVM pattern with SwiftUI
- Repository pattern for data access
- Dependency injection for testability
- Modular design with clear separation of concerns

### Testing Requirements
- Unit tests for all business logic
- UI tests for critical user journeys
- Performance tests for Apple Pencil rendering
- Accessibility testing for VoiceOver support

### Security & Privacy
- All journal data must be encrypted at rest
- Implement proper keychain storage for sensitive data
- Follow Apple's privacy guidelines
- No tracking or analytics without explicit user consent

## Apple Pencil Integration
- Use PencilKit framework for drawing and handwriting
- Implement handwriting recognition for search functionality
- Support pressure sensitivity and tilt
- Optimize for low-latency ink rendering

## Development Workflow
- Feature branch workflow with pull requests
- Continuous integration with automated testing
- Regular builds and testing on physical iPad devices
- Code reviews required for all changes

## Dependencies
- PencilKit for Apple Pencil support
- Core Data for local storage
- CloudKit for sync functionality
- Natural Language framework for text analysis