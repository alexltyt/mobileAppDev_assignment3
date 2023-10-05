# Choice of UI Framework for the University Social Networking App

**Status:** Proposed
**Date:** 5 Oct 2023

## Context

With the decision to pursue a hybrid application development approach to cater to both iOS and Android users, the next crucial step is to choose an appropriate User Interface (UI) framework. This framework will play a significant role in determining the app's look, feel, performance, and overall user experience.

## Decision

**Choice:** Flutter

### Rationale

- **Cross-Platform Consistency:** Flutter offers a rich set of widgets that ensure a consistent look and feel across both platforms, eliminating the discrepancies that sometimes arise in cross-platform development.
- **Performance:** Flutter compiles to native ARM machine code using Dart's native compilers. This means we get the performance benefits of a native application.
- **Rapid Development:** The 'hot reload' feature in Flutter allows developers to instantly view the effect of the latest changes, making the development process faster and more efficient.
- **Extensive Library:** Flutter boasts a comprehensive set of material design and Cupertino (iOS-flavor) widgets, which can help in building a visually appealing app without much effort.
- **Customizability:** Flutter’s layered architecture allows for complete customization, meaning designers have more freedom to bring their vision to reality without limitations.

## Consequences

- **Learning Curve:** While Flutter is increasingly popular, if our development team is not familiar with it, there might be a learning curve involved. However, given Flutter's growing community and extensive documentation, this challenge is manageable.
- **Package Limitations:** While Flutter has a vast library of packages, it might sometimes lag behind native platforms in terms of certain functionalities. This would require the team to build custom plugins.
- **Future-Proofing:** With tech giants like Google backing Flutter, it's reasonably future-proof. Any updates or changes in the mobile development landscape will likely be quickly incorporated into the Flutter ecosystem.
