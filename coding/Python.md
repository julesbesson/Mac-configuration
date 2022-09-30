# Python

Python is a high-level *functionnal* coding language. It is easy to learn and use and has loads of packages.

Although `python` is already native in MacOs, we shall use different and up-to-date environments with `conda`. 

## Environments

Here is how to create a new python environment and add packages to it.
```bash
conda create -n <env-name> python -c <channel-name>
conda install -n <env-name> my-package
```

Then you can activate and desactivate it.
```bash
conda activate <env-name>
conda deactivate
```

To update all python environments, run:
```bash
conda update --all
```

To get the list of all existing environments and delete one, run:
```bash
conda env list
conda remove -n <env-name> --all
```

## My setup

I prefer to have 4 separate python environments, one for general use `python-full`, one for mathematics `python-math`, one to install apps `python-app`, and one for sagemath, `sage`.

### General use

```bash
conda create -n python-full python -c conda-forge
conda install -n python-full numpy matplotlib pandoc scipy tkmacosx -c conda-forge
```
### Mathematics

```bash
conda create -n python-math python -c conda-forge
conda install -n python-math numpy matplotlib scipy -c conda-forge
```
### Apps

```bash
conda create -n python-app python -c conda-forge
conda install -n python-gen numpy matplotlib pandoc py2app tkmacosx -c conda-forge
```

### SageMath

```bash
conda create -n sage sage -c conda-forge
```