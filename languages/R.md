# R

## Repository

<https://github.com/oracle/fastr>

## Installation

R language is included in [Graal updater][].

```shell
gu install R
```

## Runs on Graal

:ballot_box_with_check: Yes

```shell
Rscript hello-world.r
```

## Supports Polyglot

:ballot_box_with_check: Yes

Example integration with Java

```R
array <- new("int[]", 4)
array[3L] <- 42
print(array[3L])
```

```shell
Rscript --jvm --polyglot polyglot.R
```

## Additional Resources

- <https://www.graalvm.org/docs/reference-manual/languages/r>

[graal updater]: https://www.graalvm.org/docs/reference-manual/graal-updater
