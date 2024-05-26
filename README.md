### Real-Time Object Detection App

#### Project Overview

This project is an Android application designed for real-time object detection using the camera feed. It leverages TensorFlow Lite for on-device machine learning to detect objects and classify them in real-time. The application also integrates Firebase to store detected objects' data, enabling further analysis and logging.

#### Features

- **Real-Time Object Detection:** Uses the device's camera to capture and process frames for object detection.
- **TensorFlow Lite Integration:** Utilizes a pre-trained TensorFlow Lite model (`AutoModel1`) to perform object detection.
- **Firebase Integration:** Detected objects and their metadata (class and confidence score) are uploaded to Firebase Realtime Database.
- **Visualization:** Draws bounding boxes and labels on the camera feed to visualize detected objects.

#### Technologies Used

- **Android SDK:** Core framework for building the Android application.
- **TensorFlow Lite:** For running the machine learning model on the device.
- **Firebase Realtime Database:** For storing and retrieving detected object data.
- **Camera2 API:** For accessing and managing the device's camera.
- **Kotlin:** Primary programming language for the application.

#### Installation and Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/rt-object-detection.git
   cd rt-object-detection
   ```

2. **Open in Android Studio:**
   - Open Android Studio.
   - Select "Open an existing Android Studio project".
   - Navigate to the cloned repository and open it.

3. **Configure Firebase:**
   - Add your `google-services.json` file to the `app` directory.
   - Ensure Firebase dependencies are included in your `build.gradle` files.

4. **Add Model and Labels:**
   - Place your TensorFlow Lite model file (`model.tflite`) in the `assets` directory.
   - Add your labels file (`labels.txt`) in the `assets` directory.

5. **Permissions:**
   - Ensure the app has camera permissions. The app will request permissions at runtime, but you can also add them manually in the `AndroidManifest.xml` file if necessary.

6. **Build and Run:**
   - Connect your Android device or use an emulator.
   - Click "Run" in Android Studio to build and deploy the app.

#### Usage

- **Launch the App:** Open the app on your Android device.
- **Grant Permissions:** Allow camera permissions when prompted.
- **Real-Time Detection:** The app will start the camera feed and display real-time object detection. Detected objects will be highlighted with bounding boxes and labels.
- **Firebase Logging:** Detected objects' data will be automatically sent to Firebase Realtime Database.



#### Contribution

Contributions are welcome! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request.

#### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
