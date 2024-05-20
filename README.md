# ChatApp

ChatApp is a real-time messaging application built using Android Studio, Kotlin, and Firebase. The app allows users to register, log in, and chat with each other in real-time.

## Features

- User Authentication (Sign Up, Log In, Log Out)
- Real-time Messaging
- User Profiles
- Online Status Indicator
- Push Notifications

## Technologies Used

- **Android Studio**: The official IDE for Android development.
- **Kotlin**: A modern programming language that makes developers happier.
- **Firebase Authentication**: To handle user authentication.
- **Firebase Firestore**: A flexible, scalable database for real-time data.
- **Firebase Cloud Messaging**: For push notifications.

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- **Android Studio**: Download and install from [here](https://developer.android.com/studio).
- **Firebase Project**: Create a Firebase project from [Firebase Console](https://console.firebase.google.com/).

### Configure Firebase:

Go to the Firebase Console, create a new project, and add an Android app to the project.
Download the google-services.json file and place it in the app directory of your project.
### Add Firebase SDK dependencies to your build.gradle files. Ensure your project-level build.gradle contains the classpath for Google services:
gradle

dependencies {
    classpath 'com.google.gms:google-services:4.3.10'
}
### Add the following to your app-level build.gradle file:
gradle

apply plugin: 'com.android.application'
apply plugin: 'com.google.gms.google-services'

dependencies {
    implementation platform('com.google.firebase:firebase-bom:28.4.2')
    implementation 'com.google.firebase:firebase-auth-ktx'
    implementation 'com.google.firebase:firebase-firestore-ktx'
    implementation 'com.google.firebase:firebase-messaging-ktx'
}
### Build and run the project:

Connect your Android device or use an emulator.
Click Run in Android Studio to build and launch the app.
###Usage
Register:

Open the app and navigate to the sign-up screen.
Fill in the registration form and create a new account.
Log In:

Log in using your email and password.
Chat:

Start a new chat by selecting a user from the user list.
Send and receive messages in real-time.
###Contributing
Contributions are welcome! Please fork this repository and submit a pull request for any changes you would like to make.

###License
This project is licensed under the MIT License. See the LICENSE file for details.
