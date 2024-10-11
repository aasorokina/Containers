# Containers
Implementation of basic standard C++ container classes

## Project description

Implemented the `s21_containers.h` library basic classes:\
`list`, `map`, `queue`, `set`, `stack`, `vector`.

Implemented the `s21_containersplus.h` library additional classes:\
`array`, `multiset`.

Implemented additional `insert_many` method, according to the table:

| Modifiers      | Definition                                      | Containers |
|----------------|-------------------------------------------------| -------------------------------------------|
| `iterator insert_many(const_iterator pos, Args&&... args)`          | Inserts new elements into the container directly before `pos`.  | List, Vector. |
| `void insert_many_back(Args&&... args)`          | Appends new elements to the end of the container.  | List, Vector, Queue, Stack. |
| `void insert_many_front(Args&&... args)`          | Appends new elements to the top of the container.  | List. |
| `vector<std::pair<iterator,bool>> insert_many(Args&&... args)`          | Inserts new elements into the container.  | Map, Set, Multiset. |

## Building project

Program library code located in the `src/lib` folder.

Makefile targets: 

`all` - builds the project and launches tests;\
`clean` - removes the object files;\
`test` - runs tests;\
`gcov_report` - generates coverage report;