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

### Decision 6: Any Additional Frameworks or Technology Stacks

#### Decision

We have decided to incorporate the following additional frameworks and technology stacks into the retail mobile app:

1.  Firebase : We will integrate Firebase for real-time database capabilities, authentication, and cloud messaging to support offline mode and push notifications.

2.  React Native : For certain cross-platform features, we will use React Native to streamline development and maintain a consistent user experience across platforms.

#### Rationale

1.  Firebase : Firebase provides essential features such as real-time data synchronization, user authentication, and push notifications, aligning with the app's requirements.

2.  React Native : React Native allows us to develop and maintain specific cross-platform features efficiently, reducing development time and effort.

#### Consequences

-  Learning Curve : Team members will need to familiarize themselves with Firebase and React Native if they are not already experienced.

-  Integration Complexity : Integrating multiple frameworks may introduce complexity into the development process.
