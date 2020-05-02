# Movie Catalogue
![GitHub stars](https://img.shields.io/github/stars/rrifafauzikomara/MovieCatalogue.svg?style=flat&logo=github&colorB=deeppink&label=stars)
![GitHub forks](https://img.shields.io/github/forks/rrifafauzikomara/MovieCatalogue?style=flat&logo=github&colorB=deeppink&label=stars)
![GitHub watchers](https://img.shields.io/github/watchers/rrifafauzikomara/MovieCatalogue?style=flat&logo=github&colorB=deeppink&label=stars)

[![GitHub license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Open Source Love](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/rrifafauzikomara/MovieCatalogue)
[![platform](https://img.shields.io/badge/platform-Flutter-blue.svg)](https://flutter.dev/)


## About Flutter
Flutter is Google's SDK for crafting beautiful, fast user experiences for
mobile, web and desktop from a single codebase. Flutter works with existing
code, is used by developers and organizations around the world, and is free
and open source. We think Flutter will help you create beautiful, fast apps, with a productive,
extensible and open development model.


## Quick start
This is a normal flutter app. You should follow the instructions in the [official documentation](https://flutter.io/docs/get-started/install).
This project uses **BLoC** (business logic component) to separate the business logic with UI itself.
It's recommended to do self-study about it before jumping into the project [here](https://bloclibrary.dev/).
And also on this project uses **Modularization** approach to separate each feature ([core](https://github.com/rrifafauzikomara/MovieCatalogue/tree/master/core), [shared](https://github.com/rrifafauzikomara/MovieCatalogue/tree/master/shared), [ui](https://github.com/rrifafauzikomara/MovieCatalogue/tree/master/lib/ui) modules).
You can do self-study about it in [here](https://github.com/rrifafauzikomara/flutter_modularization).


## Features
*  Support Dark Mode and Light Mode 🔥
*  Now Playing Movies
*  Up Coming Movies
*  Popular Movies
*  Top Rated Movies
*  Detail Movies
*  Favorite (ala style 😜)


## Example iOS
<pre>
<img src="screenshot/ios1.png" width="250" height="460">     <img src="screenshot/ios2.png" width="250" height="460">     <img src="screenshot/ios3.png" width="250" height="460">
</pre>


## Example Android
<pre>
<img src="screenshot/android1.png" width="250" height="460">     <img src="screenshot/android2.png" width="250" height="460">     <img src="screenshot/android3.png" width="250" height="460">
</pre>


## Libraries
* [BLoC Pattern](https://bloclibrary.dev/)
* [Equatable](https://pub.dev/packages/equatable)
* [Retrofit](https://pub.dartlang.org/packages/retrofit) with [Dio](https://github.com/flutterchina/dio/)
* [Json Serializable](https://pub.dev/packages/json_serializable)
* [Build Runner](https://pub.dev/packages/build_runner)
* [Shared Preferences](https://pub.dev/packages/shared_preferences) for Cache Implementation
* [Modularization](https://github.com/rrifafauzikomara/flutter_modularization) for [core](https://github.com/rrifafauzikomara/MovieCatalogue/tree/master/core) and [shared](https://github.com/rrifafauzikomara/MovieCatalogue/tree/master/shared) modules
* [Shimmer Loading](https://pub.dev/packages/shimmer)
* [Flutter Launcher Icons](https://pub.dev/packages/flutter_launcher_icons)
* [Integration Testing](https://flutter.dev/docs/cookbook/testing/integration/introduction) for development Flavor
* [Flavor](https://medium.com/@animeshjain/build-flavors-in-flutter-android-and-ios-with-different-firebase-projects-per-flavor-27c5c5dac10b) on Android and iOS (development and production)


## Todo
* [ ] Unit Testing (Mockito)
* [ ] Build and Release for iOS


## How to run Flutter App
Before run the app, make sure you have an emulator running, or a device connected over USB and debugging enabled on that device.
Then you need to register the `API_KEY` from www.themoviedb.org then enter the `API_KEY` into ***api_constant.dart*** file

```
static const apiKey = "HERE";
```


If you want to generate file `*.g.dart`, you can use this command on terminal. But before you running that, make sure go to [core](https://github.com/rrifafauzikomara/MovieCatalogue/tree/master/core) module first using `cd` command. For example `cd core`. Then you can run the command below.

One time build:
```console
flutter pub run build_runner build
```
or you can watch for changes and rebuild automatically
```console
flutter pub run build_runner watch
```


### Run Flutter app between Flavor for development and production with command prompt
Development
```console
flutter run --flavor development --target=lib/ui/launcher/main-dev.dart
```
Production
```console
flutter run --flavor production --target=lib/ui/launcher/main-prod.dart
```


### Run Flutter app between Flavor for development and production with <img src="https://github.com/rrifafauzikomara/MovieCatalogue/blob/master/screenshot/running.png" alt="Run" width="20" height="20"/>
<pre>
<img src="https://github.com/rrifafauzikomara/MovieCatalogue/blob/master/screenshot/tutor1.png" alt="Tutor1" />
<img src="https://github.com/rrifafauzikomara/MovieCatalogue/blob/master/screenshot/tutor2.png" alt="Tutor2" />
<img src="https://github.com/rrifafauzikomara/MovieCatalogue/blob/master/screenshot/tutor3.png" alt="Tutor3" />
</pre>


## How to run the Test
### Integration Testing
```console
flutter drive --target=test_driver/app.dart --flavor development
```


## License

```
MIT License

Copyright (c) [2020] [R Rifa Fauzi Komara]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```


## Author

* **R Rifa Fauzi Komara**

Don't forget to follow me, fork and give me a ★