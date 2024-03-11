# dirbean
No-fuss Web Path Discovery tool.
Simple yet effective with built-in WAF evasion techniques.

## Basic Usage
```
cat domains.txt | dirbean -w ~/wordlist/common.txt
   -w     Path to wordlist file
   -c     Concurreny level  (default:25)
```
## Installation

Part of Beanscan Suite of tools. See beanscan repository.

## Parallelism
Number of concurrency can be set using the -c flag. It uses 25 threads by default.

```
cat domains.txt | dirbean -w ~/wordlist/common.txt -c 10
```
## Important Note
As with any path discovery tool, this requires a good wordlist.
