#Mockito: Best java mock for Unit testing
##UI Tests:
- These tests interact with the UI of your app, they emulate the user behavior and assert UI results. These are the slowest and most expensive tests you can write because they require a device/emulator to run. On Android, the most commonly used tools for UI testing are Espresso and UI Automator.
##Integration Tests:
- When you need to check how your code interacts with other parts of the Android framework but without the complexity of the UI. These tests don’t require a device/emulator to run. On Android, the most common tool for integration testing is Roboelectric.
##Unit Tests:
- The system under test (SUT) is one class and you focus only on it. All dependencies are considered to be working correctly (and ideally have their own unit tests :]), so they are mocked or stubbed.
These tests are the fastest and least expensive tests you can write because they don’t require a device/emulator to run. On Android, the most commonly used tools for unit testing are JUnit and Mockito.

https://www.raywenderlich.com/195-android-unit-testing-with-mockito

