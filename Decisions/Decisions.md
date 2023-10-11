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

### Decision 1: Native Mobile App Development

#### Decision

We have decided to develop the retail mobile app as a native mobile app, separately for iOS and Android platforms.

#### Rationale

1. **Platform-Specific Features**: Native development allows us to leverage platform-specific features and capabilities, providing an optimal user experience.

2. **Performance**: Native apps typically offer better performance as they are optimized for their respective platforms.

3. **Offline Mode**: Native development provides greater control over offline mode implementation, essential for the retail app's offline browsing feature.

4. **Push Notifications**: Native apps can seamlessly integrate with platform-specific push notification services for reliable delivery.

#### Consequences

- **Development Time**: Developing separate native apps may require more development time compared to cross-platform development.

- **Maintenance**: Separate codebases for iOS and Android will require ongoing maintenance.

- **Resource Allocation**: The team will need expertise in both iOS and Android development.
