# Architectural Decision Record (ADR) for University Social Networking Mobile App

## Title: 
Architectural Choices for a University Social Networking Application

## Status: 
Proposed

## Date: 
[Date]

---

## Context:

With the rise in digital platforms catering to educational needs, there's an emerging requirement for a tailored social networking app for a university context. This app will cater to students and professors, offering functionalities from academic announcements to social interactions. Understanding the diverse user base with varying device capabilities and connectivity conditions, as well as the inherent need for security in an academic setting, informs our architectural decisions.

---

## Decision:

### 1. Native, Web, or Hybrid App:
- **Decision:** Hybrid App
- **Rationale:** To cater to both iOS and Android platforms and streamline development, a hybrid approach using a framework like Flutter or React Native is chosen. 

### 2. UI Framework:
- **Decision:** Flutter
- **Rationale:** Flutter's robustness in delivering consistent and native interfaces across platforms is in alignment with our goal for seamless user experience.

### 3. Backend Language:
- **Decision:** Node.js
- **Rationale:** The asynchronous nature of Node.js makes it apt for a real-time application like ours.

### 4. Permissions:
- **Decision:** Role-Based Access Control (RBAC)
- **Rationale:** Diverse user roles demand a granular permission system, with RBAC ensuring appropriate access levels.

### 5. Data Storage:
- **Decision:** MongoDB with Realm
- **Rationale:** MongoDB's flexible schema is conducive for a dynamic social networking environment. Realm enhances this by providing offline data capabilities.

### 6. Additional Frameworks or Technology Stacks:
- **Decision:** Service Workers, LDAP, and AES encryption.
- **Rationale:** Service Workers ensure offline content availability, LDAP manages and accesses directory info for Active Directory integration, and AES ensures data encryption for security.

---

## Consequences:

- **Performance Implications:** While hybrid apps can sometimes lag behind native apps in terms of performance, the chosen frameworks ensure that this gap is minimal. Moreover, the benefit of code reusability and faster time-to-market outweighs the marginal performance trade-offs.
  
- **Maintenance:** The hybrid approach, coupled with a consistent backend language and unified data storage solution, simplifies the maintenance process. 
  
- **Security:** The decision to use AES encryption and LDAP integration might make the app slightly more complex, but it significantly enhances the security posture of the application, especially given the sensitivity of academic data.

- **Extensibility:** Our choices allow for future extensibility. Whether it's adding new features or integrating with other platforms or tools, the modular nature of our decisions ensures that future developments can be easily integrated.


