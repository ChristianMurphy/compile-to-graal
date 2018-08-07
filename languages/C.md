# C

## Repository

<https://github.com/graalvm/sulong>

## Installation

C support comes built in with Graal.

## Runs on Graal

:ballot_box_with_check: Yes

```shell
clang -g -O1 -c -emit-llvm -I$GRAALVM_HOME/jre/languages/llvm hello-world.c
lli hello-world.bc
```

## Supports Polyglot

:ballot_box_with_check: Yes

Example integration with Java

```java
#include <stdio.h>
#include <polyglot.h>

int main() {
    void *arrayType = polyglot_java_type("int[]");
    void *array = polyglot_new_instance(arrayType, 4);
    polyglot_set_array_element(array, 2, 42);
    int element = polyglot_as_i32(polyglot_get_array_element(array, 2));
    printf("%d\n", element);
    return element;
}
```

```shell
clang -g -O1 -c -emit-llvm -I$GRAALVM_HOME/jre/languages/llvm polyglot.c
lli --polyglot --jvm polyglot.bc
```
