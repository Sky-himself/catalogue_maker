# catalogue_maker

An app to ease the process of making the catalog of products for companies

## Getting Started

topics and challenges:
- data structure of the app(handling products and projects data in a nice way)
- Provider state management and nested providers
- picking images from camera and gallery and storing a copy of them in the proper path
- working with SQLite and storing the app state on device's storage
- creating a template and generating PDF files from the data that user inputs

## Features to be added

the next feature would be the ability to remove the background of the images that user provides, and this can be done by using a service by it's API(which is not free in long term usages) or to provide a custom API that does this job

## Dependency updates

Use `flutter pub get` to install the versions recorded in `pubspec.lock`.
The `archive` constraint keeps the resolver on releases with the fixes
for CVE-2023-39139 and CVE-2023-39137. Keep the version floor when updating
the packages that use it and review the lockfile before committing changes.
