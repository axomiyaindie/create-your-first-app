# Skill: Build a Native Android App

**Goal:** Take a user from zero to a running native Android app in Kotlin + Jetpack Compose.

## Prerequisites check
- Android Studio installed  ->  https://developer.android.com/studio
- JDK 17+ (bundled with Android Studio)
- `adb devices` lists at least one device/emulator

## Steps

1. **Create project (manual, in Android Studio)**
   - File -> New -> New Project
   - Template: **Empty Activity** (Compose)
   - Name: `MyApp`
   - Package: `com.example.myapp`
   - Language: Kotlin  |  Minimum SDK: API 24
   - Build configuration language: Kotlin DSL
   - Click Finish and wait for Gradle sync

2. **Ask the user what the app does** (one sentence). Then build:
   - `MainActivity.kt` with `setContent { MyApp() }`
   - `ui/theme/` (leave the generated theme files)
   - `ui/HomeScreen.kt` - LazyColumn list
   - `ui/DetailScreen.kt` - detail view
   - Navigation Compose between the two screens

3. **Add dependencies** in `app/build.gradle.kts`:
   ```kotlin
   implementation("androidx.navigation:navigation-compose:2.8.0")
   implementation("androidx.compose.material3:material3:1.3.0")
   ```

4. **Run**
   - Click the green Run button in Android Studio, or
   ```bash
   ./gradlew installDebug
   adb shell am start -n com.example.myapp/.MainActivity
   ```

5. **Commit**
   ```bash
   git init && git add . && git commit -m "feat: initial android app"
   ```

## Rules for the agent
- Use Jetpack Compose only (no XML layouts).
- Use Material 3.
- One composable per file for anything reusable.
- Do not add extra dependencies without explaining why.
- Explain each command in one short sentence before running it.

## Done when
- App installs and launches on emulator or device.
- Home screen shows a list.
- Tapping an item opens the detail screen.
- Back navigation works.

