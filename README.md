## SummerImmersion Hands-on demo

## Setup and installation
Run these R commands in a local clone of this repo

```
install.packages("pak")
pak::local_install()
tensorflow::install_tensorflow()
keras::install_keras()
```

## Python installation

### Set correct python env for use of tensorflow
```
library(reticulate)
conda_envs <- conda_list()
env_name <- conda_envs[2,1] # replace the correct index - choose "r-reticulate" as the envionment
  
# Replace with your environment name
python_path <- conda_python(env_name)
python_path
use_python(python_path)

```

## Bookdown
This project is an R `{bookdown}' project.
Run in the R-Console:

```
install.packages("bookdown")
bookdown::render_book()
```
From the root directory of this repo to get a local copy.
Note: this will only work once you completed the project setup above.
