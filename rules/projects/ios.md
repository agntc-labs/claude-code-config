---
paths:
  - "**/*.swift"
  - "**/ios/**"
  - "**/*.xcodeproj/**"
  - "**/*.xcworkspace/**"
---

# iOS Development Rules

## SwiftUI Patterns
- Use `@StateObject` for owned objects
- Use `@ObservedObject` for passed objects
- Use `@EnvironmentObject` for app-wide state
- Prefer `async/await` over Combine for new code

## Firebase iOS
```swift
import FirebaseCore
import FirebaseAuth
import FirebaseFirestore

// Initialize in App init
FirebaseApp.configure()
```

## Project Locations
| Project | Path |
|---------|------|
| Digital Justin App | ~/Documents/Digital Justin App/ |
| Music Video | ~/Documents/Music Video/ |
| Home Service | ~/projects/ai/Home Service App/apps/ios/ |

## Build Issues
- Clean: `Cmd+Shift+K`
- Derived Data: `~/Library/Developer/Xcode/DerivedData/`
- SPM cache: `rm -rf ~/Library/Caches/org.swift.swiftpm/`

## Signing
Most projects need Xcode sign-in for device deployment.
Simulator works without signing.
