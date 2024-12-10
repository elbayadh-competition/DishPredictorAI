## University Center El Cherif Bouchoucha Aflou

# Dish Prediction App

The Dish Prediction App is a Flutter application that uses a TensorFlow Lite model to predict the best dish based on the user's input ingredients. This app leverages AI to assist users in making informed decisions about meals, making it an excellent tool for culinary exploration and personalized recommendations. The app is designed to help universities and students avoid food waste and support allergic students by recommending suitable dishes.

## Features

- **User-Friendly Interface**: Simple and intuitive design to input ingredients and view predictions.
- **AI-Powered Predictions**: Utilizes a TensorFlow Lite model for accurate dish recommendations.
- **Real-Time Performance**: Instant predictions with optimized model inference.
- **Admin Gradio Interface**: Provides an admin page for managing input and predictions via Gradio.
- **Student-Centric Design**: Helps students avoid food waste and supports allergic individuals with meal recommendations.

## How the Database is Built

The database for this app was constructed by scraping various web pages and converting the extracted data into a structured CSV file. This dataset includes detailed information about dishes and their ingredients, enabling robust model training and accurate predictions.

## Getting Started

Follow the instructions below to set up and run the application.

### Prerequisites

- Flutter SDK installed on your machine ([Flutter installation guide](https://flutter.dev/docs/get-started/install)).
- Android Studio or Visual Studio Code with Flutter and Dart plugins installed.
- TensorFlow Lite model file (`dish_predictor_model.tflite`).

### Installation

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/elbayadh-competition/dish-prediction-app.git
    cd dish-prediction-app
    ```

2. **Add the TensorFlow Lite Model**:
   - Place the `dish_predictor_model.tflite` file in the `assets` directory of the project.
   - Update the `pubspec.yaml` file to include the model in the app's assets:

     ```yaml
     flutter:
       assets:
         - assets/dish_predictor_model.tflite
     ```

3. **Install Dependencies**:

    ```bash
    flutter pub get
    ```

4. **Run the App**:
   - Connect your device or start an emulator.
   - Use the following command to run the app:

     ```bash
     flutter run
     ```

## Pages Overview

### 1. **Authentication Page**
   - Allows users to log in with a username and admin password (`123456789` by default).

### 2. **Information Page**
   - Users can enter details into the database, including their preferences and allergies.

### 3. **Home Page**
   - Displays three main categories:
     - Residence
     - Transport
     - Meals

### 4. **Dish Recommendation Page**
   - Focused on students entering what they dislike or are allergic to.
   - Uses the trained TensorFlow Lite model to recommend suitable dishes based on their inputs.

### Admin Interface
   - Admins can use the Gradio-powered page to manage and test dish predictions. The admin page is accessible at the provided Gradio link (e.g., https://5817a8c8a8745a7527.gradio.live).

## Project Structure

The project follows the standard Flutter directory structure:

```
lib/
├── main.dart             # App entry point
├── dish_prediction.dart  # Model loading and prediction logic
assets/
└── dish_predictor_model.tflite  # TensorFlow Lite model
```

## Model Details

The app uses a pre-trained TensorFlow Lite model (`dish_predictor_model.tflite`) that predicts dishes based on ingredients. The model was trained on a curated dataset of popular dishes and their ingredients. Ensure the input format matches the preprocessing used during model training.

## Dependencies

The app uses the following dependencies:

- [Flutter](https://flutter.dev/): Cross-platform UI toolkit.
- [tflite](https://pub.dev/packages/tflite): TensorFlow Lite plugin for Flutter.
- [Gradio](https://gradio.app/): Interface for the admin page.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- Thanks to TensorFlow and Flutter communities for their amazing tools and documentation.
- Special thanks to contributors and testers for their feedback and suggestions.

## Contact

For questions or support, feel free to reach out:

- **Email**: tenbrains1@gmail.com
- **GitHub**: [elbayadh-competition](https://github.com/elbayadh-competition)

---
## The link of the gradio admin page 
https://5817a8c8a8745a7527.gradio.live/

Enjoy using the Dish Prediction App for making the university life smarter 
