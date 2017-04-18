Fakeit
========

![alt text](https://github.com/moove-it/fakeit/blob/master/banner.png "Fakeit Github banner")

This library is a port of the Ruby gem [Faker](https://github.com/stympy/faker). It generates realistic fake data — like names, emails, dates, countries — to be used in your Android development environment. It can be used in a variety of scenarios, including automated testing and database population.

Download
--------
Maven
```xml
<dependency>
  <groupId>com.github.moove-it</groupId>
  <artifactId>fakeit</artifactId>
  <version>v0.2</version>
</dependency>
```
or Gradle:
```groovy
allprojects {
  repositories {
    maven { url 'https://jitpack.io' }
  }
}
  
dependencies {
  compile 'com.github.moove-it:fakeit:v0.2'
}
```

Basic usage
--------

Fakeit can be used in Java and Kotlin Android apps. Run the sample app to check all the available models and generate some random values.

First you need to initialize Fakeit:

```java
// Default locale is en
Fakeit.init(context)

// Or you can pass a Locale o a String locale
Fakeit.init(context, locale)
```

And then, call the methods like this:

```java
Fakeit.name().lastName()
Fakeit.business().type()
Fakeit.address().city()
Fakeit.card().name()
```

This is the current list of fake data models available:

- Address
- Ancient
- App
- Artist
- Bank
- Beer
- Book
- Business
- Card
- Cat
- Chuck Norris
- Code
- Company
- Compass
- Demographic
- Educator
- Esport
- File
- Food
- Friends
- Game of Thrones
- Hacker
- Harry Potter
- Hey Arnold
- Hipster
- Internet
- Job
- Lord of the Rings
- Lorem
- Music
- Name
- Phone number
- Pokemon
- Rick and Morty
- Rock band
        

Questions and issues
--------

For bug reports and feature requests, use [Github issue tracker](https://github.com/moove-it/fakeit/issues)

Contributing
--------

See the [contribution guide](CONTRIBUTING.md).

License
--------

[MIT](https://github.com/moove-it/fakeit/blob/master/LICENSE)

Fakeit is maintained by © [Moove-it](http://www.moove-it.com)
