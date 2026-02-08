# Awesome Scala Native [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) with stars

<a href="http://www.scala-native.org/"><img alt="Scala Native" align="right" width="250" height="250" src="logo.png"></a>

[Scala Native](http://www.scala-native.org/) is an optimising ahead-of-time compiler for the [Scala programming language](https://www.scala-lang.org/). Traditionally, a virtual machine, the [JVM](https://en.wikipedia.org/wiki/Java_virtual_machine), was required to run Scala programs. Scala Native taps into the compiler to emit [LLVM intermediate representation](http://llvm.org/docs/LangRef.html) rather than JVM bytecode. Then, the [LLVM](http://llvm.org/) compiler infrastructure is used to produce native libraries and executables. Given that Scala Native executables are stand-alone programs, they generally have a shorter start-up time and low memory consumption. This opens up new avenues to deploy Scala programs where previously the virtual machine would be the limiting factor. For example, developers could write programs for the command line or embedded devices.

## Contents

* [Awesome Scala Native ](#awesome-scala-native-)
  * [Contents](#contents)
  * [Tutorials and Examples](#tutorials-and-examples)
  * [Build Tools](#build-tools)
  * [Functional Programming](#functional-programming)
  * [Unit Tests](#unit-tests)
  * [Bindings](#bindings)
  * [File Formats and Parsers](#file-formats-and-parsers)
  * [Databases](#databases)
  * [Web Development](#web-development)
  * [Concurrency](#concurrency)
  * [Logging](#logging)
  * [Console](#console)
  * [Robotics](#robotics)
  * [Programs](#programs)
  * [Infrastructure](#infrastructure)
  * [Licence](#licence)

## Tutorials and Examples

* [Giter8 template for a minimal Scala Native project](https://github.com/scala-native/scala-native.g8) ⭐ 79 | 🐛 1 | 🌐 Scala | 📅 2026-02-05 - Official [Giter8](http://www.foundweekends.org/giter8/) template for a minimal Scala Native project.
* [Example project with external dependencies](https://github.com/lihaoyi/scala-native-example-app) ⭐ 54 | 🐛 2 | 🌐 Scala | 📅 2024-07-16 - Example project that uses external dependencies to generate HTML and run a test suite.
* [Hands on Scala Native](https://github.com/MasseGuillaume/hands-on-scala-native) ⭐ 32 | 🐛 0 | 🌐 Scala | 📅 2018-06-19 - Tutorial for implementing a bandwidth monitor with Ncurses.
* [Starter for Scala Native](https://github.com/GnaneshKunal/scala-native-starter) ⚠️ Archived - Scala Native project that links to a custom C library.
* [Write a simple CLI application in Scala Native](https://github.com/ItoYo16u/prettytable-native) ⭐ 11 | 🐛 12 | 🌐 Scala | 📅 2023-06-05
* [Building C code using sbt-jni](https://github.com/nadavwr/scala-native-sbt-jni-example) ⭐ 6 | 🐛 0 | 🌐 CMake | 📅 2017-05-19 - Example for compiling C code in a Scala Native project using [sbt-jni](https://github.com/jodersky/sbt-jni) ⭐ 133 | 🐛 7 | 🌐 Scala | 📅 2026-02-01.
* [Starter for Gtk+ Projects](https://github.com/jokade/scalanative-gtk-seed.g8) ⭐ 2 | 🐛 0 | 🌐 Scala | 📅 2019-06-23 - [Giter8](http://www.foundweekends.org/giter8/) template for Scala Native GUI projects using [Gtk+](https://developer.gnome.org/gtk3/stable/index.html).
* [Modern systems programming with scala native](https://pragprog.com/titles/rwscala/modern-systems-programming-with-scala-native/) book.

## Build Tools

* [Mill](https://github.com/com-lihaoyi/mill) ⭐ 2,684 | 🐛 153 | 🌐 Scala | 📅 2026-02-08 - Build tool striving for simplicity, inspired by [Bazel](https://www.bazel.build/).
* [Bloop](https://github.com/scalacenter/bloop) ⭐ 938 | 🐛 87 | 🌐 Scala | 📅 2026-02-07 - Scala build server and command-line tool for fast developer workflows.
* [Seed](https://github.com/tindzk/seed) ⭐ 238 | 🐛 24 | 🌐 Scala | 📅 2020-12-11 - Build tool based on Bloop. Focuses on user experience and cross-platform builds, inspired by [Cargo](https://github.com/rust-lang/cargo) ⭐ 14,562 | 🐛 1,567 | 🌐 Rust | 📅 2026-02-08.
* [sbt](https://www.scala-sbt.org/) - Scala's standard build tool.

## Functional Programming

* [Cats](https://github.com/typelevel/cats) ⭐ 5,411 | 🐛 262 | 🌐 Scala | 📅 2026-02-04 - Abstractions for functional programming in Scala.
* [scalaz](https://github.com/scalaz/scalaz) ⭐ 4,678 | 🐛 155 | 🌐 Scala | 📅 2026-02-04 - Type classes and instances for data structures.
* [Shapeless](https://github.com/milessabin/shapeless) ⭐ 3,407 | 🐛 28 | 🌐 Scala | 📅 2026-02-05 - Library for generic programming.
* [chimney](https://github.com/scalalandio/chimney) ⭐ 1,240 | 🐛 23 | 🌐 Scala | 📅 2026-02-05 - Boilerplate-free data transformations.
* [Squants](https://github.com/typelevel/squants) ⭐ 930 | 🐛 63 | 🌐 Scala | 📅 2026-01-12 - DSL for quantities, units of measure and dimensional analysis.
* [Quicklens](https://github.com/softwaremill/quicklens) ⭐ 845 | 🐛 42 | 🌐 Scala | 📅 2026-01-25 - Modify deeply nested case class fields.
* [SourceCode](https://github.com/lihaoyi/sourcecode) ⭐ 538 | 🐛 33 | 🌐 Scala | 📅 2025-10-15 - Implicits providing meta data similar to `__LINE__` in C.
* [PPrint](https://github.com/lihaoyi/PPrint) ⭐ 248 | 🐛 19 | 🌐 Scala | 📅 2025-12-04 - Pretty-print values and types.
* [reactify](https://github.com/outr/reactify) ⭐ 90 | 🐛 8 | 🌐 Scala | 📅 2026-02-08 - Functional Reactive Programming framework for Scala.
* [nobox](https://github.com/xuwei-k/nobox) ⭐ 33 | 🐛 0 | 🌐 Scala | 📅 2026-02-04 - Immutable primitive array wrapper without boxing.

## Unit Tests

* [ScalaCheck](https://github.com/typelevel/scalacheck) ⭐ 1,961 | 🐛 63 | 🌐 Scala | 📅 2026-02-04 - Property-based testing for Scala.
* [ScalaTest](https://github.com/scalatest/scalatest) ⭐ 1,167 | 🐛 543 | 🌐 Scala | 📅 2025-11-14 - Testing library.
* [specs2](https://github.com/etorreborre/specs2) ⭐ 737 | 🐛 9 | 🌐 Scala | 📅 2026-02-05 - Software Specifications for Scala.
* [µTest](https://github.com/lihaoyi/utest) ⭐ 509 | 🐛 17 | 🌐 Scala | 📅 2026-01-22 - Library for unit tests.
* [MUnit](https://github.com/scalameta/munit) ⭐ 464 | 🐛 40 | 🌐 Scala | 📅 2026-02-06 - Scala testing library with actionable errors and extensible APIs.
* [scalaprops](https://github.com/scalaprops/scalaprops) ⭐ 279 | 🐛 10 | 🌐 Scala | 📅 2026-02-04 - Library for property-based testing.
  * [scalaprops-shapeless](https://github.com/scalaprops/scalaprops-shapeless) ⭐ 10 | 🐛 2 | 🌐 Scala | 📅 2026-02-04 - Generation of arbitrary ADT instances.
  * [scalaprops-cross-example](https://github.com/scalaprops/scalaprops-cross-example) ⭐ 4 | 🐛 0 | 🌐 Scala | 📅 2026-02-04 - Cross-platform example.
* [minitest](https://github.com/monix/minitest) ⭐ 181 | 🐛 12 | 🌐 Scala | 📅 2024-08-12 - Lightweight testing library.
* [Makeshift](https://github.com/nadavwr/makeshift) ⭐ 1 | 🐛 0 | 🌐 Scala | 📅 2018-03-10 - Library for unit tests.

## Bindings

* [libui](https://github.com/lolgab/scalaui) ⭐ 72 | 🐛 0 | 🌐 Scala | 📅 2024-07-18 - GUI framework based on [libui](https://github.com/andlabs/libui) ⭐ 10,858 | 🐛 249 | 🌐 C | 📅 2024-05-29.
* [SDL2 and OpenGL](https://github.com/regb/scalanative-graphics-bindings) ⭐ 43 | 🐛 3 | 🌐 Scala | 📅 2022-08-02 - Bindings for the graphical frameworks [SDL2](https://www.libsdl.org/) and [OpenGL](https://www.opengl.org).
* [BLAS](https://github.com/ekrich/sblas) ⭐ 35 | 🐛 0 | 🌐 Scala | 📅 2026-02-08 - Bindings for [BLAS](http://www.netlib.org/blas/), a library for Linear Algebra.
* [Gtk+](https://github.com/jokade/scalanative-gtk) ⭐ 27 | 🐛 1 | 🌐 Scala | 📅 2020-10-11 - Bindings for the [GTK+](https://www.gtk.org/) graphical toolkit.
* [Cocoa](https://github.com/jokade/scalanative-cocoa) ⭐ 22 | 🐛 7 | 🌐 Scala | 📅 2023-04-11 - Bindings for the macOS graphical framework [Cocoa](https://en.wikipedia.org/wiki/Cocoa_\(API\)).
* [cmark](https://github.com/sparsetech/cmark-scala) ⭐ 16 | 🐛 0 | 🌐 Scala | 📅 2021-09-14 - Bindings for the [cmark](https://github.com/commonmark/cmark) ⭐ 1,921 | 🐛 70 | 🌐 C | 📅 2025-12-21 CommonMark parser library.
* [libuv](https://github.com/TimothyKlim/scala-native-libuv) ⭐ 10 | 🐛 0 | 🌐 Scala | 📅 2017-04-29 - Bindings for [libuv](https://github.com/libuv/libuv) ⭐ 26,553 | 🐛 214 | 🌐 C | 📅 2026-02-05, a library for asynchronous I/O.
* [Qt](https://github.com/jokade/scalanative-qt5) ⭐ 9 | 🐛 0 | 🌐 Scala | 📅 2020-01-06 - Bindings for [Qt](https://www.qt.io).
* [ncurses](https://github.com/edadma/ncurses) ⭐ 6 | 🐛 1 | 🌐 Scala | 📅 2025-02-16 - Bindings for the [GNU Ncurses Library](https://www.gnu.org/software/ncurses/).
* [GNU Scientific Library](https://github.com/ruivieira/scala-gsl) ⭐ 3 | 🐛 0 | 🌐 Scala | 📅 2017-10-18 - Bindings for [GNU Scientific Library (GSL)](https://www.gnu.org/software/gsl).
* [libsoup](https://github.com/jokade/scalanative-libsoup) ⚠️ Archived - Bindings for the [libsoup](https://wiki.gnome.org/Projects/libsoup) HTTP client/server library.
* [GStreamer](https://github.com/jokade/scalanative-gstreamer) ⭐ 3 | 🐛 0 | 🌐 Scala | 📅 2019-10-04 - Bindings for the [GStreamer](https://gstreamer.freedesktop.org) multimedia framework.
* [libcairo](https://github.com/edadma/libcairo) ⭐ 3 | 🐛 0 | 🌐 C | 📅 2025-05-19 - Bindings for the [Cairo](https://www.cairographics.org/) 2D graphics C library.
* [libsndfile](https://github.com/edadma/libsndfile) ⭐ 2 | 🐛 0 | 🌐 Scala | 📅 2021-09-05 - Bindings for the [Libsndfile](https://tiswww.cwru.edu/php/chet/libsndfile/rltop.html) C library for sampled sound manipulation.
* [iup](https://github.com/edadma/iup) ⭐ 2 | 🐛 0 | 🌐 Scala | 📅 2023-01-07 - Bindings for the [IUP](https://www.tecgraf.puc-rio.br/iup/) multi-platform toolkit for building graphical user interfaces.
* [readline](https://github.com/edadma/readline) ⭐ 0 | 🐛 0 | 🌐 Scala | 📅 2025-08-16 - Bindings for the [GNU Readline Library](https://www.gnu.org/software/readline/).
* [libpng](https://github.com/edadma/libpng) ⭐ 0 | 🐛 0 | 🌐 C | 📅 2021-09-07 - Bindings for the [libpng](http://www.libpng.org/) C reference library for reading and writing PNGs.
* [cairo-xlib](https://github.com/edadma/cairo-xlib) ⭐ 0 | 🐛 0 | 🌐 Scala | 📅 2021-09-18 - Bindings for the [Cairo](https://www.cairographics.org/) 2D graphics [XLib Surfaces](https://www.cairographics.org/manual/cairo-XLib-Surfaces.html) with bindings for [XLib](https://www.x.org/releases/current/doc/libX11/libX11/libX11.html) as well.
* [libyaml](https://github.com/edadma/libyaml) ⭐ 0 | 🐛 0 | 🌐 Scala | 📅 2021-10-04 - Bindings for the [LibYAML](https://pyyaml.org/wiki/LibYAML) C library for parsing [YAML](https://yaml.org/).

## File Formats and Parsers

* [ScalaPB](https://github.com/scalapb/ScalaPB) ⭐ 1,332 | 🐛 58 | 🌐 Scala | 📅 2026-02-05 - [Protocol Buffer](https://developers.google.com/protocol-buffers/) compiler for Scala.
  * [scalapb-argonaut](https://github.com/scalapb-json/scalapb-argonaut) ⭐ 2 | 🐛 0 | 🌐 Scala | 📅 2026-02-04 - JSON and Protocol Buffer converters for ScalaPB based on [Argonaut](http://argonaut.io).
* [FastParse](https://github.com/com-lihaoyi/fastparse) ⭐ 1,130 | 🐛 23 | 🌐 Scala | 📅 2026-01-14 - Library for defining and running parsers.
* [scalatags](https://github.com/com-lihaoyi/scalatags) ⭐ 772 | 🐛 40 | 🌐 Scala | 📅 2025-07-11 - HTML/XML construction and rendering.
* [uPickle](https://github.com/com-lihaoyi/upickle) ⭐ 764 | 🐛 27 | 🌐 Scala | 📅 2026-01-14 - uPickle: a simple, fast, dependency-free JSON & Binary (MessagePack) serialization library for Scala
* [argonaut](https://github.com/argonaut-io/argonaut) ⭐ 547 | 🐛 28 | 🌐 Scala | 📅 2026-02-05 - Purely functional JSON parser and library.
* [sconfig](https://github.com/ekrich/sconfig) ⭐ 131 | 🐛 11 | 🌐 Scala | 📅 2026-02-08 - [HOCON](https://github.com/ekrich/sconfig/blob/master/docs/original/HOCON.md) ⭐ 131 | 🐛 11 | 🌐 Scala | 📅 2026-02-08 parser.
* [Pine](https://github.com/sparsetech/pine) ⭐ 110 | 🐛 9 | 🌐 Scala | 📅 2020-12-10 - HTML/XML parsing, manipulation and rendering.
* [scala-json](https://github.com/MediaMath/scala-json) ⭐ 62 | 🐛 7 | 🌐 Scala | 📅 2022-01-17 - JSON parser.
* [toml-scala](https://github.com/sparsetech/toml-scala) ⚠️ Archived - [TOML](https://github.com/toml-lang/toml) ⭐ 20,341 | 🐛 14 | 📅 2025-12-24 parser with codec derivation.
* [msgpack4z](https://github.com/msgpack4z/msgpack4z-native) ⭐ 5 | 🐛 1 | 🌐 Scala | 📅 2026-02-04 - Implementation of [MessagePack](https://msgpack.org/), a binary serialisation format.
* [squiggly](https://github.com/edadma/squiggly) ⭐ 2 | 🐛 0 | 🌐 Scala | 📅 2023-06-22 - Cross-platform template language for Scala, inspired by Liquid and Hugo templates.

## Databases

* [skunk](https://github.com/typelevel/skunk) ⭐ 1,640 | 🐛 88 | 🌐 Scala | 📅 2026-02-04 -  A data access library for Scala + Postgres.
* [SQLite4S](https://github.com/david-bouyssie/sqlite4s) ⭐ 38 | 🐛 3 | 🌐 Scala | 📅 2024-06-05 - Port of the Java library [Sqlite4java](https://bitbucket.org/almworks/sqlite4java). Includes bindings for the SQLite native library.
* [scala-native-jdbc](https://github.com/lolgab/scala-native-jdbc) ⭐ 12 | 🐛 1 | 🌐 Scala | 📅 2025-06-23 - Port of the database access layer [JDBC](https://en.wikipedia.org/wiki/Java_Database_Connectivity) to Scala Native.
* [libpq4s](https://github.com/david-bouyssie/libpq4s) ⭐ 4 | 🐛 0 | 🌐 Scala | 📅 2021-10-26 - Scala wrapper around the async PostgreSQL C library libpq.

## Web Development

* [sttp](https://github.com/softwaremill/sttp) ⭐ 1,495 | 🐛 30 | 🌐 Scala | 📅 2026-02-08 - HTTP Client library.
* [snunit](https://github.com/lolgab/snunit) ⭐ 147 | 🐛 8 | 🌐 Scala | 📅 2026-02-05 - Scala Native HTTP server based on NGINX Unit.
* [Trail](https://github.com/sparsetech/trail) ⭐ 82 | 🐛 1 | 🌐 Scala | 📅 2022-05-04 - Routing library.

## Concurrency

* [castor](https://github.com/com-lihaoyi/castor) ⭐ 146 | 🐛 20 | 🌐 Scala | 📅 2024-10-24 - Lightweight, typed Actor library for Scala.
* [scala-native-loop](https://github.com/scala-native/scala-native-loop) ⭐ 56 | 🐛 4 | 🌐 Scala | 📅 2024-06-18 - Event loop and async-oriented IO for Scala Native

## Logging

* [scribe](https://github.com/outr/scribe) ⭐ 544 | 🐛 24 | 🌐 Scala | 📅 2026-02-05 - Fast and simple logging library.
* [slogging](https://github.com/jokade/slogging) ⭐ 51 | 🐛 13 | 🌐 Scala | 📅 2020-09-17 - [Typesafe-logging](https://github.com/lightbend/scala-logging) ⭐ 925 | 🐛 29 | 🌐 Scala | 📅 2026-01-30 and [SLF4J](https://www.slf4j.org/)-compatible logging library based on macros.

## Console

* [scopt](https://github.com/scopt/scopt) ⭐ 1,446 | 🐛 59 | 🌐 Scala | 📅 2025-09-06 - Command-line argument parser.
* [scallop](https://github.com/scallop/scallop) ⭐ 682 | 🐛 8 | 🌐 Scala | 📅 2025-11-30 - A simple Scala CLI parsing library.
* [decline](https://github.com/bkirwi/decline) ⭐ 669 | 🐛 24 | 🌐 Scala | 📅 2026-02-07 - A composable command-line parser for Scala.
* [fansi](https://github.com/com-lihaoyi/fansi) ⭐ 232 | 🐛 21 | 🌐 Scala | 📅 2025-10-15 - Library for creating [ANSI-coloured strings](https://en.wikipedia.org/wiki/ANSI_escape_code).
* [mainargs](https://github.com/com-lihaoyi/mainargs) ⭐ 205 | 🐛 36 | 🌐 Scala | 📅 2026-01-14 - Small, dependency-free library for command line argument parsing in Scala.
* [scala-optparse-applicative](https://github.com/xuwei-k/optparse-applicative) ⭐ 16 | 🐛 1 | 🌐 Scala | 📅 2026-02-04 - Port of Haskell's CLI argument parsing library [optparse-applicative](https://hackage.haskell.org/package/optparse-applicative).

## Robotics

* [Potassium](https://github.com/Team846/potassium) ⭐ 18 | 🐛 10 | 🌐 Scala | 📅 2018-04-27 - Framework for writing robot software.
* [WPILib](https://github.com/Team846/scala-native-wpilib) ⭐ 7 | 🐛 0 | 🌐 Scala | 📅 2018-03-28 - Reimplementation of the [FIRST Robotics WPILib libraries](http://first.wpi.edu/FRC/roborio/release/docs/java/).

## Programs

* [Coursier](https://github.com/coursier/coursier) ⭐ 2,110 | 🐛 461 | 🌐 Scala | 📅 2026-01-21 - Coursier's [`bootstrap` command](https://get-coursier.io/docs/cli-native-bootstrap) generates native launchers.
* [sglgears](https://github.com/Milyardo/sglgears) ⭐ 15 | 🐛 1 | 🌐 Scala | 📅 2018-09-26 - Port of GL [gears.c](https://github.com/JoakimSoderberg/mesademos/blob/master/src/xdemos/glxgears.c) ⭐ 15 | 🐛 0 | 🌐 C | 📅 2012-12-20.
* [fractals](https://github.com/Rusty-Bike/fractals) ⭐ 7 | 🐛 0 | 🌐 Scala | 📅 2020-10-27 - A self-similar fractal generator with basic animation support.
* [k8s-cli](https://github.com/fsat/k8s-cli) ⭐ 3 | 🐛 1 | 🌐 Scala | 📅 2017-09-15 - CLI tools to generate [Kubernetes](https://kubernetes.io/) resources for [Akka](https://akka.io/), [Play Framework](https://www.playframework.com/) and [Lagom](https://www.lagomframework.com/)-based applications.

## Infrastructure

* [Seed Docker image](https://hub.docker.com/r/tindzk/seed/tags) - Docker image for cross-platform builds with [Seed](https://github.com/tindzk/seed) ⭐ 238 | 🐛 24 | 🌐 Scala | 📅 2020-12-11.
* [scala-native-sbt-docker](https://github.com/ScalaWilliam/scala-native-sbt-docker) ⭐ 4 | 🐛 0 | 📅 2017-03-16 - Docker image for Scala Native and sbt.

## Licence

<a rel="licence" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by.svg" /></a><br />This work is licenced under a <a rel="licence" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International Licence</a>.
