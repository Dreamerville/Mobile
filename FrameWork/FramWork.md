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

### Decision 2: UI Framework

#### Decision

We have decided to use a native UI framework for developing the retail mobile app's user interface.

#### Rationale

1.  Native Look and Feel : A native UI framework ensures that the app's user interface follows platform-specific design guidelines, providing a familiar and native look and feel to users.

2.  Optimal Performance : Native UI components are optimized for performance on their respective platforms, ensuring smooth interactions and responsiveness.

3.  Platform Integration : Native UI frameworks seamlessly integrate with platform-specific features, such as navigation patterns and gestures.

4.  Offline Mode Support : Native UI development allows us to implement offline mode features with greater control and reliability.

#### Consequences

-  Development Expertise : Developers need expertise in the chosen native UI framework for each platform (e.g., UIKit for iOS, Android XML for Android).

-  Development Time : Developing separate UI components for each platform may require additional development time compared to cross-platform UI frameworks.

-  Consistency : Ensuring a consistent user interface between platforms requires careful design and development.
