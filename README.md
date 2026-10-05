# SMS Gate Android Client

This is a native Android client for SMS Gateway for Android Cloud API.

## Build on your phone

1. Create a GitHub repository from your phone.
2. Upload this entire project.
3. Open the **Actions** tab.
4. Run **Build Android APK**.
5. Download `app-debug.apk` from the workflow artifact.
6. Install it on your Android phone.

The app talks directly to:
`https://api.sms-gate.app/3rdparty/v1`

It uses the documented Basic Authentication API and sends text messages with:
- `deviceId`
- `phoneNumbers`
- `simNumber`
- `textMessage`

## Credentials

The app starts with the server/device defaults. The password constant is intentionally `CHANGE_ME` in this source project. Enter your actual password under Gateway settings before sending.

Do not publish a real SMS Gate password in a public GitHub repository. Anyone with the APK/source can potentially recover credentials if they are compiled into the app.

## API

Current SMS Gate API docs:
https://docs.sms-gate.app/integration/api/
