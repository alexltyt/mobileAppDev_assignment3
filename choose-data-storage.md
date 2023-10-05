# Data Storage Selection for the University Social Networking App

**Status:** Proposed
**Date:** 4 Oct 2023

## Context

A robust data storage system is essential for our university social networking app. The app will be handling diverse data ranging from user profiles, academic announcements, and personal interactions to potentially sensitive data such as student grades. The storage solution should be secure, scalable, efficient, and support offline data access.

## Decision

**Choice:** MongoDB with Realm

### Rationale

- **Schema Flexibility:** MongoDB's schema-less nature is particularly suited for a dynamic environment like a social networking app. It allows for easy adjustments as the app grows and evolves.
- **Performance:** MongoDB provides high performance for large-scale applications, with capabilities to handle vast amounts of data without compromising speed.
- **Realm for Offline Capabilities:** Integrating MongoDB with Realm offers offline-first capabilities. Users can access and modify data even without internet connectivity, with subsequent synchronization when they go online.
- **Scalability:** MongoDB supports horizontal scaling, ensuring that as the user base grows, the database can be scaled out by adding more servers.
- **Security Features:** MongoDB offers built-in security features like encryption at rest, encryption in transit, and advanced auditing capabilities.

## Consequences

- **Complex Queries:** While MongoDB is great for many use-cases, complex queries can be more challenging compared to traditional relational databases.
- **Data Size:** MongoDB's BSON format means that it uses more storage space compared to some other databases. Proper optimization and regular clean-up processes will be necessary.
- **Learning Curve:** If the team is accustomed to relational databases, there might be a learning curve in adapting to a NoSQL solution like MongoDB.
