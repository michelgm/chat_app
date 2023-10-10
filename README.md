# Flutter Chat App

This is a simple chat application built using Flutter, a popular open-source UI software development toolkit. The app allows users to engage in real-time text conversations.

## Features

- Real-time messaging
- User authentication
- User profiles
- Push notifications
- Emoji support

## Getting Started

### Prerequisites

- Flutter SDK installed on your machine. For installation instructions, visit [Flutter documentation](https://flutter.dev/docs/get-started/install).
- An IDE like Android Studio or Visual Studio Code with Flutter plugins installed.

### Running the App

1. **Clone the repository:**

    ```bash
    git clone https://github.com/michelgm/chat_app.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd chat_app
    ```

3. **Install dependencies:**

    ```bash
    flutter pub get
    ```

4. **Connect your device or use an emulator.**

5. **Run the app:**

    ```bash
    flutter run
    ```

## Configuring Firebase

This app uses Firebase for authentication and real-time database. Follow these steps to set up Firebase for your project:

1. Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.

2. Add your app to the project and follow the setup instructions provided.

3. Download the `google-services.json` file and place it in the `android/app` directory.

4. Enable Firebase Authentication and Firestore in the Firebase Console.

5. Update the Firebase configuration in your Flutter app. Open `lib/main.dart` and replace the Firebase initialization code with your own configuration.

    ```dart
    void main() async {
      WidgetsFlutterBinding.ensureInitialized();
      await Firebase.initializeApp(
        // Add your Firebase configuration here
      );
      runApp(MyApp());
    }
    ```

## Customization

You can customize the app by modifying the following files:

- `lib/screens/chat.dart`: Customize the chat screen UI.
- `lib/screens/auth.dart`: Customize the login screen UI.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


## Acknowledgments

- [Flutter](https://flutter.dev/)
- [Firebase](https://firebase.google.com/)
- [Academind](https://academind.com/)

