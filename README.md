# blocking-queues

General-purpose Java blocking queues for applications that need dynamic capacity management or graceful draining shutdown.

## Coordinates

```xml
<dependency>
    <groupId>io.github.monadrome</groupId>
    <artifactId>blocking-queues</artifactId>
    <version>0.5.0-SNAPSHOT</version>
</dependency>
```

当前开发线版本为 `0.5.0-SNAPSHOT`；`0.5.0` 需要等首次正式发布后再使用。

## API

- `ResizableBlockingQueue` provides a bounded FIFO queue whose capacity can be changed at runtime.
- `DrainingBlockingQueue` closes production permanently while consumers drain every accepted element before observing the configured terminal signal.

Both classes are Java 8 compatible and live in `io.github.monadrome.queues`.
