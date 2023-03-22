
# Basics  

## History  

## 6 Components  

1. `containers` : all kinds of data structure, such as vector, list, deque, set, map.  
2. `algorithms` : sort, search, copy, erase...  
3. `iterators` : generic pointer, with whose help people can apply algorithms to containers.  
4. `functors` : policy  
5. `adapters` : adapt the API of containers, functors or iterators.  
6. `allocators` : responsible for the space configuration and management.  

- With the help of `Allocator`, `Container` can access the memory for data. `Algorithm` can access the content of `Container` through `Iterator` and `Functor` can help the `Algorithm` to implement different policies. `Adapter` can customize the `Functor`.  
