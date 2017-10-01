# ![Kloggs logo](http://i.imgur.com/8VjjUUh.png) Kloggs
[![](https://img.shields.io/badge/Kotlin-1.1.1-blue.svg)](https://kotlinlang.org/)
[![Build Status](https://travis-ci.org/Minikloon/Kloggs.svg?branch=master)](https://travis-ci.org/Minikloon/Kloggs)
[![Download](https://api.bintray.com/packages/minikloon/Kloggs/Kloggs/images/download.svg) ](https://bintray.com/minikloon/Kloggs/Kloggs/_latestVersion)

Kloggs is a single-file Kotlin utility adding lambda-based logging methods over [slf4j](https://www.slf4j.org/).
These methods have a performance advantage over string concatenation and are more elegant than [parameterized methods](https://www.slf4j.org/faq.html#logging_performance).
Kloggs is a play on the cereal brand.
The library (if you can call it that) is available under [MIT License](https://tldrlegal.com/license/mit-license).

# Install

Kloggs is available on Maven through Jitpack.

Maven:
```xml
<repository>
    <id>jitpack.io</id>
    <url>https://jitpack.io</url>
</repository>
<dependency>
    <groupId>com.github.Minikloon</groupId>
    <artifactId>Kloggs</artifactId>
    <version>[Version Tag]</version>
</dependency>
```

Gradle:
```groovy
repositories {
	...
	maven { url 'https://jitpack.io' }
}
dependencies {
	compile 'com.github.Minikloon:Kloggs:[Version Tag]'
}
```

# Usage

**1. Get a logger.**
```kotlin
private val log = logger<MyFavoriteClass>()
class MyFavoriteClass
```

**2. Use the logger.**
```kotlin
log.info { "User $username has logged in!" }
```

**3. The end.**
