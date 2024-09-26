# Introduction to deep learning for scRNA-seq
**Authors: Sandeep Santhosh Kumar, Jiadong Mao, Xiaochen Zhang**

| Audience      | Prerequisites | Duration    |
| ------------- | ------------- | ----------- |
| Anyone    |Install Anaconda (including Python and Jupyter Notebook)|~ 20 min    |
| Anyone    |Install Python Packages|~ 20 min    |


### Description

This repository includes material for a hands-on workshop 'Introduction to deep learning for scRNA-seq'. We show you how to use SCVI-tools to analysis your own scRNA-seq data.

###  Installing Anaconda navigator to set up jupyter notebook environment 
(you can skip this if you already can run jupyter notebooks in an environment)

- A recommended short 5 min youtube video on setting up jupyter notebook can be found [here](https://www.youtube.com/watch?v=Gq167zHsuA0): \
  (https://www.youtube.com/watch?v=Gq167zHsuA0)
- The main steps: 
    - Install [Anaconda navigator](https://www.anaconda.com/download/success), select a graphical installer
    - Create an environemnt. `Environments` on left menu-> `create` option at the bottom -> name the new environemnt and `create`. Python version should be 3.9 or more recent (recommended is 3.9). You can find the documentation [here](https://docs.anaconda.com/navigator/getting-started/) . 
    - Install jupyter notebooks in the environment. `Home` on the left menu -> check if you are on the new environment, the name should be selected on the dropdown menu after `on` on the top of the page -> Click on `install` under the jupyter notebooks icon.
    - Click on `launch` under the  jupyter notebooks icon and navigate to this workshop notebook and proceed to install the packages.

### Installing scvi-tools and some other packages
Open your Jupyernotebook and run these code:

```python
# Only need to run this once, installs the necessary packages,  this will take afew minutes
import sys
!{sys.executable} -m pip install scanpy scvi-tools seaborn scikit-misc igraph leidenalg
```

* Typically, it's better practice to perform conda installations when using conda environments as we are, but if we don't have too many dependencies we get away with pip installations.
