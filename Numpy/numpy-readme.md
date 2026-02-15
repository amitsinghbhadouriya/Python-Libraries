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