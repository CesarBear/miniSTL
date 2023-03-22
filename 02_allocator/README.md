
# Allocator

## Standard API  

- `allocator::value_type`
- `allocator::pointer`
- `allocator::const_pointer`
- `allocator::reference`
- `allocator::cons_reference`
- `allocator::size_type`
- `allocator::difference_type`
- `allocator::rebind`
- `allocator::allocator()`
  > default constructor
- `allocator::allocator(const allocator&)`
  > copy constructor
- `template <typename U> allocator::allocator(const allocator<U>&)`
  > generic copy constructor
- `allocator::~allocator()`
  > default deconstructor
- `pointer allocator::address(reference x) const`
  > return the address of an object
- `const_pointer allocator::address(const_reference x) const`
  > return the address of a const object
- `pointer allocator::allocate(size_type n, const void* = 0)`
  > configure the memory, so that it can contain n number of T
- `void allocator::deallocate(pointer p, size_type n)`
  > give back the memory
- `size_type allocator::max_size() const`
  > return the maximum of allocatable memory
- `void allocator::construct(pointer p, const T& x)`
- `void allocator::destroy(pointer p)`
