# partial-lambdas

[![Build Status](https://travis-ci.org/velo/partial-lambdas.svg?branch=master)](https://travis-ci.org/velo/partial-lambdas?branch=master)
[![Coverage Status](https://coveralls.io/repos/github/velo/partial-lambdas/badge.svg?branch=master)](https://coveralls.io/github/velo/partial-lambdas?branch=master)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.marvinformatics/partial-lambdas/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.marvinformatics/partial-lambdas/)
[![Issues](https://img.shields.io/github/issues/velo/partial-lambdas.svg)](https://github.com/velo/partial-lambdas/issues)
[![Forks](https://img.shields.io/github/forks/velo/partial-lambdas.svg)](https://github.com/velo/partial-lambdas/network)
[![Stars](https://img.shields.io/github/stars/velo/partial-lambdas.svg)](https://github.com/velo/partial-lambdas/stargazers)

This is a java implementation for python `functools.partial`.  But what `functools.partial` does? `functools.partial` transformes one function into a new function with one or more arguments already filled.

```java
BiFunction<Integer, Integer, Integer>  multiplication = (multiplicand, multiplier) -> multiplicand * multiplier;
Function<Integer, Integer>  timesTwo = partial(multiplication, 2);
Integer result = timesTwo(4); // 8
```



