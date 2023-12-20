# Ride Counter Android Application

Ride Counter is a simple Android application designed to help users keep track of their entries in the format of date and time.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Screenshots](#screenshots)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Overview

Ride Counter simplifies the process of recording travel instances by allowing users to mark date and time entries with a single click. Whether you're a frequent traveler or want to keep a log of memorable journeys, Ride Counter is a handy tool for managing your travel history on your Android device.

## Features

- **Mark Date and Time Entries:** Quickly record travel instances by clicking the "Mark Date" button on the main screen.
  
- **View Entries:** Easily review and manage all recorded travel entries using the "View Entries" button. Long-press on an entry to delete it.

- **SQLite Database:** Utilizes SQLite for efficient and reliable local data storage, ensuring your travel history is securely maintained.

## Screenshots

<div style="display:flex; justify-content: space-between; padding: 10px;">
    <img src="https://github.com/shreyuu/RideCounter/assets/91451934/c8fb9331-4259-4f84-84a1-351828dcfb89" alt="Screenshot 1" width="250"/>
    <img src="https://github.com/shreyuu/RideCounter/assets/91451934/43129d1e-04ff-436f-b46b-3bb83022d5c2" alt="Screenshot 2" width="250"/>
    <img src="https://github.com/shreyuu/RideCounter/assets/91451934/983551b1-6123-483e-b008-f63d1062866f" alt="Screenshot 3" width="250"/>
</div>

## Getting Started

To get started with Ride Counter on your local machine, follow these steps:

### Prerequisites

Ensure you have the following tools installed:

- [Android Studio](https://developer.android.com/studio) for Android application development.

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/shreyuu/RideCounter.git
    ```

2. Open the project in Android Studio.

3. Build and run the application on an emulator or a physical device.

## Usage

### 1. Marking Date Entries

1. Launch the Ride Counter Android application on your device.

2. On the main screen, click the "Mark Date" button to record a new date entry.

3. The application will store the current date and time in the format `dd-MM-yyyy HH:mm:ss`.

4. A toast message will confirm the successful marking of the date entry.

### 2. Viewing Date Entries

1. To view all recorded date entries, click the "View Entries" button on the main screen.

2. You will be navigated to the EntriesActivity, where a list of all date entries is displayed.

3. Long-press on an entry to trigger a confirmation dialog for deletion.

4. Confirm deletion to remove the selected date entry.

### Additional Information

- Date entries are stored in a SQLite database using the `DatabaseHelper` class.

- The `EntriesActivity` displays the list of entries using a RecyclerView.


## Project Structure

The project follows a typical Android project structure, organized into modules and key directories. Here's an overview of the main components:

### `app` Module

The `app` module contains the main application code. Inside this module, you'll find the following important directories and files:

- **`src` Directory:**
  - **`main` Directory:**
    - **`java` Directory:**
      - `com.example.ride_counter` Package:
        - **`MainActivity.java`:** The main activity handling the application's primary functionality.
        - **`EntriesActivity.java`:** Activity for displaying and managing the list of entries.
        - **`DatabaseHelper.java`:** Helper class for managing SQLite database operations.
    - **`res` Directory:**
      - **`layout` Directory:**
        - **`activity_main.xml`:** XML layout file for the main activity.
        - **`activity_entries.xml`:** XML layout file for the entries activity.

### `AndroidManifest.xml`

The AndroidManifest.xml file in the `app` module defines essential information about the application, such as activities, permissions, and application metadata.

### `res` Directory

The `res` directory contains various resources, including layout files, drawable images, and string resources used in the app's user interface.

### `DatabaseHelper.java`

The `DatabaseHelper.java` file provides a SQLite database helper class for managing date entries.

### `EntriesActivity.java`

The `EntriesActivity.java` file defines the EntriesActivity, responsible for displaying a list of date entries and supporting deletion.

### `AndroidManifest.xml`

The `AndroidManifest.xml` file includes application configuration details, activity declarations, and permissions.

### `activity_entries.xml`

The `activity_entries.xml` file specifies the layout for the EntriesActivity.

## Dependencies

The Ride Counter Android application uses the following dependencies:

### AndroidX Libraries

- `implementation 'androidx.appcompat:appcompat:1.3.1'`: AndroidX AppCompat library for modern UI features on older devices.
- `implementation 'androidx.constraintlayout:constraintlayout:2.1.0'`: AndroidX ConstraintLayout library for flexible layouts.
- `implementation 'androidx.recyclerview:recyclerview:1.2.1'`: AndroidX RecyclerView library for displaying lists.

### SQLite Database

The application uses SQLite for local data storage. SQLite is an open-source, serverless, and self-contained SQL database engine.

### Material Components Library

- `implementation 'com.google.android.material:material:1.4.0'`: Material Components library for modern UI elements.

**Note:** Ensure that the versions specified in your `build.gradle` files match the versions mentioned here or use the latest stable versions available.

These dependencies enhance the development experience and provide essential functionality for the Ride Counter Android application.

## Contributing

If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and submit a pull request.

## License

This project does not have a specific license. The code is provided as-is for educational and personal use. You are welcome to use, modify, and distribute it according to your own preferences. Please respect the licenses of the libraries and tools used in this project.

## Acknowledgments

This code was created as a personal project for count the number of travelling done using open-source libraries and tools.

Feel free to explore and customize the application based on your preferences. If you encounter any issues or have suggestions, please consider contributing or reporting them in the [Issues](https://github.com/shreyuu/RideCounter/issues) section.

Enjoy using Ride Counter!
