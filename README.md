## Polynomial ADT (Linked List Implementation)

A C++ implementation of a polynomial mathematical structure using a sorted singly linked list with a dummy head node.

### Features
- **Ordered Term Insertion:** Automatically maintains terms in descending order of exponents ($d$).
- **Like Term Consolidation:** Combines coefficients when terms with identical degrees are pushed.
- **Zero-Coefficient Pruning:** Automatically removes terms whose coefficients cancel out to zero.
- **Evaluation:** Calculates $P(x)$ for any real value $x$ in $O(N)$ time complexity.

### Code Example
```cpp
Polinom p;
p.push(3.0, 2); // 3x^2
p.push(2.0, 1); // 2x
p.push(5.0, 0); // 5

// Evaluates 3(2)^2 + 2(2) + 5 = 21
double result = p.evaluate(2.0);
