# Compiling from source

## Prerequisites

- JDK (Get from [SDKMAN!](https://sdkman.io) or [Adoptium](https://adoptium.net))
- Dart SDK (Get from [here](https://dart.dev/get-dart#install))
- [CPP dev tools](https://docs.gradle.org/current/userguide/native_software.html#sec:tool_chain_installation) (Only if you're on Linux or macOS)
- [WIX Toolset](https://wixtoolset.org/releases/) (Only if you're on Windows)

If you installed the Dart SDK please add the path to the SDK into the `local.properties` file (if it doesn't exist,
create it)

```properties
# (this is when you did 'winget install dart'
dart.sdk=C:\\Program Files\\Dart\\dart-sdk
```

## Build on macOS and Linux

```
./gradlew assemble
```

## Build on Windows

```
gradlew assembleMsi
```

In both cases you will find your output in `build/distributions`
