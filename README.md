# Python Teaching Resources

By **Tyler Biggs**

---

## Getting Started with 3.7

1. Install [Anaconda](https://anaconda.org/).

2. Create a new Python 3.7 environment.

    ```bash
    conda create -n py37 python=3.7
    # conda create -n [environment_name] python=[version]
    ```

    Read more about [creating environments](https://conda.io/docs/user-guide/tasks/manage-environments.html).

## Creating a New IPython Kernel

See the [documentation](https://ipython.readthedocs.io/en/stable/install/kernel_install.html) for descriptions of the commands below and more.

```bash
# Activate the environment you wish to create a kernel in.
source activate py37

# Install ipykernel.
conda install ipykernel

# Create the kernel.
python -m ipykernel install --user --name py37 --display-name "Python 3.7"
```

## Using Jupyter Lab

__Launching a server:__

```bash
jupyter lab
```

### General Python

+ [Python Built in Functions](https://docs.python.org/3/library/functions.html)

    ```python
    dir(__builtin__)  # Show the namespace of Python's built-in functions.
    ```
+ [Python Standard Library](https://docs.python.org/3/library/) for ubiquitous
  programming needs.

### Jupyter Notebook or Lab Specific

+ [Built in "Magics"](https://ipython.readthedocs.io/en/stable/interactive/magics.html)
