# Python

## Repository

<https://github.com/graalvm/graalpython>

## Installation

Python support comes built in with Graal.

## Runs on Graal

:ballot_box_with_check: Yes

```shell
graalpython hello-world.py
```

## Supports Polyglot

:ballot_box_with_check: Yes

Example integration with Java

```python
import java
array = java.type("int[]")(4)
array[2] = 42
print(array[2])
```

```shell
graalpython --polyglot --jvm polyglot.py
```

## Sources and Resources

- <https://www.graalvm.org/docs/reference-manual/languages/python>

[graal updater]: https://www.graalvm.org/docs/reference-manual/graal-updater
