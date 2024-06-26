# Your Application Name

Your Application Name is a mobile and web application that allows users to create and save files with relevant information. The application uses Flutter, Provider, Django, and Firebase to provide a secure and scalable solution for file creation and storage.

## Installation

1. Clone the repository to your local machine.
   
    `git clone https://github.com/jehato47/sgs`


2. Install the Flutter SDK and set up your development environment. Follow the instructions for [macOS](https://flutter.dev/docs/get-started/install/macos), [Windows](https://flutter.dev/docs/get-started/install/windows), or [Linux](https://flutter.dev/docs/get-started/install/linux).

3. Install the required Flutter packages by running the following command in the project's root directory:

    `flutter pub get`



3. Start the mobile app by running it in your preferred development environment.

4. Use the application to create, view, and delete files with relevant information.

## Technology Stack

- Flutter (Dart)
- Provider for state management
- Django
- Firebase (Authentication and Cloud Storage)

## System Architecture

![System Architecture Diagram](https://i.imgur.com/qqEiCIn.png)

The Flutter-based mobile app and the web-based application both send requests to the Django server, which creates files with relevant information provided by the user. The files are then saved on Firebase Cloud Storage.

## User Authentication

Your application uses Firebase Authentication to authenticate users. Firebase Authentication provides secure authentication methods, such as email and password authentication, Google sign-in, and Facebook sign-in. When a user signs in to your application, Firebase Authentication returns a user ID token, which your application can use to verify the user's identity and secure user data.

## File Creation and Storage

When a user creates a file in your application, the file is saved in Firebase Cloud Storage. The file is saved with a unique file name, which is generated by the Django server. The file name consists of a unique identifier, the user ID, and the date and time the file was created. This ensures that each file is uniquely identified and can be easily retrieved later.

The file format depends on the information provided by the user. If the user provides text-based information, the file is saved in PDF format. If the user provides numerical data, the file is saved in XLSX format.

## User Interface

Your application has a user-friendly interface that allows users to easily create and save files. Here is an example of the user interface:

![User Interface Screenshot](https://i.imgur.com/KITeIGP.png)

The user interface consists of a form that allows users to enter relevant information. Once the user has entered the information, they can save the file, which is then stored in Firebase Cloud Storage.

## Functionality

Your application has the following functionalities:

- Create files: Users can create files by entering relevant information into a form. The files are saved in Firebase Cloud Storage.
- View files: Users can view their saved files in the app or web version.
- Delete files: Users can delete files they no longer need.

## Testing

