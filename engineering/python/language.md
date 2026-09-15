# Python language concepts: basic, intermediate, and advanced

These levels are approximate. 

## Concepts by level

| Area | Basic | Intermediate | Advanced |
|---|---|---|---|
| Syntax and control flow | Variables, indentation, `if`, `for`, `while`, `break`, `continue` | Unpacking, comprehensions, assignment expressions, structural pattern matching | Understanding evaluation order and tricky scoping behavior |
| Built-in types | `int`, `float`, `bool`, `str`, `None` | `bytes`, `bytearray`, numeric precision, choosing appropriate representations | Buffer protocol, `memoryview`, custom numeric behavior |
| Collections | Lists, dictionaries, sets, tuples; indexing and slicing | `deque`, `Counter`, `defaultdict`, `OrderedDict`; operation complexity | Designing custom containers; hash/equality invariants |
| Objects and mutability | Mutable versus immutable; `==` versus `is` | Aliasing, shallow/deep copies, mutable default arguments, hashability | Object lifetime, weak references, garbage collection, finalization |
| Functions | Parameters, return values, defaults | `*args`, `**kwargs`, keyword-only arguments, closures, scope, functions as values | Function introspection, signatures |
| Decorators | Recognize `@decorator` syntax; use supplied decorators such as `@property` and `@staticmethod` | Understand function wrapping and `f = decorator(f)`; write wrappers with `*args`, `**kwargs`, and `functools.wraps`; understand application order | Parameterized and class-based decorators; preserve typing with `ParamSpec`; handle async functions, generators, descriptors, and stacked decorators |
| Iteration | Looping and `range`, `enumerate`, `zip` | Iterables versus iterators, generator expressions, `yield`, `itertools` | Generator protocols, `yield from`, asynchronous iteration |
| Classes | Instances, attributes, methods, `__init__` | Inheritance, composition, properties, dataclasses, class/static methods | Descriptors, method resolution order, metaclasses, `__slots__` |
| Python data model | Basic use of built-in objects | Implementing `__repr__`, `__eq__`, `__hash__`, `__iter__`, `__len__` | Attribute lookup, operator dispatch, designing coherent object protocols |
| Exceptions | `try`, `except`, `raise` | `else`, `finally`, custom exceptions, exception chaining, narrow handling | Exception safety during partial updates; exception groups |
| Context managers | Using `with` for files | `__enter__`/`__exit__`, `@contextmanager`, guaranteed cleanup | `ExitStack`, async context managers, coordinating multiple resources |
| Modules and dependencies | Imports, scripts, `pip`, virtual environments | Packages, relative imports, `__main__`, `pyproject.toml` | Import machinery, dependency resolution, packaging and distribution |
| Files and data | Reading/writing text, JSON, paths | `pathlib`, CSV, binary files, encodings, streaming large files | Memory-mapped files, serialization tradeoffs, durable/atomic file updates |
| Type hints | Parameter and return annotations | Unions, generics, `TypeVar`, `Protocol`, `TypedDict`, static checking | Variance, `ParamSpec`, overloads, designing typed library interfaces |
| Testing and debugging | Assertions, basic unit tests, tracebacks | Fixtures, mocks, parametrization, logging, debugger usage | Property-based testing, deterministic concurrency tests, failure injection |
| Threading | Knowing threads share memory | `Thread`, `Lock`, `RLock`, queues, thread pools | Conditions, semaphores, deadlocks, starvation, lock ordering, linearizability |
| Async programming | Recognizing `async`/`await` | Coroutines, tasks, event loops, async I/O | Cancellation, structured concurrency, backpressure, blocking-call isolation |
| Multiprocessing | Knowing processes have separate memory | Process pools, pickling, choosing threads versus processes | Shared memory, process start methods, IPC and lifecycle management |
| Performance | Big-O basics; avoiding obvious repeated work | Profiling, benchmarking, caching, memory measurement | Interpreter overhead, allocation behavior, native extensions, workload-specific optimization |
| Runtime internals | Knowing Python executes through an interpreter | References, garbage collection basics, CPython/GIL implications | Bytecode, reference counting details, free-threaded execution, C extension constraints |

## Priorities for backend work

Focus on these intermediate skills:

- Choose collections and know their time complexity.
- Reason about references, mutation, equality, and hashing.
- Write small classes and clear function interfaces.
- Use exceptions and `try/finally` correctly.
- Understand generators and context managers.
- Protect shared state with standard locks.
- Write focused tests, including edge cases and failures.
- Use basic type hints, logging, and profiling.

