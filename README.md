# <a href="https://retest.dev"><img src="https://assets.retest.org/retest/ci/logos/recheck-screen.svg" width="300"/></a>

[![Build Status](https://travis-ci.com/retest/recheck-junit-jupiter-extension.svg?branch=master)](https://travis-ci.com/retest/recheck-junit-jupiter-extension)
[![Latest recheck-junit-jupiter-extension on Maven Central](https://maven-badges.herokuapp.com/maven-central/de.retest/recheck-junit-jupiter-extension/badge.svg?style=flat)](https://mvnrepository.com/artifact/de.retest/recheck-junit-jupiter-extension)
[![license](https://img.shields.io/badge/license-AGPL-brightgreen.svg)](https://github.com/retest/recheck-junit-jupiter-extension/blob/master/LICENSE)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg)](https://github.com/retest/recheck-junit-jupiter-extension/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
[![code with hearth by retest](https://img.shields.io/badge/%3C%2F%3E%20with%20%E2%99%A5%20by-retest-C1D82F.svg)](https://retest.de/)

JUnit Extension for [recheck](https://github.com/retest/recheck). Automatic set up and tear down of tests using recheck.

## Features

* Calls `startTest` on all `RecheckLifecycle` objects before each test.
* Calls `capTest` on all `RecheckLifecycle` objects after each test.
* Calls `cap` on all `RecheckLifecycle` objects after all tests.

## Advantages

The extension automatically calls `startTest`, `capTest` and `cap`. So it is no longer required to call those methods manually. This reduces boilerplate code and ensures the lifecycle within a test using recheck.

## Usage

Recheck JUnit extension uses JUnit's extension mechanism. It can be used by adding `@ExtendWith(RecheckExtension.class)` to your test class.

### Prerequisites

Requires at least JUnit Jupiter. For JUnit 4 support look at [recheck extension for JUnit 4](https://github.com/retest/recheck-junit-4-extension).

## License

This project is licensed under the [AGPL license](LICENSE).
