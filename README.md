# WORK MITRA — Flutter starter project

A blue-and-white Android + Web starter UI for a jobs and local-services marketplace.

## Included in this starter
- Mobile number + password login UI with basic form validation
- Language selector: English, Telugu, Hindi
- Customer / Worker role selection screen
- Home screen with service categories, job CTA, jobs tab and profile tab
- Responsive centered login layout suitable for web preview
- Flutter project structure and no third-party runtime dependencies

## Important prototype limitations
This is a **front-end prototype**, not a production-ready service. Login currently validates the form locally and creates an in-memory session. It does not create accounts, verify passwords, save user data, connect to a database, or send messages. Role selection is a UI placeholder. Backend authentication, database, worker verification, job posting, chat, payments, maps and admin authorization must be implemented and security-tested before launch.

## Run locally
Install Flutter SDK, then from this folder:

```bash
flutter pub get
flutter run
```

For Android APK:
```bash
flutter build apk --release
```

For web:
```bash
flutter config --enable-web
flutter build web --release
```

## Structure
```text
work_mitra/
  lib/
    main.dart
    app_state.dart
    screens/
      login_screen.dart
      role_screen.dart
      home_screen.dart
  assets/
  pubspec.yaml
  analysis_options.yaml
  README.md
```

## Next development phase
1. Connect Supabase project and configure secure authentication.
2. Create profiles, workers, categories, jobs, applications, bookings and reviews tables.
3. Add real registration and role-specific onboarding.
4. Add admin web dashboard with role-based access policies.
5. Test Telugu, Hindi and English layouts on Android and web.
