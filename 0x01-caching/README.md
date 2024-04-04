0x01-caching
1. Least Recently Used (LRU):

    LRU replacement policy evicts the least recently accessed items from the cache when it reaches its capacity limit.
    This policy assumes that items that have not been accessed for a longer time are less likely to be accessed in the near future.
    LRU is widely used due to its simplicity and effectiveness in capturing temporal locality.

2. Least Frequently Used (LFU):

    LFU replacement policy evicts the least frequently accessed items from the cache when it reaches its capacity limit.
    This policy prioritizes items that are accessed more frequently, assuming that frequently accessed items are more likely to be accessed again in the future.
    LFU can be beneficial for workloads with skewed access patterns where a few items are accessed significantly more frequently than others.

3. First-In-First-Out (FIFO):

    FIFO replacement policy evicts the oldest items that were inserted into the cache when it reaches its capacity limit.
    This policy operates on a simple queue-based approach, where the first item inserted into the cache is the first one to be evicted when space is needed.
    FIFO is straightforward to implement but may not always capture access patterns effectively, especially in scenarios where older items are still frequently accessed.

Other Replacement Policies:

    Besides LRU, LFU, and FIFO, there are other cache replacement policies designed to address specific characteristics of different workloads.
    Adaptive replacement policies dynamically adjust eviction decisions based on access patterns and cache contents. Examples include ARC (Adaptive Replacement Cache) and CLOCK-Pro.
    Random replacement policies randomly select items for eviction, which can sometimes provide simple and efficient cache management without relying on explicit access patterns.