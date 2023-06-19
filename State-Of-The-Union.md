# What makes a great platform and great app?
- A great platform is more than a collection of frameworks and technologies.
- It is the combination of a language, frameworks, tools and services created to work together seemlessly to create something special.
- A great app uses the building blocks of the system integrate withint the system and extend on it. 

# What's new in Swift?
- Swift Macros
  - Pain point: Some APIs are hard to use, requiring a lot of boilerplate code just toget strated
  - Solution: Swift Macros, new kind of API to help use APIs easier 
  - Attached macros, to extend code to existing code e.g. @AddAsync
  - In order to understand under-the-hood, set a breakpointpoint, step into the macro function and Xcode expands the macro right in the source editor

- Swift <-> C++ Interoperability
  - Use both languages in the same project without a bridging layer

# What's new in SwiftUI?
- Animations
  - default to .spring(duration: , bounce: )
  - new animated symbols in SF Symbols
  - AnimationPhase API for multi-part animation
  - Keyframe Animation API for properties at specific times and the rest intermediate values are interpolated by SiwftUI
  
- Data
  - making it simpler by just focusing on @State and @Environment, the rest like ObservableObject can be handled using @Obsrvable Swift Macros
  - SwiftData framework for data modeling and management, built on top of CoreData (Objective-C specific) but for Swift, using @Model macro 

- App Experiences
  - Widget Kit: you can surface your content in many places across the system
    - also supports interactivity within the widget itself    
  - App Intents: your app's functionality is integrated into the system
    - withing spotlight, shortcuts and siri 
  - TipKit: you can surface beautiful tips directly in your app
    - inteligently educate users about features at the right time
    - customize template, add targetting, manage overall frequency 
  - AirDrop: share content to users that are nearby
    - ShareLink() in SwiftUi
  - StoreKit
    - Marketting and merchendising  

# What's new in Xcode?
- Source Editor
  - Code completion with prioritisation  
  - Macro for preview #Preview { ContentView() }
- Testing
  - Test results overview, more graphical, video recording of when the test failed  

# VisionOS
- Known frameworks: SwiftUI/UIKit (to build UI), RealityKit (to presnt 3D content), ARKit (to understand the space around users)
- Apps launch on Shared Space, can open window (SwiftUI scene, exisiting iOS apps), volumes (3d objects) and dedicated spaces (full space for a particular app)
- .offset z modifier for depth
- ornaments (affix UI components to the edges of windows and volumes), materials (adapt to the users environment) and hover effects (selects where the user looks)

# Accessebility
- Support for users sensitive to animations and flashing light
  - Pause Animated Images
  - Dim Flashing Lights in AVFoundation
- Vision OS
  - Spacitial computing with in-built accessibility features enabled   


# Privacy
- Calendar Prompts
  - when apps don't need access to calendar, only write new events, *Add Only Permission* 
- Photo access
  - users can choose if they provide only selected pictures or the full library, in-app *Photo Picker*
- App Security  
  - Privacy Manifests files and signatures for 3rd party SDKs  
  - Xcode combines all manifest into a single easy to ready report

      
