# Catalogue Maker

A Flutter app that turns product details and photos into a PDF catalogue. It grew out of a recurring catalogue workflow where gathering information, taking photos, and assembling the final PDF took place in separate tools.

![Catalogue Maker project and product screens](docs/images/catalogue-maker-screens.jpg)

## Workflow

1. Create a catalogue project and add its products.
2. Fill in product details and choose photos from the gallery or take them with the camera.
3. Open the PDF preview to review the generated catalogue.

Projects and products use Provider for state management and SQLite for local persistence. The app stores copies of chosen images on the device. Start with [the project screens](lib/screens), [the database helper](lib/helpers/db_helper.dart), and [the PDF preview](lib/screens/view_pdf_screen.dart).

Automatic photo background removal is a future idea.

## Run locally

Use a Flutter SDK that satisfies the Dart 2 constraint in [`pubspec.yaml`](pubspec.yaml). Run on a mobile device or emulator to try the image picker and on-device database.

```sh
flutter pub get
flutter run
```

## Dependency updates

Use `flutter pub get` to install the versions recorded in `pubspec.lock`.
The `archive` constraint keeps the resolver on releases with the fixes
for CVE-2023-39139 and CVE-2023-39137. Keep the version floor when updating
the packages that use it and review the lockfile before committing changes.
