Change Log
==========

Version 0.9.6
-------------

- Add support for window insets on all edges (great for apps supporting edge-to-edge).
- Remove the need to call `LumberYard.install()` when using the Timber module.
- Remove the `timber-no-op` module; there's no code that needs to be included in release builds now.
- Add temporary LeakCanary2 module to make use of it while it's in beta.
- Fix bug where resource IDs would display as errors in Android Studio.
- Migrate deployment to Maven Central.

Version 0.9.5
-------------

- Add pretty printing JSON option in HTTP logger module

Version 0.9.4
-------------

- Fix crash on older versions of Android (at least on API 21 and 22)
- Fix state restoration of drawer and scroll view
- Bump various dependencies

Version 0.9.3
-------------

- Fix bug where Timber logs were not sharing
- Fix Timber log FileProvider [potentially clashing](https://commonsware.com/blog/2017/06/27/fileprovider-libraries.html) with consuming application

Version 0.9.2
-------------

- Add OkHttp log interceptor module
- Bump various dependencies, including AndroidX to the new stable release

Version 0.9.1
-------------

- Fix drawer not building correctly when no custom container provided in builder.

Version 0.9.0
-------------

Initial release of DebugDrawer, including modules for
 - Device info: Things like resolution and API level.
 - LeakCanary: Hides the launcher icon and provides access in the drawer.
 - Retrofit: Allows for changing endpoints and configuring mock behaviour.
 - Timber: Collects and displays Timber logs in a dialog.
