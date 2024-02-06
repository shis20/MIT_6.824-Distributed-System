# Lecture 1 Introduction

 - Parallelism
 - fault tolerance 
 - Physical Reason
 - Security/ isolated 

## Challenges

 - Concurrency
 - Partial failure
 - Performance

----------------------------------------------------

## Infrastructure

 - Storage
 - Communication
 - Computation (MapReduce System)
   > abstract and hidden
## Abstractions

- Implementation
  > RPC, Threads, concurrencies
  >
## Performance

 - Scalabilities - 2X computers -> 2X throughput (the web server would not longer the bottle necy, the Database would be bottleneck instead) --- storage problem raised.

## Fault Tolerance

- Availability
- Recoverability
- (Non-volatile Memory - do not require a continuous power supply to retain data , etc. flash)
- Replication

-------------------------------------------------------------------------
## Consistencsy

  - Put(key, value)
  - Get(R) -> V 
  - More than one copy data, different versions/replications! 
  - Strong Consistency : may expensive to get the most recent put data (consult all copies)
  - Weak Consistency: allow stale read (go with it!, its ok :) )
----------------------------------------------------------------------------

 - Input 1 -> Map       a, 1     b, 1
 - Input 2 -> Map                b, 1
 - Input 3 -> Map       a, 1              c, 1
 -                       |        |         |
 -                    reduce     reduce   reduce
 -                     a, 2      b, 2       c, 1
