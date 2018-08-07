# Java

## Repository

<https://github.com/oracle/graal>

## Installation

Java support comes built in with Graal.

## Runs on Graal

:ballot_box_with_check: Yes

```shell
javac HelloWorld.java
java HelloWorld
```

## Supports Polyglot

:ballot_box_with_check: Yes

Example integration with JavaScript

```java
import org.graalvm.polyglot.*;

class Polyglot {
    public static void main(String[] args) {
        Context polyglot = Context.create();
        Value array = polyglot.eval("js", "[1,2,42,4]");
        int result = array.getArrayElement(2).asInt();
        System.out.println(result);
    }
}
```

```shell
javac Polyglot.java
java Polyglot
```

## Sources and Resources

- <https://www.graalvm.org/docs/reference-manual/languages/jvm>
- <https://www.graalvm.org/docs/reference-manual/polyglot>
