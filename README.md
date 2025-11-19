# MovFlix

**MovFlix** is a feature-rich Flutter application that serves as your ultimate movie companion. Discover popular, trending, and top-rated movies, watch trailers, and manage your personal watchlist with ease.

## Features

- **Authentication**: Secure Login and Sign Up functionality using Firebase Authentication.
- **Movie Discovery**: Browse through Popular, Trending, and Top Rated movie lists.
- **Search**: Find movies instantly by title.
- **Detailed Information**: Access comprehensive movie details including overviews, ratings, release dates, genres, and runtime.
- **Trailers**: Watch movie trailers directly within the app (via YouTube).
- **Wishlist**: Save your favorite movies to a personalized watchlist (synced across devices using Firebase Realtime Database).
- **Similar Movies**: Discover new movies based on your interests.
- **Responsive UI**: A beautiful, dark-themed user interface built with Flutter.

## Tech Stack

- **Frontend**: [Flutter](https://flutter.dev/) (Dart)
- **Backend / BaaS**: [Firebase](https://firebase.google.com/)
  - **Authentication**: For user management.
  - **Realtime Database**: For storing user wishlists.
- **API**: [The Movie Database (TMDB)](https://www.themoviedb.org/documentation/api)
- **State Management**: `setState` (Native Flutter)

## Screenshots

*(Add your screenshots here)*

## Installation

Follow these steps to set up the project locally.

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) installed.
- A [TMDB API Key](https://www.themoviedb.org/documentation/api).
- A [Firebase Project](https://console.firebase.google.com/) set up.

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/movflix.git
   cd movflix
   ```

2. **Navigate to the project directory**
   ```bash
   cd movflix
   ```

3. **Install dependencies**
   ```bash
   flutter pub get
   ```

4. **Configure Firebase**
   - Create a project in the Firebase Console.
   - Add Android/iOS/Web apps to your Firebase project.
   - Download `google-services.json` (for Android) and place it in `android/app/`.
   - (Optional) Use `flutterfire configure` to automatically generate `firebase_options.dart`.

5. **Configure TMDB API**
   - Open `lib/services/movie_service.dart`.
   - Replace the `apiKey` variable with your own TMDB API key:
     ```dart
     final String apiKey = 'YOUR_TMDB_API_KEY';
     ```

6. **Run the App**
   ```bash
   flutter run
   ```

## Folder Structure

```
movflix/
├── lib/
│   ├── models/          # Data models (Movie, MovieDetails)
│   ├── screens/         # UI Screens (Home, Login, MovieList, etc.)
│   ├── services/        # API and Database services (MovieService, DatabaseService)
│   ├── main.dart        # Application entry point
│   └── firebase_options.dart # Firebase configuration
├── android/             # Android native code
├── ios/                 # iOS native code
├── web/                 # Web specific files
└── pubspec.yaml         # Dependencies
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made by [Your Name]
