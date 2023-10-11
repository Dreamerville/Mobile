# Architectural Decision Record (ADR)

## Group Members

- [Elvis Chizoba]


## Scenario

### Scenario 1: Retail Mobile App

You are a team responsible for developing a new mobile app for a retail company. The app will allow customers to browse and purchase products, view their order history, and track the status of their deliveries. Additionally, the app will have a loyalty program feature, where customers can earn and redeem points for discounts on future purchases. The following requirements must be considered:

1. The retail company wants the app to support offline mode, allowing customers to browse products and view their order history even when they are not connected to the internet. The app should sync data with the server once an internet connection is available.

2. The retail company wants to send push notifications to customers to notify them about order updates, new product arrivals, and exclusive offers. The app should integrate with a push notification service to handle the delivery of notifications.

3. The app needs to integrate with various payment gateways to facilitate secure and convenient transactions for customers. The team should select and integrate a suitable payment gateway or a combination of gateways based on security, ease of use, and compatibility with the app's target platforms.

## Architectural Decision

### Decision 5: Data Storage

#### Decision

We have decided to use a combination of relational and NoSQL databases for data storage in the retail mobile app.

#### Rationale

1.  Relational Database : We will use a relational database for structured data such as user profiles, orders, and loyalty program information. Relational databases provide data consistency and integrity.

2.  NoSQL Database : For unstructured or semi-structured data like product descriptions and reviews, we will use a NoSQL database. NoSQL databases offer flexibility and scalability for handling varying data formats.

3.  Offline Mode : The combination of databases will support the app's offline mode by providing access to essential data even without an internet connection.

4.  Scalability : This architecture allows us to scale specific database components independently based on their needs.

#### Consequences

-  Integration Complexity : Managing data across multiple database types may introduce integration challenges.

-  Maintenance : Ongoing maintenance and optimization of both database types will be required.

-  Data Consistency : Ensuring data consistency between the two types of databases may require synchronization mechanisms.
