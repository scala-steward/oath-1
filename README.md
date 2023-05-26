[![Build status](https://img.shields.io/github/workflow/status/scala-jwt/oath/Continuous%20Integration.svg)](https://github.com/scala-jwt/oath/actions)
[![CI Status](https://github.com/scala-jwt/oath/actions/workflows/ci.yml/badge.svg)](https://github.com/scala-jwt/oath/actions/workflows/ci.yml)
[![Coverage status](https://img.shields.io/codecov/c/github/scala-jwt/oath/master.svg)](https://codecov.io/github/scala-jwt/oath)
[![Maven Central](https://img.shields.io/maven-central/v/io.github.scala-jwt/jwt-core_2.13.svg)](https://central.sonatype.dev/artifact/io.github.scala-jwt/jwt-core_2.13/0.0.6)

## Scala JWT - OATH

__OATH__ provides an easy way for Rest API Applications to manipulate JWTs in complex systems.
1. Customize registered claims via configuration. 
1. Create a variety of JWT tokens with different configuration for each use case
1. Token encryption.

### Modules

* [JWT Docs](./jwt/README.md) - A Scala API of [java-jwt](https://github.com/auth0/java-jwt)
* [Juror Docs](./juror/README.md) - Extension of JWT to manipulate different type of tokens

### SBT Dependencies

* [jwt-core](https://mvnrepository.com/artifact/io.github.scala-jwt/jwt-core)
* [juror-core](https://mvnrepository.com/artifact/io.github.scala-jwt/juror)

```scala
val jwtCore = "io.github.scala-jwt"  %% "jwt-core"  % "0.0.0"
val juror   = "io.github.scala-jwt"  %% "juror"     % "0.0.0"
```

### Json Converters

* [jwt-circe](https://mvnrepository.com/artifact/io.github.scala-jwt/jwt-circe)

```scala
val jwtCirce = "io.github.scala-jwt" %% "jwt-circe" % "0.0.0"
```

* [jwt-jsoniter-scala](https://mvnrepository.com/artifact/io.github.scala-jwt/jwt-jsoniter-scala)

```scala
val jwtJsoniterScala = "io.github.scala-jwt" %% "jwt-jsoniter-scala" % "0.0.0"
```

### Known Issues
 * Audience single empty string in the list might lead to unexpected behaviours raised in [java-jwt#662](https://github.com/auth0/java-jwt/issues/662) 