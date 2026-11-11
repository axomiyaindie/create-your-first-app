# Skill: Build a Flutter App

**Goal:** Take a user from zero to a running Flutter app (iOS + Android) without prior coding knowledge.

## Prerequisites check
- `flutter --version` -> 3.x+
- `dart --version`
- Android Studio installed (for Android builds)
- Xcode installed (for iOS builds, macOS only)

If missing, guide the user to https://docs.flutter.dev/get-started/install for their OS.

## Steps

1. **Create project**
   ```bash
   flutter create my_app
   cd my_app
   ```

2. **Clean up**
   - Delete the counter demo from `lib/main.dart`
   - Keep `MaterialApp` and theme

3. **Ask the user what the app does** (one sentence). Then build:
   - `lib/screens/home_screen.dart` - list view
   - `lib/screens/detail_screen.dart` - detail page
   - `lib/widgets/item_card.dart` - reusable card
   - Bottom navigation with 2 tabs (Home, Settings)
   - Simple `setState` state management (no external packages yet)

4. **Run**
   ```bash
   flutter devices
   flutter run
   ```
   If no device: use an Android emulator from Android Studio.

5. **Commit**
   ```bash
   git init && git add . && git commit -m "feat: initial flutter app"
   ```

## Rules for the agent
- Use Material 3 (`useMaterial3: true`).
- One widget per file for anything reusable.
- No external state packages (Riverpod / Bloc) unless the user asks.
- Never edit `android/` or `ios/` config unless required.
- Explain each command in one short sentence before running it.

## Done when
- `flutter run` launches on at least one device/emulator.
- Home screen shows a list.
- Tapping an item opens the detail screen.
- Bottom navigation switches between tabs.

