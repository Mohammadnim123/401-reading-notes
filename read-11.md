# Jupyter Lab

**JupyterLab is a next-generation web-based user interface for Project Jupyter**.

>JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner.

![JupyterLab](https://jupyterlab.readthedocs.io/en/stable/_images/interface_jupyterlab.png)

**You can arrange multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing, for example:**

* Code Consoles provide transient scratchpads for running code interactively

* Kernel-backed documents enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.

* Notebook cell outputs can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.

* Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers.

# Numpy Tutorial

**NumPy is a commonly used Python data analysis package. By using NumPy, you can speed up your workflow, and interface with other packages in the Python ecosystem, like scikit-learn, that use NumPy under the hood**

**Numpy 2-Dimensional Arrays** 
With NumPy, we work with multidimensional arrays. We’ll dive into all of the possible types of multidimensional arrays later on, but for now, we’ll focus on 2-dimensional arrays. A 2-dimensional array is also known as a matrix, and is something you should be familiar with. In fact, it’s just a different way of thinking about a list of lists. A matrix has rows and columns. By specifying a row number and a column number, we’re able to extract an element from a matrix.

![Numpy](https://fgnt.github.io/python_crashkurs_doc/_images/numpy_array_t.png)

***Creating A NumPy Array***
We can create a NumPy array using the numpy.array function. If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns. 

**Using NumPy To Read In Files**
It’s possible to use NumPy to directly read csv or other files into arrays. We can do this using the numpy.genfromtxt function.

**Broadcasting**
Unless the arrays that you’re operating on are the exact same size, it’s not possible to do elementwise operations. In cases like this, NumPy performs broadcasting to try to match up elements

