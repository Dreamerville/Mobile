# Architectural Decision Record (ADR)

## Scenario

### Scenario 1: Retail Mobile App

You are a team responsible for developing a new mobile app for a retail company. The app will allow customers to browse and purchase products, view their order history, and track the status of their deliveries. Additionally, the app will have a loyalty program feature, where customers can earn and redeem points for discounts on future purchases.

## Architectural Decision

### Decision 5: Data Storage

#### Decision

We have decided to use a combination of SQL and NoSQL databases for data storage in the retail mobile app. SQL databases will be used for structured data, such as user profiles and order history, while NoSQL databases will handle semi-structured and unstructured data, such as product information and reviews.

#### Rationale

1. Structured Data: SQL databases offer strong data consistency and are suitable for structured data that requires complex queries and transactions.

2. Scalability: NoSQL databases excel in handling semi-structured and unstructured data, providing the flexibility needed for product information and user-generated content.

3. Hybrid Approach: The hybrid approach allows us to utilize the strengths of both SQL and NoSQL databases, optimizing data management based on specific use cases.

4. Reliability: Using a combination of databases ensures redundancy and reliability. Even if one database experiences issues, the other can continue to serve critical data.

#### Consequences

- Complex Data Synchronization: The team must implement synchronization mechanisms to ensure data consistency between SQL and NoSQL databases.

- Maintenance Overhead: Managing two types of databases increases maintenance complexity, including backups and updates.

- Skill Requirement: Developers need expertise in both SQL and NoSQL database management.

## Business Requirements Met

- The decision aligns with the business requirements of handling structured and unstructured data efficiently and reliably.

## User Needs Met

- The decision meets user needs by ensuring data consistency and performance for various types of data used within the app.
