Sometimes it's useful to look at world from the another view.


In linear algebra, the transpose of a matrix **A** is another matrix **A**<sup>T</sup>
(also written **A**′, **A**<sup>tr</sup>,<sup>t</sup>**A** or **A**<sup>t</sup>)
created by any one of the following equivalent actions:

- reflect **A** over its main diagonal (which runs from top-left to bottom-right) to obtain **A**<sup>T</sup>
- write the rows of **A** as the columns of **A**<sup>T</sup>
- write the columns of **A** as the rows of **A**<sup>T</sup>


Formally, the _i_ row, _j_ column element of
**A**<sup>T</sup> is the _j_ row, _i_ column element of
**A**:</p>

[**A**<sup>T</sup>]<sub>i j</sub> = [**A**]<sub>j i</sub>


If **A** is an _m_ × _n_ matrix then **A**<sup>T</sup> is an _n_ × _m_ matrix.

You have been given a matrix as a 2D list with integers.
Your task is to return a transposed matrix based on input.

![Matrix](transposed-matrix.png)

**Input:** A matrix as a list of lists with integers.

**Output:** The transposed matrix as a list of lists with integers.

**Example:**

```python
transpose([[1, 2, 3],
     [4, 5, 6],
     [7, 8, 9]]) == [[1, 4, 7],
                     [2, 5, 8],
                     [3, 6, 9]]
transpose([[1, 4, 3],
     [8, 2, 6],
     [7, 8, 3],
     [4, 9, 6],
     [7, 8, 1]]) == [[1, 8, 7, 4, 7],
                     [4, 2, 8, 9, 8],
                     [3, 6, 3, 6, 1]]
```

**How it is used:**

The most obvious use for this idea is in mathematical software,
but the concept can be applied in the area of vector graphics.
On a computer, one can often avoid explicitly transposing a matrix in memory by simply accessing the same data in a different order.

**Precondition:**
```python
0 < len(matrix) < 10
all(0 < len(row) < 10 for row in matrix)
```
