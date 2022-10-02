# Python

Python is a high-level *functionnal* coding language. It is easy to learn and use and has loads of packages.

Although `python` is already native in MacOs, we shall use different and up-to-date environments with `conda`. 

## Environments

Here is how to create a new python environment and add modules to it.
```bash
conda create -n myenv python -c mychannel
conda install -n myenv mymodule
```

Then you can activate and desactivate it.
```bash
conda activate myenv
conda deactivate
```

To update a python environment, run:
```bash
conda activate myenv
conda update --all
```
if you want to update one module, prefer
```bash
conda activate myenv
conda update mymodule
```

To get the list of all existing environments and delete one, run:
```bash
conda env list
conda remove -n myenv --all
```

## My setup

I prefer to have 4 separate python environments, one for general use `python-full`, one for mathematics `python-math`, one to install apps `python-app`, and one for sagemath, `sage`.

### General use

```bash
conda create -n python-full python -c conda-forge matplotlib notebook numpy pandoc scipy tkmacosx
```
### Mathematics

```bash
conda create -n python-math python -c conda-forge matplotlib notebook numpy scipy
```
### Apps

```bash
conda create -n python-app python -c conda-forge matplotlib numpy pandoc py2app tkmacosx
```

### SageMath

```bash
conda create -n sage sage -c conda-forge
```