# Architectural Decision Record (ADR)

## Group Members

- [Elvis Chizoba]

## Scenario

### Scenario 1: Retail Mobile App

You are a team responsible for developing a new mobile app for a retail company. The app will allow customers to browse and purchase products, view their order history, and track the status of their deliveries. Additionally, the app will have a loyalty program feature, where customers can earn and redeem points for discounts on future purchases.

## Architectural Decision

### Decision 1: Native, Web, or Hybrid App

#### Decision

We have decided to develop a native mobile app for the retail company.

#### Rationale

1. Performance: Native apps offer superior performance compared to web or hybrid apps. This is crucial for providing a seamless shopping experience to customers.

2. Access to Device Features: Native apps have direct access to device features like camera, GPS, and push notifications, enabling enhanced functionalities such as product scanning and location-based notifications.

3. User Experience: Native apps can provide a consistent and polished user experience tailored to each platform (iOS and Android).

4. Offline Mode: Native apps can better support offline mode, allowing users to browse products and view order history even when not connected to the internet.

5. Security: Native apps provide a higher level of security, which is essential for handling user data, payments, and loyalty points.

#### Consequences

- Development Effort: Developing separate apps for iOS and Android requires additional development effort and resources.

- Maintenance: Ongoing maintenance and updates will be needed for both app versions.

- Platform-Specific Development: Native app development requires platform-specific skills and knowledge.

## Business Requirements Met

- The decision aligns with the business requirements of providing a high-performance, secure, and feature-rich app.

## User Needs Met

- The decision meets user needs for a responsive and user-friendly shopping experience.
