# Selection of App Platform: Native, Web, or Hybrid

**Status:** Proposed
**Date:** 5 Oct 2023

## Context

The digital landscape is vast with diverse user bases spanning across various device platforms, mainly iOS and Android. With our objective to cater to a university audience comprising of students and professors, it's imperative to offer a seamless experience regardless of the device platform. Considering this, the decision regarding whether to go native, web, or hybrid is crucial.

## Decision

**Choice:** Hybrid App

### Rationale

- **Unified Development:** A hybrid approach, especially using frameworks like Flutter or React Native, allows for writing a single codebase that works efficiently on both iOS and Android. This not only reduces development time but also ensures consistency in features and functionality across platforms.
- **Cost Efficiency:** Developing separate native apps for iOS and Android can be resource-intensive. With a hybrid approach, we can optimize resource allocation, resulting in cost savings.
- **Faster Time-to-Market:** With a unified codebase, the time taken from development to deployment reduces significantly. This ensures that we can get the app to our university audience faster.
- **Flexibility:** Hybrid frameworks are generally equipped with plugins and integrations that allow the app to access device-specific features, ensuring users get a near-native experience.

## Consequences

- **Performance Consideration:** While hybrid apps have come a long way and offer near-native performance, there might be specific instances or features where a native app could outperform. However, with proper optimization and using the right tools, this gap can be minimized.
- **Maintenance:** Updates or changes can be rolled out for both platforms simultaneously, making maintenance streamlined. Moreover, issues can be addressed universally, ensuring consistent app quality.
- **Future Scalability:** As technology evolves, it might be easier to scale or integrate new features into a hybrid app, given its flexible architecture.
