# Pitfalls

## numpy

### Variable overridden due to using the same name

```python
import numpy as np
d = np.arange(16).reshape(4,4)
x = np.array([x[:2] for x in d])
y = np.array([x[2:] for x in d])
```

The intention here is to assign the first two columns to `x`, and the last two
columns to `y`. The problem is `x` will be overridden in the last line!

Fix: Change the `x` in list comprehension to some other name, e.g. `v`.

Better code:

```python
x = d[:, :2]
y = d[:, 2:]
```
Note: This new code is slightly different from the earlier example, in that here `x` is a "reference" to the underlying data of `d`, which means modifying `x` will also modify `d`.

Takeaway:
- Be wary of potential variable name duplication
- It's worthwhile to learn about numpy slicing
