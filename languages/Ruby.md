# Ruby

## Repository

<https://github.com/oracle/truffleruby>

## Installation

Ruby language is included in [Graal updater][].

```shell
gu install ruby
```

## Runs on Graal

:ballot_box_with_check: Yes

```shell
ruby hello-world.rb
```

## Supports Polyglot

:ballot_box_with_check: Yes

Example integration with Java

```ruby
array = Java.type('int[]').new(4)
array[2] = 42
print(array[2])
```

```shell
ruby --polyglot --jvm polyglot.rb
```

## Sources and Resources

- <https://www.graalvm.org/docs/reference-manual/languages/ruby>

[graal updater]: https://www.graalvm.org/docs/reference-manual/graal-updater
