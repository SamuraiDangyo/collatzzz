# collatzzz

A Simple Collatz (bench) program.
Benching sum of (given) Collatz steps.
And more ...

## Problem

```
x         = {1, inf}
x (odd)  -> 3 * x + 1
x (even) -> x / 2
0        -> 1 (special)
```

## Theory

Collatz conjecture assumes that:
Every number collapses to eternal 1 -> 4 -> 2 -> 1 loop.
Not mathematically proven yet.

## Versions

- v0.1: 1 CPU only
- v0.2: Multiple CPUs. Accepts input too
- v0.3: More commands. Bug fixes
- v0.4: Cosmetic improvements
- v0.5: More cosmetic improvements

## Source code

Maybe later ...

## Scaling

![Scaling](https://raw.githubusercontent.com/SamuraiDangyo/collatzzz/main/10M-0MB-1-16CPU.png)

## Example: Bench

```
> ./collatzzz
```

```
...
Collatz:    0 -> 100,000,000
Sum(steps): 17,923,493,583
CPU(s):     16
Hash(MB):   0
SPS:        5,516,618,523
Time(ms):   3,249
```

## Example: Nth

```
> ./collatzzz -nth 42
```

```
...
Nth:        42
Result:     8
CPU(s):     3
Hash(MB):   0
SPS:        0
Time(ms):   0
```

## Example: List

```
> ./collatzzz -list 35 42
```

```
35: 13
36: 21
37: 21
38: 21
39: 34
40: 8
41: 109
42: 8
```

## Example: Sum

```
> ./collatzzz -sum 0 1000000000
```

```
...
Collatz:    0 -> 1,000,000,000
Sum(steps): 203,234,783,374
CPU(s):     16
Hash(MB):   0
SPS:        8,338,521,453
Time(ms):   24,373
```

## Example: Help

```
> ./collatzzz --help
```

```
A Simple Collatz (bench) program
--help         This help
--version      Show version
... [N]        Show sum 0 -> N
-cores [N]     Set cores
-hash [MB]     Set hash in MB
-list [A] [B]  Show list A -> B
-sum [A] [B]   Show sum A -> B
-nth [N]       Show N:th Collatz steps
```
