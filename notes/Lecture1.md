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
