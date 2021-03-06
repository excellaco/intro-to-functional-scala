# Scala Curriculum I Guide

Follow the curriculim of learning resources below, including our primer, [Intro to Functional Scala](README.md). See that you're gaining an understanding of the key concepts below.

## Key Concepts

Scala:

  - [1.1 Why Functional? Why Scala?](README.md#section-11---why-scala)
  - [1.2 Getting Started](README.md#12-getting-started)
    - Referential integrity, pure functions, indempotence, uniform access principle
    - functional vs. imperative
    - Hallmark functional features  
      - Higher Order Functions, functions as first class values, sequence comprehensions, yield, combinators
      - Closures
      - Currying
    - anonymous functions    
    - expressions (vs statements), evaluation, functional loops with and without fors, function structure, final variables, string interpolation, mutable collectors & operations, [tail recursion](https://www.scala-exercises.org/scala_tutorial/tail_recursion)
- [1.3 Functional Data Structures](https://www.scala-exercises.org/fp_in_scala/functional_data_structures)
- [1.4 Exceptions without Errors](README.md#1.4-Exceptions-without-errors)
  - [Why do we need monads?](https://stackoverflow.com/questions/28139259/why-do-we-need-monads/28139260#28139260)
- [2.1 Scala Intro](README.md#Section-21---Intro)
  - Object-oriented meets functional
  - Syntactically concise
  - Pure objected-oriented
  - Have opererator overloading
  - can be use in compiled or interpreted mode, compiles to bytecoder (and interoperable with Java) or JavaSxript, interpreted in tools like a REPL
- [2.4 Object orientation](README.md#251-Object-Orientation)
  - functions vs objects (functions are objects)
  (https://docs.scala-lang.org/tour/traits.html), generics, subtyping, variance, etc.
  - functions vs methods
  - [traits](https://docs.scala-lang.org/tour/traits.html)
  - classes in hierarchies; hierarchy of standard Scala types; polymorphism
  - organize classes and traits into packages
  - [case classes](https://docs.scala-lang.org/tour/case-classes.html)
  - implicit classes
    - [Finding implicits](https://docs.scala-lang.org/tutorials/FAQ/finding-implicits.html)
  - [DI in Scala](https://di-in-scala.github.io/)
- [2.4.2 Polymorphism and Types](README.md#242-Polymorphism-and-types)
- [2.5 Pattern Matching](README.md#2.5-Pattern-Matching)
  - collections data structure
  - pattern matching
  - [for comprehensions](https://docs.scala-lang.org/tour/for-comprehensions.html)
  - [map to map functions to elements, flatmap for returning in 1 list](http://www.brunton-spall.co.uk/post/2011/12/02/map-map-and-flatmap-in-scala/)
  - fold, reduce, shift
  - tuples - like a list but fixed in size and can hold objects with different types. They can be used to return multiple values at once, and are also useful to pass a list of data values as messages between actors in concurrent programming.
  - [Option](http://danielwestheide.com/blog/2012/12/19/the-neophytes-guide-to-scala-part-5-the-option-type.html) - type for representing optional values instead of null, so forces the compiler to deal with it
  - Match as a switch
  - [monads](https://medium.com/@sinisalouc/demystifying-the-monad-in-scala-cc716bb6f534), monoids
- [2.6 - Abstractions for concurrency](README.md#section-26---concurrency)
  - [futures/promises](README.md#futures-and-promises)
  - semaphores, actors, etc
- [Testing](README.md#27-Testing---scalatest-and-specs)
- [sbt](README.md#using-sbt)

Play:

Open-source scalable web framework in Scala or Java (JVM), based on a lightweight, stateless web-friendly architecture & built on Akka. Predictable & minimal resource consumption.

  - [Main concepts overview](https://www.playframework.com/documentation/2.6.x/ScalaHome)
    - [App architecture](https://www.playframework.com/documentation/2.6.x/Anatomy)
    - [Working with Play, deploying, etc](https://www.playframework.com/documentation/2.6.x/Home)
    - [Configuration API](https://www.playframework.com/documentation/2.6.x/ScalaConfig)
    - Actions - represents HTTP response to client, [Essential Action](https://www.playframework.com/documentation/2.6.x/ScalaEssentialAction)
    - [Routing](), [session & flash scopes (state available next request only, via cookies so 4kb max strings only)](https://www.playframework.com/documentation/2.6.x/ScalaSessionFlash)
    - [Body parsers](https://www.playframework.com/documentation/2.6.x/ScalaBodyParsers)
    - [Error Handling](https://www.playframework.com/documentation/2.6.x/ScalaErrorHandling)
    - [Async, futures](https://www.playframework.com/documentation/2.6.x/ScalaAsync)
    - [Streaming HTTP responses](https://www.playframework.com/documentation/2.6.x/ScalaStream)
    (https://www.playframework.com/documentation/2.6.x/ScalaActions)
    - Comet, WebSocket
    - [Template engine](https://www.playframework.com/documentation/2.6.x/ScalaTemplates)
    - [Working with JSON](https://www.playframework.com/documentation/2.6.x/ScalaJson)
    - Databases
      - [Accessing a database via Slick, functional relational mapper (FRM)](https://www.playframework.com/documentation/2.6.x/PlaySlick)
        - [Database Evolutions](https://www.playframework.com/documentation/2.6.x/Evolutions)
        - Work with data almost as if using Scala collections
        - Full control over when database access happens and what data is transferred
        - Can use SQL directly
        - Database actions are executed asynchronously so good for reactive apps based on Play & Akka
      - [Access a database via Anorm for more complex queries or legacy databases](https://www.playframework.com/documentation/2.6.x/ScalaAnorm)
    - [Cache API via Ehcache](https://www.playframework.com/documentation/2.6.x/ScalaCache)
    - [Runtime DI](https://www.playframework.com/documentation/2.6.x/ScalaDependencyInjection) and [Compile-time DI](https://www.playframework.com/documentation/2.6.x/ScalaCompileTimeDependencyInjection)
    - [Logging API](https://www.playframework.com/documentation/2.6.x/ScalaLogging)
    - [Testing](https://www.playframework.com/documentation/2.6.x/ScalaTestingYourApplication)
      - [With a database](https://www.playframework.com/documentation/2.6.x/ScalaTestingWithDatabases)
      = [Web service clients](https://www.playframework.com/documentation/2.6.x/ScalaTestingWebServiceClients)
  - Kalium cryptography

## Learning Steps

### 1: Preliminary Concepts & Scala Foundation

1. JVM necessities: how the JVM works, garbage collection, commands, tools, whats new in the JDK, etc. [Video tutorial on JVM](https://www.safaribooksonline.com/library/view/introduction-to-jvm/9781788834513/)
1. [Video Overview of Scala from Martin Odersky, creator](https://www.youtube.com/watch?v=ecekSCX3B4Q)
1. [Fundamentals First (video)](https://www.youtube.com/watch?v=ugHsIj60VfQ)
1. [Our guide, Intro to Functional Scala](README.md)
1. Scala exercises:
    1. [Scala exercises - std lib](https://www.scala-exercises.org/std_lib)
    1. [Scala exercises - exercise concepts](https://www.scala-exercises.org/scala_tutorial/terms_and_types)
    1. [Excerism.io - katas](hhttp://exercism.io/languages/scala/exercises)
1. [Scala for the Impatient (book)](http://fileadmin.cs.lth.se/scala/scala-impatient.pdf)
1. [Video clips of each concept](https://www.safaribooksonline.com/library/view/practical-scala-for/9781491969472/)

### 2: Play

1. [Play Concepts overview](https://www.playframework.com/documentation/2.6.x/ScalaHome)
1. First tutorial:
  - Create a Welcome to Play scaffold: `playframework/play-scala-seed.g8` then `sbt run`
  - Pick up with this [tutorial here](https://spr.com/building-a-simple-rest-api-with-scala-play-part-2/)
    - See view returned, edit `/conf/routes` to add a GET, /api to same controller class `HomeController` and in there add a new function to return a string like `def indexapi() = Action { Ok("Hello from Play API!") }`.
    - Add new controller, data access
    - [Create an Actor and use it](https://www.playframework.com/documentation/2.6.x/ScalaAkka)

  Additional examples:

  - [Play web framework tutorials](https://www.playframework.com/documentation/2.6.x/Tutorials) - including for Slick, JPA, Anom, EBean, Comet, WebSocket, Kalium cryptography, compile time DI
  - [Play starter example](https://github.com/playframework/play-scala-starter-example)
  - [Play, Scala,  REST API Example](https://github.com/playframework/play-scala-rest-api-example)
  - [Play, Scala, Slick example](https://github.com/playframework/play-scala-slick-example)
  - [Creating forms with Play](http://pedrorijo.com/blog/play-forms/#getting-started)

### 4: In-depth Learning

- [Neophyte's Guide to Scala - a little deeper in explaining concepts](http://danielwestheide.com/scala/neophytes.html)
- [Coursera Course, Functional Programming Principles in Scala](https://www.coursera.org/learn/progfun1)
- [Twitter Scala School](https://twitter.github.io/scala_school/)
- [Get the most out of Scala with Functional Programming in Scala (Scala book club used it)](https://www.manning.com/books/functional-programming-in-scala)
- [Martin Odersky's Programming in Scala book](https://www.scala-lang.org/docu/files/ScalaByExample.pdf)
- [Scala By Example (PDF)](http://www.scala-lang.org/docu/files/ScalaByExample.pdf)
