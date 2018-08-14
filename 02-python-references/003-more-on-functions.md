## Python References

* Recursion
* Fibonacci with recursion

&nbsp;
&nbsp;
&nbsp;

### Recursion

```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)
        
print(factorial(6))
```

The recursive algorithm breaks the problem down into smaller problems and refers to itself, or calls itself from within each time its iterating. To quite from  "This function does not use any explicit loops. Repetition is provided by the repeated recursive invocations of the function. There is no circularity in this defini- tion, because each time the function is invoked, its argument is smaller by one, and when a base case is reached, no further recursive calls are made."
