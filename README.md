# react-native-push-notification-app
# React Native Push Notification App

This project is a mobile application developed using React Native and Expo that demonstrates real-time push notifications. It simulates WhatsApp-style call alerts and supports background and killed-state delivery on Android devices, including Android 15.

## Features

- Push notifications using Expo Push API
- Background and killed-state notification support
- Local notification testing functionality
- Android 15 compatibility
- Deep linking data simulation via JSON payload
- Built entirely online using Expo Snack (no installation required)

## Technologies Used

- React Native (JavaScript)
- Expo SDK and Expo Go app
- Expo Push Notifications API
- Snack (Expo’s web-based development environment)

## How to Run

1. Open the project in Expo Snack or load the app in Expo Go using the shared QR code.
2. On launch, the app displays the Expo Push Token associated with the device.
3. Copy the token and use Expo’s notification tool at [https://expo.dev/notifications](https://expo.dev/notifications) to send a push notification.
4. The device receives the notification, even if the app is in the background or not running.

## Sample Push Payload

```json
{
  "to": "ExponentPushToken[xxxxxxxxxxxxxxxxxxxxxx]",
  "title": "Incoming Call",
  "body": "Tanmai Kiran is calling you now!",
  "data": {
    "screen": "CallScreen"
  }
}
