# JavaScript

## Repository

<https://github.com/graalvm/graaljs>

## Installation

JavaScript support comes built in with Graal.

## Runs on Graal

:ballot_box_with_check: Yes

```shell
js hello-world.js
```

## Supports Polyglot

:ballot_box_with_check: Yes

Example integration with Java

```javascript
const array = new (Java.type("int[]"))(4);
array[2] = 42;
console.log(array[2]);
```

```shell
js --jvm --polyglot polyglot.js
```

## Sources and Resources

- <https://www.graalvm.org/docs/reference-manual/languages/js>
- <https://www.graalvm.org/docs/reference-manual/polyglot>
