# collatzzz

A Simple Collatz (bench) program.
Benching sum of (given) collatz steps.
And more ...

## Versions

- v0.1: 1 CPU only
- v0.2: Multiple CPUs. Accepts input too
- v0.3: More commands. Bug fixes

## Source code

Maybe later ...

## Example: help

```
> ./collatzzz --help

==============================
A Simple Collatz (bench) program
--help         This help
... [N]        Show sum 0 -> N:th
-cores [N]     Set cores
-hash [MB]     Set hash in MB
-list [A] [B]  Show list A -> B
-sum [A] [B]   Show sum A -> B
-nth [N]       Show N:th Collatz steps
```

## Example: nth

```
> ./collatzzz -nth 424242424242

... Nth ...
==============================
Nth:        354
CPU(s):     16
Hash(MB):   0
SPS:        0
Time(ms):   0
```

## Example: list

```
> ./collatzzz -list 2 7

2: 1
3: 7
4: 2
5: 5
6: 8
7: 16
```

## Example: sum 1B

```
> ./collatzzz -sum 0 1000000000

... Sum ...
==============================
Collatz:    0 -> 1,000,000,000
Sum(steps): 203,234,783,374
CPU(s):     16
NPS:        8,867,910,000
Time(ms):   22,918
```

## Example: bench

```
> ./collatzzz

... Bench ...
==============================
Collatz:    0 -> 100,000,000
Sum(steps): 17,923,493,583
CPU(s):     16
Hash(MB):   0
SPS:        5,588,866,100
Time(ms):   3,207
```
