# dirbean
No-fuss Web Path Discovery tool.
Simple yet effective with built-in WAF evasion techniques.

## Basic Usage
```
Dirbean v.03- @iamfriedbean
No-fuss Web Path Discovery tool

   -w     Path to wordlist file
   -c     Concurreny level  (default:10)
   -r     Number of request per second. Default is 100 (e.g. -r 120)
   -c     Concurrency level  (default:10)
   -t     Request timeout in seconds (default: 10)
   -m     HTTP method to use (HEAD or GET , default: HEAD)
   -p     Optional URL proxy
   -v     Verbose Output Level (1: low, 2: medium, 3: high)
   -s     Response status codes to match (default: 200,403,401,302,201,202,204)
   -H     Custom headers (Format: Header1:Value1,Header2:Value2)

Examples:
   cat domains.txt | dirbean -w ~/wordlist/common.txt
   echo 'http://example.com' | dirbean -w ~/wordlist/common.txt -c 10 -v 2

```
## Installation

Part of Beanscan Suite of tools. See beanscan repository.

## Parallelism
Number of concurrency can be set using the -c flag. It uses 25 threads by default.
Recommend lowering the concurrency if time is not an issue.

```
cat domains.txt | dirbean -w ~/wordlist/common.txt -c 10
```
## Important Note
As with any path discovery tool, this requires a good wordlist.
