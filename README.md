Python Teaching Resources
=========================

By **Tyler Biggs**

---

Getting Started with 3.7
------------------------

1. Install [Anaconda](https://anaconda.org/).

2. Create a new Python 3.7 environment.

    ```bash
    conda create -n py37 python=3.7
    # conda create -n [environment_name] python=[version]
    ```

    Read more about [creating environments](https://conda.io/docs/user-guide/tasks/manage-environments.html).

3. Install [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html).

Using Jupyter Lab
-----------------

__Creating a New IPython Kernel__:

See the [documentation](https://ipython.readthedocs.io/en/stable/install/kernel_install.html) for descriptions of the commands below and more.

```bash
# Activate the environment you wish to create a kernel in.
source activate py37
# Install ipykernel.
conda install ipykernel
# Create the kernel.
python -m ipykernel install --user --name py37 --display-name "Python 3.7"
```

__Launching a server:__

```bash
jupyter lab
```

**Reloading imports:**

```python
%load_ext autoreload  # Load the extension.
%autoreload 2         # Reload all modules (except those excluded by %aimport)
                      # every time before executing the Python code typed.
```

**Enabling imports from parent directories**:

```python
import sys, os
sys.path.insert(0, os.path.abspath('..'))
```

General Python
--------------

+ [Python Built in Functions](https://docs.python.org/3/library/functions.html)

    ```python
    dir(__builtin__)  # Show the namespace of Python's built-in functions.
    ```
+ [Python Standard Library](https://docs.python.org/3/library/) for ubiquitous
  programming needs.

Jupyter Notebook or Lab Specific
--------------------------------

+ [Built in "Magics"](https://ipython.readthedocs.io/en/stable/interactive/magics.html)

Resources
---------

__Notebook Examples__:

+ [A gallery of interesting Jupyter Notebooks](https://github.com/jupyter/jupyter/wiki/A-gallery-of-interesting-Jupyter-Notebooks)
+ [Peter Norvig](https://github.com/norvig/pytudes#pytudes-index-of-jupyter-ipython-notebooks)
+ [Kaggle](https://www.kaggle.com/) Machine Learning Competitions