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

### Decision 3: Backend Language

#### Decision

We have decided to use [Backend Language] as the programming language for the retail mobile app's backend.

#### Rationale

1.  Familiarity : Our development team has extensive experience with [Backend Language], which will accelerate development and reduce potential issues.

2.  Community and Ecosystem : [Backend Language] has a strong community and a wide range of libraries and frameworks that can streamline backend development.

3.  Scalability : [Backend Language] offers scalability options, allowing us to handle increased traffic and data as the app grows.

4.  Compatibility : [Backend Language] is compatible with our chosen database and other technology stacks.

#### Consequences

-  Development Team Skills : We need to ensure that our development team is skilled in [Backend Language] to maximize productivity.

-  Maintenance : Ongoing maintenance and updates will require expertise in [Backend Language].

-  Compatibility : We must verify that [Backend Language] is compatible with the chosen database and other components of the system.
