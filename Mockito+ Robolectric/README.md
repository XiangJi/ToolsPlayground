#Mockito: Best java mock for Unit testing
##UI Tests:
- These tests interact with the UI of your app, they emulate the user behavior and assert UI results. These are the slowest and most expensive tests you can write because they require a device/emulator to run. On Android, the most commonly used tools for UI testing are Espresso and UI Automator.
##Integration Tests:
- When you need to check how your code interacts with other parts of the Android framework but without the complexity of the UI. These tests don’t require a device/emulator to run. On Android, the most common tool for integration testing is Roboelectric.
##Unit Tests:
- The system under test (SUT) is one class and you focus only on it. All dependencies are considered to be working correctly (and ideally have their own unit tests :]), so they are mocked or stubbed.
These tests are the fastest and least expensive tests you can write because they don’t require a device/emulator to run. On Android, the most commonly used tools for unit testing are JUnit and Mockito.

https://www.raywenderlich.com/195-android-unit-testing-with-mockito



# Robolectric

最后说道要测试Android代码逻辑，光有JUnit和Mockito是不够的，假设你使用了TextView的setText,用Mockito框架的话，默认的TextView的getText方法会返回null,如果是简单的代码，使用Mockito的桩设置还可以接受，如果是要测试到Activity的生命周期等一些复杂逻辑就显得比较复杂了。

  为了解决这个问题,诞生了Instrumentation、Robolectric等等的测试框架，不过Instrumentation实际上还是要运行代码到平台上测试，耗费大量的时间，我们今天要介绍的是运行在JVM上的Robolectric测试框架。

https://maxwell-nc.github.io/android/robolectricTest.html





Running tests on an Android emulator or device is slow! Building, deploying, and launching the app often takes a minute or more. That’s no way to do TDD. There must be a better way.



http://robolectric.org/

