# NumPy

<p>NumPy (Numerical Python) is one of the most important libraries in the python ecosystem for scientific computing.<br>It provides fast, efficient tools for working with numerical data.</p>

<h2>NumPy is used for:</h2>
<ul>
    <li>Performing numerical computations</li>
    <li>Working with large, multi-dimensional arrays and matrices</li>
    <li>Mathematical operations (linear algebra, statistics, Fourier transforms, etc)</li>
    <li>High performance data processing</li>
</ul>

<p>As its core is the ndarray (N - dimensional array), which is much faster and more money efficient than python's built-in lists.</p>
<p>Ex:-</p>
<pre>
import numpy as np
arr = np.array([1,2,3,4,5])
print(arr*2)
</pre>

<h2>Who created and when?</h2>
<p>NumPy was created by <u>Travis Oliphant</u> in 2005.</p>
<p>Combining features of libraries like:</p>
<ul>
    <li>Numeric</li>
    <li>Numarray</li>
</ul>

<h2>Why Important?</h2>
<p>NumPy is foundational for many other libraries:</p>
<ul>
    <li>Pandas</li>
    <li>SciPy</li>
    <li>MatPlotLib</li>
    <li>Tensorflow</li>
    <li>PyTorch</li>
</ul>
<p>Without NumPy, most modern data science and machine learning workflows in python wouldn't exist.</p>

<h2>Installation of NumPy</h2>
<h3><li>Standard Installation - (Most Common) :</li></h3>
<p>Open command prompt/ terminal and run.<p>
<pre>
pip install numpy
</pre>
<h3><li>For Anaconda - (For data science) :</li></h3>
<p>NumPy usually comes preinstalled, but if needed</p>
<pre>
conda install numpy
</pre>
<h3><li>For Jupyter Notebook :</li></h3>
<pre>
!pip install numpy
</pre>
<h3><li>Verify installation :</li></h3>
<pre>
import numpy as np
print(np._version_)
</pre>

<h2>NumPy Array vs Python list</h2>
<h3><li>Performance (speed) :</li></h3>
<table>
    <tr>
        <th>NumPy arrays</th>
        <th>Python lists</th>
    </tr>
    <tr>
        <td>Much faster</td>
        <td>Slower for math operations</td>
    </tr>
    <tr>
        <td>Optimized for numerical computation</td>
        <td>Not optimized for large numerical data</td>
    </tr>
    <tr>
        <td>Implemented in C internally</td>
    </tr>
    <tr>
        <td>Ex:
            <pre>
import numpy as np
arr = np.array([1,2,3,4])
print(arr*2)
            </pre>
        </td>
        <td>Ex:
            <pre>
list = [1,2,3,4]
result = [x * r for x in list]
print(result)
            </pre>
        </td>
    </tr>
</table>
<h3><li>Memory Efficiency :</li></h3>
<table>
    <tr>
        <th>NumPy arrays</th>
        <th>Python lists</th>
    </tr>
    <tr>
        <td>Store elements in contiguous memory</td>
        <td>Store references to objects</td>
    </tr>
    <tr>
        <td>Same data type -> less memory</td>
        <td>More memory usage</td>
    </tr>
    <tr>
        <td>Stores raw values -> efficient</td>
        <td>Stores pointers -> More overhead</td>
    </tr>
    <tr>
        <td>Ex:- 
            <pre>
[1 2 3]
            </pre>
        </td>
        <td>Ex:-
            <pre>
[1,2,3]
            </pre>
        </td>
    </tr>
</table>
<h3><li>Data type Handling :</li></h3>
<table>
    <tr>
        <th>NumPy arrays</th>
        <th>Python lists</th>
    </tr>
    <tr>
        <td>Same data type only</td>
        <td>Can store mixed types</td>
    </tr>
    <tr>
        <td>Ensures speed and efficiency</td>
        <td>Flexible but inefficient for math</td>
    </tr>
    <tr>
        <td>Ex:-
            <pre>
arr = np.array([1,2,3])
print(arr.dtype)
            </pre>
        </td>
        <td>Ex:-
            <pre>
list = [1,'hello',3.3]
print(list)
            </pre>
        </td>
    </tr>
</table>
<h3><li>Multi-Dimensional Support :</li></h3>
<table>
    <tr>
        <th>NumPy array</th>
        <th>Python lists</th>
    </tr>
    <tr>
        <td>-> Matrix operations<br>
        -> Linear algebra<br>
        -> Broad casting</td>
        <td>-> Limited operations</td>
    </tr>
    <tr>
        <td>Built for this-
            <pre>
arr = np.array([[1,2],
                [3,4]])
            </pre>
        </td>
        <td>Possible by messy-
            <pre>
list = [[1,2],[3,4]]
            </pre>
        </td>
    </tr>
</table>

<h3>When to use what?</h3>
<li>Use python list for General programming.</li> 
<li>Use NumPy for Numerical Computing/ Ml/ Data Science</li>

<h2>Creating Arrays</h2>
<p>An array is a collection of elements of the same data type stored in contiguous memory locations.</p>
<ul>
    <li>Array can by one-dimensional, two-dimensional, or multi-dimensional</li>
    <li>NumPy arrays are more efficient than list.</li>
</ul>
<p>We can convert a list into a NumPy array using: </p>
<pre>
np.array()
</pre>
<p>Ex :-</p>
<pre>
import numpy as np
arr = np.array([1,2,3,4])
print(arr)
</pre>
<h3>Creating Multi-dimensional arrays</h3>
<h4><li>2D array (Matrix)</li></h4>
<p>A list inside a list -> Rows & Columns</p>
<p>Ex :-</p>
<pre>
arr = np.array([[1,2,3],
                [4,5,6]])
print(arr)
</pre>
<h4><li>3D array</li></h4>
<p>Think of it as layers of matrices</p>
<p>Ex :-</p>
<pre>
arr = np.array([
    [[1,2],[3,4]],
    [[5,6],[7,8]]
])
print(arr)
</pre>

<h2>Array attributes</h2>
<p>Array attributes gives information about the array.</p>
<p>Ex :-</p>
<pre>
import numpy as np
arr = np.array([1,2,3],
                [4,5,6])
</pre>
<h3><li>Shape :</li></h3>
<>Shows dimensions(rows, columns) of array.
<pre>
print(arr.shape)
</pre>
<pre>
output : (2,3)
2 rows, 3 columns
</pre>
<p>-> It represents the structure of an array</p>
<h3><li>ndim :</li></h3>
<p>Shows number of dimensions (axes)</p>
<pre>
print(arr.ndim)
</pre>
<pre>
output : 2
because matrix = 2D
</pre>
<h3><li>size :</li></h3>
<p>Total number of elements</p>
<pre>
print(arr.size)
</pre>
<pre>
output : 6
</pre>
<h3><li>dtype :</li></h3>
<p>Shows data type of elements</p>
<pre>
print(arr.dtype)
</pre>
<pre>
output : int
</pre>
<h3><li>item size :</li></h3>
<p>Memory (in bytes) used by one element</p>
<pre>
print(arr.itemsize)
</pre>
<pre>
output : 8
</pre>
<h3><li>nbytes</li></h3>
<p>Total memory used by array</p>
<p><u>Formula</u> = size * itemsize</p>
<pre>
print(arr.nbytes)
</pre>
<pre>
output : 48
6 elements * 8 bytes
</pre>



