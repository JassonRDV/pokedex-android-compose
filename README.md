# Pokédex — Android App with Jetpack Compose

A native Android Pokédex built with Kotlin and Jetpack Compose. It uses PokeAPI to load Pokémon information and displays a grid of entries with a detail view.

## Features in the source

- A grid of Pokémon with their names, numbers, and images.
- A detail view showing the selected Pokémon's name, sprite, and types.
- Previous and next controls in the detail view.
- PokeAPI integration through Retrofit.
- ViewModel state and a repository layer.
- Image loading with Coil and dependency injection with Hilt.

## Screenshots

<p>
  <img src="images/1.png" width="200" alt="Pokédex screenshot 1">
  <img src="images/2.png" width="200" alt="Pokédex screenshot 2">
  <img src="images/3.png" width="200" alt="Pokédex screenshot 3">
</p>

## Technology

Kotlin, Jetpack Compose, Material 3, ViewModel, coroutines, Hilt, Retrofit, and Coil.

## Getting started

1. Clone this repository and open its root folder in Android Studio.
2. Install Android SDK 35 and configure a Gradle JDK compatible with the project; the source targets Java 21.
3. Sync the Gradle project.
4. Select an emulator or device running Android 8.0 / API 26 or newer.
5. Run the `app` configuration with internet access.

The current PokeAPI service does not require an API key.

To request a debug build on Windows:

```powershell
.\gradlew.bat assembleDebug
```

## Source guide

- [PokemonListScreen.kt](app/src/main/java/com/example/pokedex/ui/screens/PokemonListScreen.kt): Pokémon grid.
- [PokemonDetailScreen.kt](app/src/main/java/com/example/pokedex/ui/screens/PokemonDetailScreen.kt): selected entry and navigation controls.
- [PokemonViewModel.kt](app/src/main/java/com/example/pokedex/viewmodel/PokemonViewModel.kt): UI state and data loading.
- [PokeApiService.kt](app/src/main/java/com/example/pokedex/data/api/PokeApiService.kt): list and detail endpoints.
- [PokemonRepository.kt](app/src/main/java/com/example/pokedex/data/repository/PokemonRepository.kt): API access layer.

## Contact

[Jasson Ramos on LinkedIn](https://www.linkedin.com/in/jassonramos/)
