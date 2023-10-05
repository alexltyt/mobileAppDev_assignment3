Student Name: MO CHAU, NGAN (Michael) &  SHEK YIN, LEUNG (Alex)    
Student ID: 886718,891365                                                     
 
 
Assignment 3: Architectural Decision Record (ADR)
 
Title: Architectural Decisions for University Social Networking Mobile App
 
Date: 4 Oct 2023
 
Status: Proposed
 
Context:
We are developing a social networking app tailored for university students and professors. The main aim of this app is to provide a platform for students to connect with each other, professors to post assignments, and everyone to manage schedules.
 
Decisions:
 
1. Native, Web, or Hybrid App:
 
Decision: Hybrid App
 
Rationale: Given the need to support both iOS and Android platforms, a hybrid approach using a framework like Flutter or React Native allows for writing mostly a single codebase for both platforms, ensuring faster development and easier maintenance.
 
2. UI Framework:
 
Decision: Flutter
 
Rationale: Flutter offers a rich set of fully customizable widgets to create native interfaces, helping maintain a consistent UI experience across both iOS and Android.
 
3. Backend Language:
 
Decision: Node.js
 
Rationale: Node.js is scalable and offers asynchronous operations. Its non-blocking nature is especially suitable for applications that require real-time operations, such as our university social networking app.

 
 
 
4. Permissions:
 
Decision: Role-Based Access Control (RBAC)
 
Rationale: With diverse user roles, such as students, professors, and administrators, RBAC allows for a granular permission system. This ensures that each user role only accesses the features and data they're supposed to.
 
5. Data Storage:
 
Decision: MongoDB with Realm
 
Rationale: MongoDB provides a flexible schema which is essential for the dynamic nature of a social networking app. Realm, in tandem with MongoDB, facilitates an offline-first design, which syncs data once the device is back online.
 
6. Accessibility
 
Decision: Implement accessibility widgets in Flutter and follow Web Content Accessibility Guidelines (WCAG).
 
Rationale: It's important that all users, regardless of their physical capabilities, can use the app seamlessly. Flutter provides a range of widgets to aid accessibility.
 
 
Consequences:
 
Performance Implications: While hybrid apps can sometimes lag native apps in terms of performance, the chosen frameworks ensure that this gap is minimal. Also, the benefit of code reusability and faster develop time worth the performance trade-offs.
 
Maintenance: The hybrid approach, coupled with a consistent backend language and unified data storage solution, simplifies the maintenance process.
 
Extensibility: Our choices allow for future extensibility. Whether it's adding new features or integrating with other platforms or tools, the modular nature of our decisions ensures that future developments can be easily integrated.
 
 
 
 
 
 
