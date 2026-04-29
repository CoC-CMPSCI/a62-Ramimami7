# A62: Random Numbers and Closest to Mean

**Code your program here:** [https://classroom.github.com/a/GXPSnEiA](https://classroom.github.com/a/GXPSnEiA)

---

## [Programming Assignment Guide]

**Read the Assignment Directions below, then complete the following `main.cpp` in your cloned Repository.**

**Assignment Directions:**

In this assignment, you will complete two functions in `main.hpp`. **Do NOT edit `main.cpp`** — it is already complete and calls your functions.

| Function 1: `int getRandom(void)` |
|---|
| • Returns a random integer between `0` and `99` (inclusive) <br>• Use `rand() % 100` to generate the value <br>• The random seed is set by `srand(time(0))` in `main.cpp` — do not call srand in your function |

| Function 2: `int getClosestMed(int num1, int num2, int num3)` |
|---|
| • Calculate the mean: `(num1 + num2 + num3) / 3.0` <br>• Return whichever of the three values is closest to the mean (smallest absolute difference) <br>• Example: `getClosestMed(1, 2, 3)` → mean is 2.0 → return `2` <br>• Example: `getClosestMed(1, 10, 11)` → mean is 7.33 → return `10` |

**To compile and run:**

```cpp
g++ main.cpp
./a.out
```

**To run tests:**

```cpp
make test
make test ARGS="[T1]"
```

**Starter Code (`main.cpp`):**

```cpp
#include <iomanip>
#include <iostream>
#include <cstdlib>
#include <ctime>
#include <cmath>
using namespace std;

int getRandom(void);
int getClosestMed(int, int, int);

int getRandom(void)
{
    // TODO
}

int getClosestMed(int rdnum1, int rdnum2, int rdnum3)
{
    // TODO
}
```

**How to compile and run your program:**

- To compile your program in VS Code, open the new terminal (ctrl-`) and type: `g++ main.cpp -o main`
- To run your program: `./main`

**How to test your program:**

- To run all tests: `make test`
- To run a specific test (e.g., T1): `make test ARGS="[T1]"`

**[Expected Output]**

*Your output should contain the correct values. The exact wording or formatting may differ — tests check values only, not the entire output.*

Example run (random seed from time):

```cpp
Random values 32	79	33
 Mean Value is 48
The closest value to mean is 33
```

**How to pass the test:**

Test items: **compile, run, T1, T2, T3, T4**

| Test | Input | Expected Values (checked by test) | Points |
|---|---|---|---|
| T1 | getRandom() called 10 times with srand(42) | all values in [0, 99] | 20 |
| T2 | getClosestMed(1, 2, 3), getClosestMed(10, 20, 30) | 2, 20 | 20 |
| T3 | getClosestMed(1, 10, 11), getClosestMed(1, 5, 9) | 10, 5 | 20 |
| T4 | getClosestMed(0, 50, 100), getClosestMed(0, 33, 99) | 50, 33 | 20 |

To test your program, type the command in your terminal: `make test`

**Make sure that your program passes the test and there is ✓ in your GitHub Classroom Repository.**

